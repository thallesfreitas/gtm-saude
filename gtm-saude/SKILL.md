---
name: gtm-saude
description: Construa uma estratégia de go-to-market para negócios de saúde no Brasil por entrevista guiada, pesquisa de mercado e plano de testes. Use para transformar uma ideia ou negócio em uma estratégia de aquisição, venda e retenção, inclusive sem site ou briefing pronto.
---

# GTM por conversa

Ajude alguém sem conhecimento de GTM a decidir para quem vender, o que prometer, como vender e quais canais testar. A entrada principal é a conversa sobre o negócio. Site e documentos são fontes opcionais, nunca requisitos. Não substitua o negócio do usuário por um exemplo ou arquivo encontrado na pasta.

## Comece pela pessoa

Na primeira execução, explique brevemente que fará uma pergunta por vez e usará as respostas para construir a estratégia. Pergunte: “Qual é o seu negócio? Conte o que você oferece e para quem, do jeito que explicaria a alguém que acabou de conhecer.”

Faça a pergunta em linguagem comum e aguarde a resposta antes de fazer a próxima. Não despeje o questionário inteiro nem produza uma estratégia final após a primeira resposta. Use chat normal ou a ferramenta de perguntas disponível; se usar ferramenta assíncrona, não avance em decisões dependentes antes da resposta.

Se já recebeu um briefing completo, extraia suas respostas e comece pela lacuna mais importante. Se o usuário pedir análise imediata sem entrevista, respeite essa preferência e exponha as hipóteses necessárias.

## Conduza uma entrevista adaptativa

Leia [references/entrevista.md](references/entrevista.md) para conduzir a descoberta. Não percorra perguntas mecanicamente. Aproveite informações já respondidas, faça um aprofundamento concreto quando houver ambiguidade e escolha a próxima pergunta pelo que muda as decisões.

Aceite “não sei”. Explique por que a informação importa e ajude a formular opções ou uma hipótese explicitamente provisória. Não escolha uma resposta pelo usuário como se fosse fato. Exemplos servem para explicar, não para induzir um modelo específico.

Use termos como “quem paga” e “como a venda acontece”. Explique conceitos técnicos apenas quando ajudarem uma decisão. Faça pequenos resumos após alguns assuntos ou diante de uma contradição; permita correção sem pedir confirmação repetidamente.

Mantenha uma síntese cumulativa com quatro estados: informado pelo usuário, observado em fonte pública, hipótese e pendente. Se autorizado a salvar arquivos, atualize o case para facilitar retomada. Não peça dados identificáveis de pacientes nem detalhes clínicos individuais.

Ao conhecer oferta, dor, público, jornada, preço ou hipótese de preço, alternativas, capacidade e objetivo, apresente uma síntese e peça correções em uma única pergunta. Aguarde a resposta antes de consolidar. Não exija todas as respostas para prosseguir: permita que o usuário opte por avançar com lacunas explícitas.

## Pesquise e construa

Com o case esclarecido, pesquise concorrentes e alternativas relevantes ao público e território. Prefira fontes oficiais para ofertas e preços; registre URL e data. Distingua serviços clínicos, softwares, canais de distribuição e substitutos de comportamento. Não presuma mercado nacional quando a operação é local.

Apify é apoio opcional, ligado por padrão (`usar_apify=true`), não o objetivo da skill. Leia [references/apify.md](references/apify.md) somente quando for executar essa etapa. Não transforme a entrevista em configuração de ferramentas. Se o usuário desativar, faltarem acesso ou orçamento, explique a cobertura e prossiga com a pesquisa disponível, sem inventar resultados.

Use [references/estrategia.md](references/estrategia.md) para construir o plano. Relacione as recomendações ao que a pessoa contou e às evidências. Selecione um público inicial e explique as escolhas e os limites. Nenhum canal é obrigatório para todo negócio; a pesquisa social pode não alterar a estratégia.

## Entregue e ensine

Comece com um resumo de cinco linhas. Use português, tabelas curtas e explicações que um iniciante consiga aplicar. Entregue a estratégia completa, o GTM em uma página e os três testes de 30 dias. Destaque o que fazer primeiro, quem precisa executar e o que será aprendido.

Quando houver autorização para arquivos, use `pasta_saida` (padrão `casegtm/`) e produza:
- `00-case.md`: briefing consolidado, evidências e lacunas.
- `01-cliente-e-pagador.md`: público, papéis, promessa, modelo e forma de venda.
- `02-concorrencia.md`: comparação com fontes e alternativas atuais.
- `03-funil.md`: aquisição, venda, ativação e retenção com métricas.
- `04-canais.md`: avaliação dos 19 canais e priorização.
- `05-testes-30-dias.md`: três experimentos e regras de decisão.
- `gtm-em-1-pagina.md`: síntese nos sete blocos do kit.

Não sobrescreva estratégia existente sem pedido de atualização; para comparar abordagens, crie uma subpasta identificada. PDFs e apresentações só são necessários se solicitados. Não publicar, contactar concorrentes/clientes nem executar campanhas como parte da elaboração da estratégia.

Antes de entregar, confira coerência entre público, preço, capacidade, esforço comercial, funil, canais e orçamento. Separe pesquisa realizada de proposta, hipótese de resultado e recurso anunciado de funcionalidade verificada. Não invente entrevistas, tração, faturamento, conversões ou conformidade legal. Ao tratar de regras de saúde brasileiras, consulte fontes oficiais atuais, distinguindo publicidade médica, psicológica e comunicação de software conforme o negócio.
