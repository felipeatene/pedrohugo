# SOS PARCERIA — índice e integração

Material documental para revisão humana e ensaios com dados sintéticos. Não há PDFs reais neste módulo. A existência dos roteiros não comprova execução nem homologação.

## Ordem de leitura

1. [Relatório da sessão](relatorio-da-sessao.md): histórico preservado e limites de verificação.
2. [Protocolo operacional](protocolo-operacional.md): inventário, transcrição, conferência e destinação mensal.
3. [Critérios de auditoria](criterios-de-auditoria.md): distinção entre F, G e H.
4. [Layout e atualização](layout-e-atualizacao.md): cabeçalhos, abas e confirmação da gravação.
5. [Treinamento e checklist](treinamento-e-checklist.md): preparação e revisão humana.
6. [Prompt operacional v1](../../prompts/consolidar-sos-parceria-v1.md): instruções reutilizáveis.
7. [Lote sintético](../../referencias/documentos/lote-sos-ficticio.md) → [gabarito](../../referencias/consolidacoes/sos-ficticio-esperado.md) → [cenários de aceite](../../testes/cenarios-sos-parceria.md).

## Integração com o projeto

O [README principal](../../README.md) apresenta o fluxo geral. Os [cenários gerais](../../testes/cenarios.md) continuam aplicáveis. A pasta canônica é `testes/`; não existe uma segunda suíte em `tests/`.

As [instruções de extração](../../.agents/skills/analisar-pdfs-veterinarios/SKILL.md) e [consolidação](../../.agents/skills/consolidar-dados-veterinarios/SKILL.md), com seus contratos, exigem rastreabilidade e revisão humana. O módulo SOS acrescenta regras de apresentação e conferência documental; não autoriza aprovar registros pendentes nem incluir dados não revisados em indicadores aprovados. Pendências podem constar no inventário operacional, identificadas como tais.

No ensaio, use apenas o catálogo simulado e as páginas simuladas do lote. T-05 demonstra deduplicação, mas não fornece despesas para calcular total. A planilha privada não está anexada: cores exatas, dimensões e gravação no Drive dependem de validação separada no ambiente autorizado.

## Fontes e privacidade

A continuação em 21/10/2026 confirmou a existência dos arquivos na branch, mas o histórico recuperado contém referências a respostas sem seu conteúdo e não disponibiliza os anexos. As afirmações históricas herdadas não foram revalidadas contra os PDFs ou a planilha. A orientação humana de manter setembro e reforçar a falta de datas está visível; não se aplica automaticamente a outros anexos sem data.

Publicar somente instruções e exemplos sintéticos. Não incluir nomes de tutores, contatos, CPF, assinaturas, fotos, IDs reais de documentos, links privados, prontuários, pagamentos ou extrações reais, inclusive em descrições de PR e evidências de teste. O `.gitignore` é proteção auxiliar: não remove arquivos já rastreados nem protege textos sensíveis em Markdown. Revisar o diff e o histórico antes de publicar.

## Validação e liberação

Conferência estática de links, arquivos e coerência do gabarito é distinta de execução do assistente. Os cenários devem ser registrados como aprovado, falhou, bloqueado ou não executado, com evidências sintéticas. A liberação do piloto depende de revisão humana e ambiente autorizado; este PR não equivale a essa liberação.
