# Layout, cabeçalhos e atualização da planilha

## Estrutura mensal

As abas de prontuários são mensais. As abas de notas fiscais são **separadas** e não devem receber prontuários.

- Cada **anexo inteiro** fica na aba do primeiro mês documentado no arquivo, mesmo quando há exames ou internações posteriores em outro mês.
- Em ausência de data confiável, não escolher mês por adivinhação. A decisão expressa da pessoa responsável autoriza a inclusão em um mês informado, com H registrando a ausência das datas.
- Exatamente **uma linha totalmente em branco** entre blocos de anexos.
- O preenchimento de um novo bloco não pode sobrescrever linhas, fórmulas, abas ou anexos anteriores.

## Cabeçalhos definitivos: reproduzir exatamente o nome do SEI

### Um único arquivo — quatro células

| Célula de informação | Conteúdo |
|---|---|
| 1 | ID do documento no SEI |
| 2 | **Nomenclatura integral e exata** do arquivo no SEI |
| 3 | Clínica |
| 4 | Município |

### Dois arquivos iguais — cinco células

| Célula de informação | Conteúdo |
|---|---|
| 1 | IDs dos dois documentos |
| 2 | **Nomenclatura exata** do primeiro arquivo no SEI |
| 3 | **Nomenclatura exata** do segundo arquivo no SEI |
| 4 | Clínica |
| 5 | Município |

**Não** unir os nomes de arquivos na mesma célula, abreviar, renomear, remover pontuação ou criar nomes explicativos. Antes de adotar cabeçalho duplo, **verificar que os arquivos realmente descrevem os mesmos atendimentos** e registrar diferenças documentais caso existam.

## Referência visual canônica

Na sessão, a **linha 11 da aba “Ago - 25”** foi declarada modelo obrigatório para a formatação do cabeçalho. A faixa de títulos da tabela usa **vermelho-escuro**; o cabeçalho usa **rosa-claro**, incluindo Município. A altura e a largura precisam reproduzir o modelo.

Conferir a combinação:
- preenchimento, fontes, bordas, alinhamento horizontal e vertical;
- centralização e quebra automática do texto;
- altura do cabeçalho e altura de conteúdo suficiente para exibir todos os caracteres;
- posicionamento de campos sem deslocar município ou clínica;
- títulos de A a I **somente na faixa vermelha**, nunca repetidos nas células F–I do cabeçalho;
- **datas em negrito**, isoladamente, nos grupos de procedimentos;
- procedimentos/quantidades/valores na fonte regular;
- preservação dos estilos antigos em outras abas.

A referência visual pertence à planilha operacional **privada**. Um exemplo fictício deste GitHub não substitui essa planilha aprovada.

## Apresentação dos procedimentos na coluna F

~~~text
[Data em negrito — usar formatação parcial da célula]
05/10/2025
Consulta — 1 unidade — R$ 75,00.
Hemograma — 1 unidade — R$ 60,00.

[Data em negrito — usar formatação parcial da célula]
06/10/2025
Internação — 2 diárias — R$ 100,00 cada — R$ 200,00.
~~~

Sem códigos internos de venda no texto final; preservar as chaves do sistema de origem em registro privado. Sem total geral do atendimento no final da célula.

## Regras da atualização no Drive

1. Identificar o **documento canônico** e a aba correta.
2. Registrar os intervalos antes da alteração e fazer cópia de segurança/versionamento apropriado.
3. Conferir o próximo bloco vazio; inserir separador e cabeçalho.
4. Transcrever as células F, G, H preservando os demais campos.
5. Aplicar estilo **pelo modelo aprovado**, não com cor aproximada ou suposições.
6. Autoajustar alturas, testar descrições longas e datas em negrito parcial.
7. Ler novamente o intervalo gravado e comparar número de linhas, descrições e valores.
8. Informar somente o status verdadeiro: preparado, parcial, gravado ou conferido.

**Erros de execução anteriores:** a sessão relatou arquivos que não abriam, cópias locais desatualizadas, meses separados dentro do mesmo anexo, títulos duplicados, Município fora da cor rosa e alturas insuficientes. Todos esses itens integram a conferência obrigatória.
