# Lote SOS-TREINO-001 — DOCUMENTO FICTÍCIO

**IMPORTANTE: EXEMPLO SINTÉTICO.** Este arquivo **não é transcrição, reprodução nem anonimização reversível** de qualquer prontuário, nota ou documento real. Nomes genéricos, IDs e valores de situações combinadas são inventados para testar as regras estabelecidas. Nenhum registro abaixo prova execução, pagamento ou pactuação de serviços reais.

## Plano de preços SIMULADO para este teste

| Item hipotético | Serviço | Preço unitário máximo |
|---|---|---:|
| P-01 | Consulta clínica comum | R$ 100,00 |
| P-02 | Hemograma | R$ 75,00 |
| P-03 | Anestesia inalatória | R$ 300,00 |
| P-04 | Aplicação de medicação em animal pequeno | R$ 35,00 |
| P-05 | Esterilização canina com microchipagem | R$ 400,00 |
| P-06 | Teste felino A/B | R$ 200,00 |

O catálogo fictício **não prevê** sedação avulsa nem suplemento por embalagem. Não use este quadro em lotes reais.

## Documento T-01 — cão submetido à esterilização

**Páginas simuladas 1–3.**

- Ficha T-01.1; animal: **Paciente A**; canino; atendimento em 05/10/2025.
- Relatório: esterilização eletiva; documento médico com assinatura, mas sem número de microchip anexado.
- Foto: sim.
- Demonstrativo:
  - Consulta clínica comum: 1 × R$ 90,00 = R$ 90,00.
  - Hemograma: 1 × R$ 60,00 = R$ 60,00.
  - Esterilização canina com microchipagem: 1 × R$ 400,00 = R$ 400,00.
  - Anestesia inalatória: 1 × R$ 350,00 = R$ 350,00.
- Há resultado do hemograma, mas **não** há número de microchip e comprovante de registro.

## Documento T-02 — cobrança de grupo sem individualização

**Páginas simuladas 4–5.**

- Relatório informa “quatro gatos vacinados e testados”; não apresenta códigos individuais nem fotos associáveis aos quatro.
- Demonstrativo coletivo: 4 testes felinos A/B × R$ 130,00 = R$ 520,00.
- Demonstrativo coletivo: 4 vacinas felinas × R$ 90,00 = R$ 360,00.
- O Plano fictício prevê teste felino A/B, mas não prevê **vacina felina**.
- Nota fiscal apresenta cobrança agregada. Não existe discriminação dos pagamentos individualizados por animal.

## Documento T-03 — datas múltiplas, desconto global e produto

**Páginas simuladas 6–9.**

- Ficha T-03.1: **Paciente B**, felino. Dias de atendimento: 07/10 e 08/10/2025.
- 07/10: aplicação de medicação, 2 × R$ 25,00 = R$ 50,00.
- 08/10: suplemento por embalagem, 3 × R$ 58,00 = R$ 174,00.
- Ficha T-03.2: **Paciente C**, canino. Atendimento em 08/10/2025.
- 08/10: consulta comum, 1 × R$ 80,00 = R$ 80,00.
- O demonstrativo único dos dois animais oferece **desconto global de R$ 25,00**, sem indicar como se reparte.
- A ficha do Paciente C menciona exame não cobrado, mas **não** apresenta resultado desse exame.

## Documento T-04 — erro aritmético, datas ausentes e orçamento

**Páginas simuladas 10–11.**

- Ficha T-04.1: **Paciente D**, canino, datas de atendimento e internação ausentes.
- Orçamento: banho terapêutico, quantidade 1, preço unitário R$ 100,00, valor total de linha R$ 230,00.
- Orçamento: sedação avulsa, quantidade 1, preço unitário R$ 180,00, valor total de linha R$ 180,00.
- Não há recibo, nota de quitação ou comprovante bancário.
- Emissão do orçamento: 15/11/2025, **não** considerada data automática dos procedimentos.

## Documento T-05 — arquivo repetido

**Páginas simuladas 12–14.**

Documento **T-05-B** reproduz o texto, as despesas e todas as fichas do **T-05-A** (duas versões documentais com IDs diferentes; equivalência já conferida no cenário fictício). Os nomes oficiais hipotéticos são “Anexo Clínico Original” e “Anexo Clínico Reapresentado”.

**Resultado esperado:** um cabeçalho com **cinco células** e um único conjunto de fichas; não somar os valores duas vezes.

## Documento T-06 — laudo de exame não é laudo de caso

**Páginas simuladas 15–16.**

- Ficha T-06.1: **Paciente E**, canino.
- Despesa: “Hemograma + bioquímico”, 1 pacote por R$ 120,00.
- Anexo: resultado do hemograma assinado pela unidade laboratorial; **não** consta relatório clínico individualizado ou CRMV do veterinário solicitante.
- Pacote sem analitos bioquímicos e respectivos preços discriminados.

## Tarefa do treinamento

1. Criar uma lista completa de itens (sem omitir produtos ou despesas grupais).
2. Preencher um consolidado **fictício** A–I, com datas em negrito e preços originais.
3. Confrontar cada linha ao Plano hipotético.
4. Registrar na coluna G somente itens realmente não pactuados ou acima dos valores do quadro.
5. Registrar na H a falta de microchip, individualização, laudo, datas, compatibilidade aritmética e situação do pagamento.
6. Não ratear desconto de T-03.
7. Não usar data do orçamento de T-04 como data de atendimento.
8. Não duplicar T-05-A/T-05-B.
9. Manter os IDs e as nomenclaturas exatas dos documentos fictícios.
10. Conferir o resultado com [gabarito explicado](../consolidacoes/sos-ficticio-esperado.md).

**Proibição:** os preços hipotéticos desta referência não podem alimentar a tabela de produção.
