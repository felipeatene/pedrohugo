# Treinamento da analista e checklist de conferência

Este guia permite treinar um assistente de IA sem presumir que o prompt, sozinho, “aprendeu” os procedimentos. **O modelo deve consultar o Plano, o modelo aprovado e os documentos do lote em toda execução.** O treinamento é um protocolo de instruções + exemplos + correções humanas verificáveis.

## Sequência de treinamento proposta

| Etapa | Exercício | Critério de aprovação |
|---|---|---|
| 1 — Contexto | Ler protocolo e contrato G/H | Explicar a distinção F/G/H sem equívocos |
| 2 — Exemplo pequeno | Processar T-01 | Detectar anestesia acima do pacto e microchip ausente |
| 3 — Atendimento coletivo | Processar T-02 | Não inventar animais individualizados |
| 4 — Itens e descontos | Processar T-03 | Distinguir produto, aplicação e desconto global |
| 5 — Inconsistência documental | Processar T-04 | Preservar números divergentes; orçamento não é pagamento |
| 6 — Duplicidade | Processar T-05 | Usar cabeçalho com cinco células, sem duplicar fichas |
| 7 — Exame clínico | Processar T-06 | Diferenciar laudo de laboratório e laudo do caso |
| 8 — Projeto real autorizado | Um anexo pequeno com revisor | Todos os itens e valores rastreáveis por página |
| 9 — Escalar | Lotes maiores | Nenhuma etapa de conferência omitida |

**Importante:** os dados de exemplo no repositório são fictícios. Somente após validação do ambiente autorizado e da política de privacidade podem ser fornecidos PDFs reais ao assistente.

## Documentos que o operador deve fornecer ao modelo

- Versão vigente do Plano de Trabalho e catálogo de preços.
- Planilha canônica atual, com cabeçalho e registros já aprovados.
- Anexos/PDFs autorizados e nomenclaturas SEI exatas.
- Documento com decisões e regras vigentes (este guia).
- Orientação sobre a aba desejada quando não há mês identificável.
- Identificação da unidade de trabalho: ficha, animal, atendimento, demonstrativo, sem confundi-las.

## Checklist antes de gravar

- [ ] Li **todas** as páginas e continuações de cada demonstrativo.
- [ ] Tenho inventário de todas as fichas, grupos e animais não identificados.
- [ ] Preservei todos os lançamentos, mesmo materiais/medicamentos menores.
- [ ] Guardei página, descrição, quantidade, valor unitário e total original.
- [ ] Recalculei linhas, desconto e total, sem corrigir números da fonte por palpite.
- [ ] Comparei cada procedimento com o item e a modalidade **corretos** do Plano.
- [ ] G só contém não pactuados e valores **acima** da referência.
- [ ] Itens pactuados **abaixo** da referência não foram incluídos em G.
- [ ] H apresenta ausência de datas, laudos, CRMV, microchip, evolução e discriminação.
- [ ] Não transformei item de exame em laudo do caso.
- [ ] Não associei despesa coletiva, desconto global ou produto a um animal por suposição.
- [ ] Identifiquei os itens pagos e não pagos **por animal e atendimento**, ou registrei que faltam dados para isso.
- [ ] Não confundi NF/orçamento/em aberto com comprovante de pagamento.
- [ ] Comparei possíveis anexos repetidos antes de somar fichas.

## Checklist depois de gravar

- [ ] Mesmo anexo está integralmente em uma aba mensal.
- [ ] A seleção do mês está apoiada em data **documentada** ou escolha humana registrada.
- [ ] Há uma linha vazia entre os blocos.
- [ ] Cabeçalho é de **quatro ou cinco células**, conforme número de arquivos idênticos.
- [ ] Nomes de arquivos são idênticos ao cadastro no SEI.
- [ ] Cabeçalho segue integralmente o estilo da **linha 11 de agosto** da planilha privada.
- [ ] Títulos A–I estão na faixa vermelha, não repetidos no cabeçalho.
- [ ] Município acompanha o padrão rosa do cabeçalho.
- [ ] Datas na coluna F estão em **negrito parcial** e acima dos procedimentos.
- [ ] As células F/G/H mostram todo o texto, sem truncamento por altura.
- [ ] Reabri/relí a planilha do Drive e confirmei que as alterações estão gravadas.
- [ ] Não modifiquei abas de NF nem dados consolidados anteriormente.

## Como avaliar e corrigir o assistente

Quando encontrar um erro, não reescrever apenas uma célula. Registre:
1. Referência do anexo/ficha (internamente);
2. página e valor original;
3. regra violada (ex.: G contém item abaixo do pacto);
4. correção exigida;
5. validação da nova saída;
6. se é um erro recorrente, novo cenário no conjunto de testes.

Se o assistente disser “concluído” antes de verificar todos os itens, exigir relatório de cobertura: páginas lidas, fichas, linhas financeiras, somas conferidas, dúvidas e status real da gravação.

## Critério mínimo para liberação do piloto

**Revisão humana integral**, confirmação das chaves de origem, nenhuma despesa omitida nos exemplos, cálculos reconciliados ou divergências explicitadas, formatação aprovada e gravação confirmada. Não confiar em percentual de “acurácia” declarado pelo próprio assistente sem comparação com gabarito humano.

## Modelo de relatório de conclusão

~~~text
Anexo/documento: [nome SEI completo]
IDs vinculados: [identificadores no ambiente privado]
Período documentado: [ou “ausente”]
Aba: [mês e justificativa]
Fichas identificadas: [n]
Itens financeiros transcritos: [n]
Somas reconciliadas: [n] de [n]; divergências: [detalhes]
Pendências: [quais]
G auditada contra o Plano: [sim/não; versão]
Formatação e linhas conferidas: [sim/não]
Read-back do Drive: [sim/não]
Estado: preparado / parcial / gravado / conferido
~~~

Não utilizar números inventados em relatórios de execução.
