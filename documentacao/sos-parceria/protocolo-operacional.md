# Procedimento operacional padrão — SOS PARCERIA

**Objetivo:** consolidar fichas médico-veterinárias e despesas em uma planilha mensal, com comparação à tabela pactuada e registro de divergências, mantendo rastreabilidade por página.

## A. Pré-requisitos

Confirme antes de processar: (a) Plano de Trabalho e tabela pactuada **vigentes**, inclusive aditivos; (b) PDF integral e nome/ID exatos no SEI; (c) planilha de consolidação aprovada; (d) ambiente autorizado para dados reais e cópias de segurança; (e) autorização para editar a planilha específica.

Planilhas e PDFs reais permanecem fora do GitHub público. A leitura de PDF escaneado pode exigir OCR aprovado, revisão da imagem e verificação de tabelas; extração automática sem conferência visual não basta.

## B. Inventário integral das páginas

- Registrar contagem de páginas físicas e quais contêm ficha, laudo, fotografia, evolução, cirurgia, exames, demonstrativo, NF, recibo ou comprovante.
- Identificar início/fim de cada ficha, incluindo demonstrativos continuados na página seguinte.
- Criar identificador documental de cada atendimento; separar **atendimentos distintos de um mesmo animal** sem somar duas vezes o mesmo recibo.
- Conferir associação dos demonstrativos ao animal. Se um comprovante traz nome de outro animal, manter **associação pendente**.
- Anotar campos ausentes/ilegíveis, datas não informadas, descontos, cobrança coletiva e valores em aberto.

**Unidades diferentes:** ficha ≠ animal único ≠ atendimento ≠ venda ≠ procedimento ≠ comprovante. Um anexo pode ter várias fichas do mesmo animal ou uma ficha referente a um grupo.

## C. Transcrição financeira exaustiva

Para cada item do documento original, conservar:

| Campo | Exemplo fictício |
|---|---|
| Data do serviço | 03/10/2025 ou “não identificada” |
| Descrição original | “Hemograma + perfil bioquímico” |
| Quantidade | 1 |
| Valor unitário | R$ 120,00 |
| Valor de linha | R$ 120,00 |
| Desconto específico | R$ 0,00 |
| Total líquido atribuível | R$ 120,00 |
| Fonte | arquivo, página física, número da linha/venda (em manifesto privado) |
| Associação | animal/ficha identificada ou pendente |

Não ignorar **medicações, suplementos, materiais, taxas, exames, procedimentos, diárias, sondas, seringas, anestesia** e outras linhas de custo. Não converter pacote em itens unitários sem comprovante.

Quando há datas distintas, a célula F segue o padrão:

~~~text
03/10/2025  [data formatada em negrito]
Consulta — 1 unidade — R$ 75,00.
Exame — 1 unidade — R$ 120,00.

04/10/2025  [data formatada em negrito]
Internação — 1 diária — R$ 100,00.
~~~

Os códigos de venda saem da **apresentação**, mas devem ficar no registro de proveniência privado. Não colocar total cobrado no fim da célula F.

## D. Conferência aritmética

1. Recalcular cada linha: quantidade × unitário.
2. Somar todas as linhas **do animal e do atendimento**, sem duplicidade.
3. Deduzir somente descontos que a documentação permite atribuir.
4. Comparar total do demonstrativo, NF e comprovante de transferência separadamente.
5. Registrar divergências, inclusive diferenças pequenas.
6. Não ratear descontos coletivos ou despesas conjuntas sem regra documental.
7. Um documento “em aberto” ou orçamento não equivale a pagamento confirmado.

Quando a fonte apresenta preço unitário inconsistente com seu total, copiar **ambos os campos originais** e registrar a diferença em H. Não preencher número “corrigido” pela IA.

## E. Verificação de pactuação

Para cada item, procurar a entrada no Plano com:

- nomenclatura, descrição técnica e modalidade;
- espécie e peso/porte quando relevantes;
- método do exame;
- serviço versus compra de produto;
- preço unitário e número do item.

A classificação de G é restrita a **não pactuados ou preço unitário acima do pactuado**. Se a nomenclatura é diferente, mas o serviço correspondente está previsto e custa menos, fica fora de G; H pode mencionar a diferença de descrição. Se a correspondência técnica não puder ser confirmada, registrar a dúvida sem impor equivalência artificial.

Não equiparar automaticamente **compra de medicamento** à **aplicação de medicação**, nem uma anestesia sem modalidade à inalatória; avaliar item por item.

## F. Documentação clínica

- Coluna B: foto existente e associável ao animal, quando comprovada.
- Coluna C: laudo/relatório **do caso** identificando veterinário responsável e CRMV; resultados isolados de exames não o substituem.
- Coluna H: registrar ausências ou inconsistências de datas, evolução, exame, cirurgia, anestesia, fotos, responsável técnico.
- Castração, **inclusive associada a piometra**, exige verificação de microchipagem e número/registro.
- Internação: conferir datas de admissão, alta, diárias e evolução por turno.
- Em venda coletiva: registros de execução, despesas e pagamentos **por animal**.
- Para perfis bioquímicos: discriminar analitos quando a tabela é por parâmetro; não inventar preços unitários de pacote.

## G. Destinação mensal e escrita na planilha

1. Encontrar o primeiro mês documentado no anexo, usando datas de atendimento/exame relacionadas ao caso.
2. Todas as fichas **do mesmo anexo** ficam na mesma aba do mês inicial, mesmo que procedimentos atravessem meses.
3. Se não houver data, **pedir decisão humana**; registrar no histórico da consolidação que o mês foi indicado manualmente.
4. Comparar existência de possível duplicata; se realmente idêntica, **não repetir pacientes**. Cabeçalho de cinco células com os nomes exatos dos dois arquivos SEI.
5. Caso um só arquivo, cabeçalho com **quatro células**.
6. Preservar a linha de títulos vermelha, o cabeçalho rosa, uma linha vazia entre anexos e o estilo do modelo validado.
7. Abrir altura suficiente para texto em F/G/H, inclusive descrições longas.
8. Aplicar negrito em **trechos de data**, sem deixar procedimento inteiro em negrito.
9. Não alterar outras abas, fórmulas ou blocos.

## H. Validação final e comunicação

Antes de declarar conclusão, conferir:
- páginas examinadas vs. páginas existentes;
- nº esperado vs. nº efetivo de fichas;
- itens efetivos vs. itens da fonte;
- G sem itens pactuados abaixo do valor;
- H com datas e ausências relevantes;
- somas/descontos/NF/transferências com divergências registradas;
- duplicidades e associação correta por animal;
- cabeçalho completo com nome do SEI sem alterações;
- aba mensal correta e anexo inteiro;
- formatação do modelo e linha vazia separadora;
- **leitura posterior do intervalo gravado no Drive**.

Status possíveis: **preparado**, **parcial**, **gravado sem conferência**, **conferido**, **pendente de decisão humana**. Falha de gravação deve ser comunicada como falha; não criar alegação de sucesso.

## I. Limites da análise

Esta planilha documenta achados para posterior RTMA, não substitui a diligência formal nem determina, por si só, desvio de finalidade ou aprovação da despesa. As classificações de gravidade discutidas pela equipe são **internas** e não devem aparecer como rótulos em H. O texto das observações deve ser técnico, direto e curto, sem pedidos de retificação antes da etapa processual apropriada.
