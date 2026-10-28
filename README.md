# GTM Saúde

Skill para construir uma estratégia de go-to-market de negócios de saúde no Brasil por uma entrevista didática, com uma pergunta por vez.

Não exige site nem briefing pronto. Parte da descrição do empreendedor, ajuda a esclarecer decisões e combina as respostas com pesquisa de mercado.

## Instalar no Codex

Envie esta mensagem ao Codex:

```text
Use $skill-installer para instalar:
https://github.com/thallesfreitas/gtm-saude/tree/main/gtm-saude
```

## Começar

```text
Use $gtm-saude para construir a estratégia do meu negócio.
```

A primeira pergunta é sobre o negócio. As seguintes se adaptam às respostas: problema, público, jornada, preço, alternativas, recursos e objetivo. Você pode responder “não sei”; a skill ajuda a formular hipóteses sem tratá-las como fatos.

Se já tiver um briefing, envie-o junto. Site e documentos são opcionais.

## Entregas

- Case consolidado e definição de cliente, decisor e pagador.
- Promessa, posicionamento e forma de venda.
- Concorrência e alternativas com fontes.
- Funil de aquisição, ativação, venda e retenção.
- Avaliação dos 19 canais de Tração e priorização.
- Três experimentos de 30 dias e GTM em uma página.

Os arquivos são salvos em `casegtm/`, ou na pasta indicada, quando houver autorização de escrita. Pesquisa, hipóteses e resultados observados são identificados separadamente.

## Pesquisa com Apify

Ligada por padrão como apoio para analisar comunicação pública no Instagram. Precisa de acesso ao Apify na ferramenta usada e de orçamento autorizado para coleta paga. A skill não inclui credenciais, créditos nem conexão automática.

Para desativar:

```text
Use $gtm-saude para construir minha estratégia, com usar_apify=false.
```

Aceita menos perfis que o limite quando só houver poucos pertinentes e confirmados. Seguidores e curtidas não são tratados como evidência de aquisição ou receita.

## Limites e validação

A estratégia é uma proposta para validação com clientes e experimentos. Não executa campanhas nem promete resultados clínicos ou comerciais. Não envie dados identificáveis de pacientes.

A estrutura da skill foi validada com o validador do Codex. A entrevista completa ainda precisa ser avaliada em usos reais; validação estrutural não comprova qualidade de todas as estratégias.

## Estrutura

```text
gtm-saude/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── entrevista.md
    ├── apify.md
    └── estrategia.md
```

Licença MIT.
