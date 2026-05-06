# Aula 01 — Exercícios: Introdução à IA e Machine Learning

> Banco de exercícios distribuído em três níveis de dificuldade, com respostas comentadas.

---

## Sumário

- [Nível Básico](#nível-básico)
- [Nível Intermediário](#nível-intermediário)
- [Nível Avançado](#nível-avançado)
- [Quadro-Síntese de Revisão](#quadro-síntese-de-revisão)

---

## Nível Básico

### Questão 1

Defina, com suas próprias palavras, o que é Inteligência Artificial.

**Resposta:**

Inteligência Artificial é a área da computação que desenvolve sistemas capazes de executar tarefas que normalmente exigiriam inteligência humana, como reconhecer padrões, analisar informações, aprender com a experiência e tomar decisões.

**Comentário didático:** o ponto-chave é a ideia de **simular capacidades cognitivas humanas em máquinas**. Não é necessário que a máquina "pense" como um humano — basta que produza resultados que, se viessem de um humano, seriam considerados inteligentes.

---

### Questão 2

Diferencie IA Forte de IA Fraca, indicando se cada uma já existe atualmente.

**Resposta:**

| Tipo | Definição | Existe hoje? |
|---|---|---|
| **IA Fraca** | Sistemas que executam tarefas específicas, sem compreensão geral. | Sim (assistentes virtuais, recomendação, classificadores). |
| **IA Forte** | Inteligência geral semelhante à humana, capaz de raciocinar em qualquer contexto. | Não — apenas hipotética. |

**Comentário didático:** essa distinção é frequentemente confundida em discussões públicas. Mesmo modelos avançados como o ChatGPT são considerados **IA Fraca**, pois operam em domínios delimitados (conversação, geração de texto), apesar de parecerem versáteis.

---

### Questão 3

Cite as quatro principais subáreas da Inteligência Artificial.

**Resposta:**

1. **Visão Computacional** — interpretação de imagens e vídeos.
2. **Processamento de Linguagem Natural (PLN)** — compreensão e geração de texto e voz.
3. **Robótica Inteligente** — IA aplicada a sistemas físicos.
4. **Aprendizado de Máquina (Machine Learning)** — algoritmos que aprendem com dados.

---

### Questão 4

Quais são os três pilares do Machine Learning?

**Resposta:**

1. **Dados** — base do aprendizado.
2. **Características (atributos / features)** — propriedades que descrevem os dados.
3. **Algoritmo** — método que aprende padrões e gera previsões.

---

### Questão 5

Cite três aplicações cotidianas de IA.

**Resposta (exemplos possíveis):**

- Recomendações em serviços de streaming (Netflix, Spotify).
- Filtro de spam de e-mail.
- Análise de trânsito em aplicativos de navegação (Google Maps, Waze).
- Filtros de rosto em redes sociais.
- Assistentes virtuais (Alexa, Google Assistant, Siri).

---

## Nível Intermediário

### Questão 6

Explique, com um exemplo cotidiano, a diferença entre **Inteligência Artificial** e **Aprendizado de Máquina**.

**Resposta:**

**Inteligência Artificial** é a área ampla que engloba todas as técnicas para fazer máquinas simularem inteligência humana. **Machine Learning** é uma **subárea da IA** focada em sistemas que aprendem a partir de dados, sem regras programadas explicitamente.

**Exemplo cotidiano — filtro de spam:**

- Um filtro **baseado em IA tradicional (não-ML)** poderia funcionar com regras fixas: "se o e-mail contém a palavra 'promoção', marque como spam".
- Um filtro **baseado em ML** analisa milhares de e-mails marcados como spam ou não-spam pelos usuários, aprende padrões (palavras-chave, remetentes, formatação) e melhora sua classificação ao longo do tempo, **sem que ninguém precise reprogramar suas regras**.

**Comentário didático:** todo ML é IA, mas nem toda IA é ML. Um sistema especialista baseado puramente em regras lógicas é IA, mas não é Machine Learning.

---

### Questão 7

Diferencie aprendizado supervisionado e não supervisionado, dando um exemplo de aplicação para cada.

**Resposta:**

| Característica | Supervisionado | Não Supervisionado |
|---|---|---|
| Dados de treino | Rotulados (com resposta correta) | Sem rótulos |
| Objetivo | Prever saída para novos dados | Descobrir padrões ocultos |
| Exemplo de aplicação | Classificação de e-mails (spam/não-spam) | Segmentação de clientes por comportamento de compra |

**Comentário didático:** uma forma simples de identificar o tipo é perguntar: *"Os dados de treino têm a resposta esperada junto?"*. Se sim, é supervisionado; se não, é não supervisionado.

---

### Questão 8

Por que a qualidade e a quantidade dos dados são fatores críticos para o sucesso de um modelo de Machine Learning?

**Resposta:**

Modelos de ML aprendem **padrões a partir de exemplos** — portanto, a qualidade do que aprendem depende diretamente da qualidade dos dados de treino. Existem quatro razões principais:

1. **Dados ruins geram modelos ruins** — o princípio "lixo entra, lixo sai" se aplica diretamente: erros, inconsistências e dados incompletos se traduzem em previsões pouco confiáveis.
2. **Quantidade insuficiente** impede que o modelo identifique padrões reais, levando-o a generalizar mal para novos casos.
3. **Falta de variedade** produz vieses: o modelo aprende apenas os padrões representados nos dados e falha em casos sub-representados.
4. **Dados representativos garantem justiça** — análises tornam-se mais confiáveis e equitativas para todos os grupos atingidos pelo sistema.

---

### Questão 9

Escolha uma situação do dia a dia e descreva como você aplicaria **aprendizado por reforço** nela.

**Resposta (exemplo):**

**Treinamento de um cachorro a sentar quando ouve "senta".**

- **Agente:** o cachorro.
- **Ambiente:** a sala onde o treino ocorre.
- **Ações possíveis:** sentar, ficar em pé, latir, deitar.
- **Recompensa:** petisco quando senta após o comando.
- **Punição:** ausência de recompensa (ou um "não" firme) quando faz outra ação.

Com repetições, o cachorro aprende a associar o comando "senta" + ação de sentar = recompensa, maximizando o comportamento desejado.

**Outro exemplo válido — robô aspirador aprendendo a navegar:** o robô recebe recompensa por cobrir áreas sujas e penalização por colidir com móveis; ao longo do tempo, otimiza seu trajeto.

---

### Questão 10

O que é **viés em IA** e como ele pode prejudicar uma decisão automatizada?

**Resposta:**

**Viés em IA** ocorre quando um sistema de aprendizado de máquina produz resultados sistematicamente desfavoráveis a determinados grupos, geralmente porque os dados de treino eram **inadequados, desbalanceados ou pouco representativos**.

**Exemplo concreto:** sistemas de reconhecimento facial treinados predominantemente com imagens de pessoas brancas apresentam taxas de erro significativamente maiores ao identificar pessoas negras. Se esse sistema for usado em segurança pública ou autenticação bancária, pode resultar em discriminação direta — falsas identificações, bloqueio injustificado de acesso, ou erros em investigações.

**Comentário didático:** o viés geralmente **não é intencional** — emerge do conjunto de dados. Por isso, mitigar viés exige diversificação dos dados, auditorias e transparência algorítmica.

---

### Questão 11

Descreva, em ordem, as etapas do pipeline de criação de um modelo de Machine Learning.

**Resposta:**

1. **Definição do problema** — identificar claramente o que se deseja resolver.
2. **Coleta de dados** — reunir informações relevantes.
3. **Limpeza e preparação** — tratar valores ausentes, remover inconsistências.
4. **Divisão dos dados** — separar em treino (≈70%) e teste (≈30%).
5. **Escolha do algoritmo** — selecionar a técnica adequada ao problema.
6. **Treinamento** — ajustar os parâmetros do modelo com os dados de treino.
7. **Avaliação** — medir o desempenho com os dados de teste.
8. **Otimização** — refinar o modelo com base nos resultados.

---

## Nível Avançado

### Questão 12

Imagine que você trabalha em uma empresa de e-commerce. Proponha uma solução de Machine Learning para melhorar as vendas e justifique qual tipo de aprendizado seria utilizado.

**Resposta:**

**Solução proposta — Sistema de recomendação personalizada de produtos.**

**Como funcionaria:**

- Coleta-se o histórico de navegação, compras, avaliações e tempo gasto em cada produto pelos usuários.
- O sistema identifica padrões de comportamento e similaridades entre usuários e entre produtos.
- A cada acesso, sugere itens com alta probabilidade de interesse para o usuário específico.

**Tipos de aprendizado envolvidos:**

- **Aprendizado não supervisionado** para a segmentação inicial — agrupar clientes com perfis similares (clustering), sem rótulos predefinidos.
- **Aprendizado supervisionado** para prever a probabilidade de um usuário comprar determinado produto, com base em dados históricos rotulados (comprou / não comprou).
- **Aprendizado por reforço** poderia ser incorporado posteriormente para otimizar a ordenação das recomendações com base em cliques e conversões reais.

**Justificativa:** a abordagem combinada permite **descobrir grupos de comportamento** (não supervisionado), **prever ações específicas** (supervisionado) e **adaptar continuamente** as recomendações conforme os usuários interagem (reforço).

---

### Questão 13

Por que um modelo de Machine Learning pode ter **ótimo desempenho nos dados de treino** e **péssimo desempenho nos dados de teste**?

**Resposta:**

Esse fenômeno é chamado de **overfitting** (sobreajuste). Ocorre quando o modelo **memoriza os dados de treino** em vez de **aprender padrões generalizáveis**. Causas comuns:

1. **Modelo excessivamente complexo** — captura ruído e particularidades irrelevantes do conjunto de treino.
2. **Conjunto de treino pequeno ou pouco diverso** — não representa adequadamente a variedade real dos dados.
3. **Treinamento prolongado em excesso** — o modelo se ajusta cada vez mais aos exemplos vistos, perdendo capacidade de generalização.
4. **Dados de teste com distribuição diferente** — o modelo nunca aprendeu a lidar com aquele tipo de exemplo.

**Analogia didática:** é como um estudante que decora as respostas de uma lista específica de exercícios em vez de entender a matéria. Vai bem nos exercícios decorados, mas falha em qualquer prova com questões diferentes.

**Mitigação:** divisão treino/validação/teste, regularização, redução da complexidade do modelo, aumento dos dados, validação cruzada.

---

### Questão 14

Disserte sobre a frase: *"A Inteligência Artificial não substituirá médicos, mas médicos que usam IA substituirão os que não usam."*

**Resposta (modelo de dissertação):**

A frase sintetiza uma visão pragmática sobre a relação entre IA e profissões intelectuais. Ela propõe que o vetor de transformação do trabalho **não é a substituição direta** do humano pela máquina, mas sim a **mudança no perfil profissional exigido**.

A IA já demonstra capacidade de auxiliar a medicina em tarefas específicas: análise de exames de imagem com precisão equivalente ou superior à de especialistas, descoberta acelerada de medicamentos, sugestão de diagnósticos diferenciais e personalização de tratamentos. Porém, a prática médica envolve elementos que ainda escapam à IA — empatia, julgamento ético, comunicação com pacientes vulneráveis, decisões em contextos ambíguos com escassez de dados.

O profissional que **integra IA ao seu fluxo de trabalho** ganha vantagens significativas: maior precisão em diagnósticos, mais tempo para o cuidado humanizado, capacidade de lidar com volumes maiores de informação. Já o profissional que **se recusa a adotar essas ferramentas** torna-se progressivamente menos competitivo, não porque a IA o substitua, mas porque concorrentes humanos potencializados por IA o superam.

A lição se estende a outras áreas: advogados que usam IA para análise de jurisprudência, programadores que usam IA para acelerar codificação, designers que a usam para prototipagem rápida. **A IA redefine não o "se" trabalhamos, mas o "como" trabalhamos** — exigindo qualificação contínua e disposição para integrar novas ferramentas ao ofício.

---

### Questão 15

Por que sistemas de reconhecimento facial podem falhar com determinados grupos étnicos? Explique o problema e sugira formas de mitigá-lo.

**Resposta:**

**Origem do problema:**

Os sistemas de reconhecimento facial são treinados em conjuntos de imagens. Se o conjunto de treino é dominado por pessoas de um grupo étnico específico (tipicamente brancos, em sistemas desenvolvidos no hemisfério norte), o modelo aprende a reconhecer com alta precisão as características desse grupo, mas **falha em generalizar** para grupos sub-representados.

**Mecanismo técnico:**

- Pessoas com tons de pele mais escuros têm **menos contraste facial** em condições típicas de iluminação dos datasets.
- Modelos otimizados em dados desbalanceados aprendem a priorizar características presentes na maioria.
- Avaliações de desempenho geralmente são feitas em conjuntos igualmente desbalanceados, mascarando o problema.

**Consequências sociais:**

- Falsas identificações em sistemas de segurança pública.
- Bloqueios injustos em autenticação bancária ou desbloqueio de dispositivos.
- Reforço de desigualdades estruturais já existentes.

**Estratégias de mitigação:**

1. **Diversificação dos dados de treino** — coletar imagens representativas de todos os grupos demográficos.
2. **Auditorias regulares** — avaliar o desempenho separadamente para cada grupo, não apenas no conjunto agregado.
3. **Transparência algorítmica** — divulgar limitações conhecidas dos sistemas.
4. **Regulação e supervisão** — exigir testes de equidade antes da implantação em contextos sensíveis.
5. **Equipes diversas** — desenvolvedores de origens variadas tendem a identificar mais cedo os pontos cegos do sistema.

---

## Quadro-Síntese de Revisão

| Conceito | Definição em uma frase |
|---|---|
| **IA** | Área da computação que cria sistemas capazes de simular inteligência humana. |
| **ML** | Subárea da IA em que sistemas aprendem padrões a partir de dados. |
| **IA Forte / IA Fraca** | Inteligência geral hipotética / inteligência específica existente. |
| **Aprendizado supervisionado** | Aprende com dados rotulados (entrada + resposta). |
| **Aprendizado não supervisionado** | Descobre padrões em dados sem rótulos. |
| **Aprendizado por reforço** | Aprende por tentativa e erro, com recompensas e punições. |
| **Deep Learning** | ML baseado em redes neurais profundas com múltiplas camadas. |
| **Viés em IA** | Resultado sistematicamente injusto causado por dados desbalanceados. |
| **Overfitting** | Modelo que memoriza o treino e generaliza mal para novos dados. |
| **Pipeline de ML** | Definição → coleta → limpeza → divisão → treino → avaliação → otimização. |
