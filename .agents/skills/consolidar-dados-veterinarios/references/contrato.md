# Contrato de consolidação versão 0.2

Entradas: JSON de extração no contrato 0.2 e revisões com review_id, record_id, versao_extracao, decisao, revisor_id, instante e alteracoes. No ensaio, use os arquivos fictícios explicitamente designados. Em produção, nunca trate revisões fictícias como autorização.

## Elegibilidade

A decisão aprovar deve referir-se à versão exata e não ter conflito com outra decisão vigente. Uma correção deve incluir campo, valor anterior, novo valor, motivo e evidência. Se faltarem metadados de revisão, a versão não corresponder ou houver conflito não resolvido, excluir dos indicadores e listar pendência. Não inferir aprovação de pasta, nome de arquivo ou confiança do modelo.

A unidade padrão é avaliação por documento. Sem chave confiável, não converter para animais únicos. Dois PDFs diferentes podem descrever o mesmo atendimento; sinalizar possíveis duplicatas sem decidir por nome. Repetição do mesmo record_id/versão conta uma vez, após comparar conteúdo; divergência exige revisão.

## Entregáveis

1. consolidado.csv: uma linha por avaliação aprovada, com record_id, document_id, versao_extracao, review_id e campos definidos. UTF-8, ponto e vírgula; preservar acentos, citar delimitadores e quebras. Neutralizar células textuais iniciadas por =, +, -, @, tabulação ou retorno, mantendo original no JSON privado.
2. relatorio.md: objetivo/período, base, exclusões, panorama, insights, ações e limitações. Usar modelos/relatorio.md.
3. pendencias.md: identificadores, etapa, motivo e próximo passo; separar contagens operacionais de conteúdo clínico.
4. manifesto.json: arquivos e hashes de entrada quando disponíveis, versões, IDs/revisões incluídos e excluídos, fórmulas e contagens. Registrar data e identificador da consolidação; não inventar hashes nem evidências.

## Regras de interpretação

Percentual sem denominador não é aceito. Ausência não equivale a resposta negativa. Comparações exigem definições e períodos compatíveis. Amostra pequena deve ser apresentada como descritiva. Referenciar achados nos registros e evidências originais; pendências podem se apoiar no inventário e no motivo da revisão.

Quando não houver dados para um insight, dizer o que falta. Toda ação é sugestão para avaliação humana, com prioridade justificada, responsável a definir e sem execução externa.
