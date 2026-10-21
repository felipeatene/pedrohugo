---
name: consolidar-dados-veterinarios
description: Consolidar extrações veterinárias revisadas em tabelas, relatório e insights rastreáveis com ações sugeridas. Usar após extração documental, distinguindo registros aprovados, pendentes e excluídos.
---

# Consolidar e gerar insights

Leia [o contrato](references/contrato.md) antes de calcular ou relatar. Identifique raiz do projeto, lote, versões dos campos, extrações, revisões humanas e destino autorizado. Use referências de consolidação para apresentação, sem importar seus fatos para a base atual.

## Privacidade

JSON e relatórios também podem conter dados sensíveis. Antes de ler dados reais, confirme autorização e ambiente de processamento verificado no contexto existente. Se faltar essa definição, trabalhe apenas com exemplos fictícios até esclarecimento. Não enviar conteúdo a serviço externo nem publicar resultados por conta própria.

## Fluxo

1. Inventarie arquivos e a unidade de contagem. Confira compatibilidade de versões e campos, registros duplicados e revisões correspondentes à versão exata da extração. Não escolher silenciosamente entre revisões conflitantes.
2. Separe aprovados, pendentes, rejeitados e incompatíveis. Aprovação precisa de registro humano rastreável; status no JSON extraído, sozinho, não basta. Use os aprovados para indicadores de conteúdo e o inventário completo somente para indicadores de fluxo claramente identificados.
3. Aplique correções humanas rastreáveis à versão derivada, preservando o histórico. Não contar extração e revisão como duas avaliações. Não deduplicar animais por nome.
4. Calcule contagens e percentuais de forma reproduzível com ferramentas autorizadas disponíveis. Informe numerador, denominador, unidade, período e ausências. Se não conseguir verificar um cálculo, sinalize-o como não validado e não o apresente como fato pronto para decisão.
5. Gere CSV e relatório conforme modelos e contrato, preservando vínculos com record_id, document_id, versão e revisão. Liste exclusões e motivos. Se não houver aprovados, entregue relatório de pendências sem inventar indicadores clínicos.
6. Para cada insight, separe fato, interpretação, limitação, evidência e ação sugerida. Prioridade deve ter justificativa e responsável fica a definir quando não informado. Não invente prazo acordado.
7. Confira que as somas reconciliam com a base e que nenhuma hipótese aparece como fato. Entregue os arquivos e limites para decisão humana; não envie mensagens, altere sistemas nem execute ações propostas.

Não diagnosticar, recomendar tratamento, atribuir causalidade ou extrapolar prevalência populacional a partir da amostra documental. Tendência requer períodos comparáveis e base suficiente; caso contrário, explique a limitação.
