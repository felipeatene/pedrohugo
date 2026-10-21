# Contrato de extração versão 0.2

A raiz do projeto fornece configuracao/campos.local.json (piloto) ou campos.example.json (ensaio). Leia referencias/extracoes/ficha-exemplo.md e lote-ficticio.json apenas como forma esperada.

## Saídas

- Markdown por documento com `<!-- pagina_pdf: N -->`, N físico iniciado em 1; preservar páginas vazias e indicar método por página.
- Ficha por registro com valores, página, trecho e pendências; seguir modelos/ficha.md.
- JSON de lote com versao_contrato, lote_id, tipo_dados, versao_campos e registros.
- Cada registro contém record_id, document_id, versao_extracao, status `em_revisao`, campos e pendencias. Uma unidade é uma avaliação documentada, não um animal único global.
- Cada campo contém valor_original, valor_normalizado, situacao, evidencias e confianca_calibrada.
- Situações: encontrado, ausente, ilegivel, conflitante, nao_aplicavel. Valores sem leitura segura são null. Conflitos preservam alternativas e suas evidências. Não aplicável requer motivo.
- Cada evidência contém pagina_pdf positiva e trecho literal; acrescente metodo quando conhecido. Para ilegível, cite o trecho legível ao redor e explique a limitação, sem inventar a parte ausente.
- Confianca_calibrada é null no piloto. Aprovação existe somente em registro humano separado, vinculado a record_id e versao_extracao; mudança invalida a aprovação anterior para a nova versão.

## Identidade e auditoria

Em produção, document_id deve permitir localizar o PDF por manifesto privado, preferindo SHA-256 dos bytes. Registrar hash, versões da skill/campos/extrator/OCR/modelo e instante de execução em manifesto privado. IDs DOC-001 dos exemplos são identificadores fictícios, não hashes.

Não unir pacientes pelo nome. Se houver vários atendimentos, criar record_id distinto com vínculo à evidência. JSON inválido exige correção de formato sem inventar conteúdo; se a correção falhar, registrar erro e encaminhar para revisão. Arquivo parcialmente lido não recebe cobertura completa.
