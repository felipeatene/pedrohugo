# Cenários de teste — consolidação SOS PARCERIA

**Somente material fictício.** Fontes: [lote de treinamento](../referencias/documentos/lote-sos-ficticio.md) e [gabarito](../referencias/consolidacoes/sos-ficticio-esperado.md).

| Caso | Entrada | Resultado obrigatório |
|---|---|---|
| 01 | Consulta abaixo do valor pactuado | F preenchida; **G vazia** para o item |
| 02 | Anestesia inalatória acima do valor | G com item pactuado, preço e diferença |
| 03 | Produto/suplemento sem item próprio | Não tratar automaticamente como aplicação de medicamento |
| 04 | Castração sem número de microchip | H com falta da comprovação, ainda que F tenha “com microchipagem” |
| 05 | Piometra com castração | Exigir mesma verificação de microchipagem |
| 06 | Pacote de hemograma + bioquímica | H aponta analitos e valores não discriminados; sem inventar parâmetros |
| 07 | Laudo de exame sem relatório clínico | C/H reconhecem insuficiência de laudo do caso |
| 08 | Quatro animais em uma conta | Não criar quatro animais identificados nem dividir valor por suposição |
| 09 | Desconto conjunto sem rateio | Valores e desconto preservados; H registra individualização ausente |
| 10 | Quantidade × preço diferente do total de linha | Preservar os números originais e apontar a diferença |
| 11 | Orçamento ou “em aberto” | Não rotular como pago |
| 12 | Atendimento sem datas e NF datada | Não inferir data clínica da NF |
| 13 | Anexo começa em agosto, termina em setembro | Todas as fichas em **agosto** |
| 14 | Anexo sem qualquer data | Suspender mês até orientação humana expressa |
| 15 | Dois arquivos com conteúdo idêntico e nomes diferentes | Um conjunto de registros; cabeçalho com cinco células e nomes exatos |
| 16 | Arquivo único | Cabeçalho com quatro células |
| 17 | Cabeçalho com Município fora do rosa | Falha no teste visual |
| 18 | Títulos da tabela em célula F do cabeçalho | Falha de estrutura |
| 19 | Linha sem altura suficiente e texto cortado | Falha de legibilidade |
| 20 | Falta linha vazia entre anexos | Falha de layout |
| 21 | Datas em negrito juntamente com valores | Falha: negrito deve ser apenas nas datas |
| 22 | Assistente gera Excel local, mas diz que editou Drive | Falha: status incorreto |
| 23 | Documento repetido aparece com ID novo | Conferir conteúdo antes de deduplicar |
| 24 | Demonstrativo em nome de outro paciente | Não atribuir valores ao paciente da ficha |
| 25 | Nota fiscal e demonstrativo divergem | H com valores/documentos sem reconciliação artificial |
| 26 | Medicamento abaixo de referência realmente aplicável | Fora de G, mas preservar F |
| 27 | RTMA ainda não elaborado | H factual; sem solicitar formalmente retificação |
| 28 | Pagamento sem associação individual ao animal | OSC deve discriminar pagos e não pagos por animal e atendimento |

## Verificações automatizáveis

- Contagem de linhas de ficha por anexo vs inventário.
- Unicidade da chave (ID de documento + ficha + versão), preservando duplicatas confirmadas de documentos.
- Nenhum cabeçalho com títulos A–I indevidos nas suas células de dados.
- Exatamente uma linha vazia antes do próximo bloco.
- Altura e quebra de texto compatíveis com conteúdo.
- Separação das abas prontuários e NF.
- Valor de linha calculado contra quantidade × unitário, com campo para divergências.
- Presença de referência do item pactuado em todo apontamento de excesso em G.
- Prova de leitura posterior do intervalo efetivamente salvo.

## Homologação

Estes são critérios esperados, **não resultados de testes já executados**. Para homologar, registrar data, modelo, executor, versões dos arquivos, revisão humana e diferença entre saída e gabarito. A execução com documentos reais depende de autorização específica e proteção de dados.
