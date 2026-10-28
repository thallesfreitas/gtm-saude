# GTM Saúde

Skill para construir uma estratégia de go-to-market de negócios de saúde no Brasil por uma entrevista didática, com uma pergunta por vez.

Não exige site nem briefing pronto. Parte da descrição do empreendedor, ajuda a esclarecer decisões e combina as respostas com pesquisa de mercado.

## Instalar no Codex

Envie esta mensagem ao Codex:

```text
Use $skill-installer para instalar:
https://github.com/thallesfreitas/gtm-saude/tree/main/gtm-saude
```

## Instalar no Claude

A pasta `gtm-saude/` segue o formato de skill do Claude (`SKILL.md` + `references/`), então funciona sem adaptação. O arquivo `agents/openai.yaml` é só do Codex e é ignorado.

### Claude Code (terminal)

Com um comando:

```bash
npx skills add thallesfreitas/gtm-saude
```

Quando perguntar em quais agentes instalar, escolha Claude Code.

Ou manualmente, sem instalador:

```bash
git clone --depth 1 https://github.com/thallesfreitas/gtm-saude /tmp/gtm-saude && \
mkdir -p ~/.claude/skills && cp -r /tmp/gtm-saude/gtm-saude ~/.claude/skills/
```

Abra uma sessão nova e invoque com `/gtm-saude`.

### App do Claude (web e desktop)

Não precisa usar terminal, Git ou gerar um arquivo compactado:

1. [Baixe o ZIP pronto da versão v1.0.0](https://github.com/thallesfreitas/gtm-saude/releases/download/v1.0.0/gtm-saude.zip). Outras versões ficam em [Releases](https://github.com/thallesfreitas/gtm-saude/releases).
2. Confirme que execução de código e criação de arquivos estão ativadas em **Settings > Capabilities** (a opção pode aparecer como **Create and edit files**).
3. Vá em **Customize > Skills**, clique em **+**, depois **Create skill** e **Upload a skill**.
4. Envie o arquivo `gtm-saude.zip` que baixou e ative a skill.

O ZIP já contém a pasta `gtm-saude/` com `SKILL.md` e as referências. Escolha o arquivo anexado à Release, não o “Source code (zip)” automático do GitHub, que contém o repositório inteiro.

Skills instaladas no app também aparecem no Claude Code quando você entra com a mesma conta. O contrário não acontece: o que é instalado só no Claude Code não vai para o app.

## Começar

No Codex:

```text
Use $gtm-saude para construir a estratégia do meu negócio.
```

No Claude, peça em linguagem natural:

```text
Use a skill gtm-saude para construir a estratégia do meu negócio.
```

A primeira pergunta é sobre o negócio. As seguintes se adaptam às respostas: problema, público, jornada, preço, alternativas, recursos e objetivo. Você pode responder “não sei”; a skill ajuda a formular hipóteses sem tratá-las como fatos.

Se já tiver um briefing, envie-o junto. Site e documentos são opcionais.

## Exemplo de entrevista completa

Este diálogo é fictício e usa uma plataforma de cuidados paliativos para ilustrar todos os assuntos da entrevista. Valores, capacidade e metas abaixo são respostas de exemplo, não dados de um negócio real nem recomendações clínicas.

**A skill faz uma pergunta por vez e espera a resposta.** Aqui mostramos a conversa inteira para você entender o percurso. Na prática, a ordem muda conforme as respostas, perguntas já respondidas são puladas e aprofundamentos podem ser necessários.

### 1. O negócio

**Skill:** Qual é o seu negócio? Conte o que você oferece e para quem, do jeito que explicaria a alguém que acabou de conhecer.

**Você:** Uma plataforma de cuidados paliativos principalmente remota, com abrangência nacional, criada por uma médica paliativista. Queremos apoiar pacientes com doenças graves e suas famílias.

### 2. A jornada

**Skill:** Como uma família começa a usar o serviço e o que acontece depois, do primeiro contato ao acompanhamento?

**Você:** Começa por uma triagem, depois há uma consulta médica para entender as necessidades. A família pode contratar um plano mensal renovável de baixa, média ou alta intensidade, de acordo com o apoio necessário.

### 3. O estágio do negócio

**Skill:** Esse serviço já atende clientes ou ainda está sendo criado?

**Você:** Estamos estruturando o piloto. A médica já tem experiência clínica, mas ainda não vendemos os planos da plataforma.

### 4. O problema que leva à procura

**Skill:** O que costuma acontecer para uma família procurar esse tipo de ajuda?

**Você:** A família fica angustiada com uma doença grave, não sabe por onde começar e precisa organizar o cuidado e o apoio a quem cuida. Queremos validar se esse é o principal motivo de contratação.

### 5. Quem usa, decide e paga

**Skill:** Quem recebe o cuidado, quem escolhe o serviço e quem paga? Podem ser pessoas diferentes.

**Você:** O paciente recebe o cuidado junto com seus cuidadores. Nossa hipótese é que um filho adulto participe da escolha e a família pague. Isso ainda precisa ser confirmado em entrevistas.

### 6. O primeiro público e o território

**Skill:** Entre as pessoas que você pretende atender, quem faz sentido alcançar primeiro e onde consegue entregar o serviço?

**Você:** Queremos começar com famílias de pacientes com câncer que já tenham acompanhamento presencial. O atendimento remoto pode ser nacional, mas nossa rede presencial inicial estará apenas em São Paulo; não podemos prometer cobertura presencial no país todo.

### 7. O que está incluído

**Skill:** O que a família recebe no plano e o que fica de fora?

**Você:** Pretendemos oferecer acompanhamento de paliativista, psicologia, enfermagem, fonoaudiologia, espiritualidade e orientação a cuidadores, conforme o plano. Também queremos organizar apoio ao luto e encaminhamento jurídico. Procedimentos presenciais e atendimento de emergência não estão incluídos. Frequência e disponibilidade de cada profissional ainda precisam ser definidas.

### 8. Preço e cobrança

**Skill:** Quanto você cobra ou pensa cobrar, e como seria feita a cobrança?

**Você:** Pensamos em mensalidades entre R$ 2 mil e R$ 6 mil, dependendo da intensidade. É uma estimativa; ainda precisamos calcular os custos da equipe e validar a disposição de pagar.

**Skill:** Vou registrar essa faixa como hipótese de preço, não como valor validado. O custo da equipe e o escopo de cada plano precisam entrar na decisão.

### 9. As alternativas atuais

**Skill:** Como essas famílias resolvem o problema hoje, antes de conhecer sua solução?

**Você:** Imaginamos que recorram ao SUS, a consultas particulares separadas, ao WhatsApp do médico e ao apoio da própria família. Precisamos perguntar como isso funciona de verdade e quais dificuldades permanecem.

### 10. O motivo para escolher sua oferta

**Skill:** Por que uma família trocaria o que faz hoje pelo seu serviço?

**Você:** Nossa hipótese é que ter o acompanhamento organizado por uma equipe e apoio aos cuidadores reduza a dificuldade de coordenar tudo sozinha. Ainda não temos entrevistas ou resultados que comprovem essa preferência.

### 11. Como os clientes chegam

**Skill:** Como chegaram os clientes que você já tem ou, se ainda não tem, quais caminhos pretende testar?

**Você:** Ainda não temos clientes da plataforma. Queremos testar indicação de médicos, como hematologistas, geriatras e neurologistas, e usar o WhatsApp para atender os interessados. No futuro, pensamos em operadoras e seguradoras.

### 12. Dinheiro e tempo disponíveis

**Skill:** Quanto dinheiro e tempo consegue dedicar a conquistar clientes no próximo mês?

**Você:** Podemos reservar R$ 1.500 para os testes e seis horas por semana da fundadora. Não temos uma pessoa dedicada a vendas. Gastos com ferramentas de pesquisa precisam ser combinados separadamente.

### 13. Capacidade de entrega

**Skill:** Quantos novos clientes consegue receber sem prejudicar a entrega?

**Você:** Nossa estimativa inicial é de até cinco famílias, mas isso depende da intensidade de cada plano e da disponibilidade da equipe. Precisamos confirmar a capacidade antes de ampliar a divulgação.

### 14. O objetivo

**Skill:** O que gostaria de alcançar com esse primeiro ciclo e em quanto tempo?

**Você:** Em 30 dias, queremos conversar com dez famílias qualificadas e tentar contratar duas para o piloto. São metas de aprendizagem, não uma previsão de vendas.

### 15. Síntese antes da estratégia

**Skill:** Entendi que vocês estão montando um piloto, com atendimento remoto e uma rede presencial inicial limitada a São Paulo. A família é a provável pagadora, o preço ainda é hipótese e a capacidade estimada é de cinco famílias. O objetivo é testar demanda e contratação com R$ 1.500 e seis horas semanais. O escopo dos planos e os custos da equipe ainda estão abertos. O que você gostaria de corrigir ou acrescentar antes de eu montar a estratégia?

**Você:** Está correto. Pode avançar, mantendo preço, capacidade e perfil de quem decide como hipóteses a validar.

### E se eu não souber responder?

**Você:** Não sei quem decide a contratação.

**Skill:** Tudo bem. Isso ajuda a escolher com quem conversar e como apresentar a oferta. Nas situações que você conhece, quem costuma procurar ajuda primeiro?

A conversa continua a partir da resposta. A skill não precisa que você saiba termos de marketing, tenha um site ou preencha um formulário antes de começar.

### O que acontece depois?

A skill pesquisa concorrentes e alternativas, verifica as fontes disponíveis e constrói os sete blocos da estratégia. Quando o Apify estiver disponível e houver orçamento autorizado, ele entra como pesquisa complementar da comunicação pública dos concorrentes.

Ao final, você recebe a estratégia, o GTM em uma página, os três testes de 30 dias e a sequência de primeiras ações. As lacunas ficam identificadas; propostas não são apresentadas como resultados já alcançados.

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

No Claude, use a mesma frase sem o `$` ("Use a skill gtm-saude..."). Para usar o Apify no Claude, o conector do Apify precisa estar ligado na conversa.

Aceita menos perfis que o limite quando só houver poucos pertinentes e confirmados. Seguidores e curtidas não são tratados como evidência de aquisição ou receita.

## Limites e validação

A estratégia é uma proposta para validação com clientes e experimentos. Não executa campanhas nem promete resultados clínicos ou comerciais. Não envie dados identificáveis de pacientes.

A estrutura da skill foi validada com o validador do Codex. A entrevista completa ainda precisa ser avaliada em usos reais; validação estrutural não comprova qualidade de todas as estratégias.

## Estrutura

```text
gtm-saude/
├── SKILL.md
├── agents/openai.yaml   (só Codex)
└── references/
    ├── entrevista.md
    ├── apify.md
    └── estrategia.md
```

Licença MIT.
