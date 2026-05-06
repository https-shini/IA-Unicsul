# Aula 02 — Exercícios: Histórico da IA e Sistemas Inteligentes

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

Em que ano e em qual evento a IA foi oficialmente reconhecida como campo de pesquisa?

**Resposta:**

Em **1956**, na **Conferência de Dartmouth**, organizada por John McCarthy, Marvin Minsky, Claude Shannon e Nathaniel Rochester. O termo "Inteligência Artificial" havia sido cunhado por McCarthy em **1955**.

---

### Questão 2

Quem é Alan Turing e por que ele é considerado o "pai da computação"?

**Resposta:**

**Alan Turing** foi um matemático britânico (1912–1954) que, em **1936**, formulou o conceito da **Máquina de Turing** — um modelo matemático que define o que é computável. Esse modelo se tornou a base teórica de todos os computadores modernos. Em **1950**, Turing publicou o artigo que estabeleceu as bases filosóficas e práticas da IA, propondo o famoso **Teste de Turing**.

---

### Questão 3

O que é a linguagem LISP e qual sua importância para a IA?

**Resposta:**

**LISP** (List Processing) é uma linguagem de programação criada por **John McCarthy em 1958**, fortemente associada ao desenvolvimento da IA simbólica. Sua importância vem de sua **flexibilidade na manipulação de símbolos e estruturas de dados**, características essenciais para representar conhecimento e raciocínio simbólico — abordagem dominante na IA das décadas de 1960 e 1970.

---

### Questão 4

O que era ELIZA e por que foi um marco?

**Resposta:**

**ELIZA**, criada em **1966** por Joseph Weizenbaum, foi um dos primeiros programas a simular um diálogo em linguagem natural, imitando um **psicoterapeuta**. Funcionava com **palavras-chave e respostas genéricas**, sem qualquer compreensão real. Sua importância está em ter mostrado que **interações simples podem parecer surpreendentemente humanas**, antecipando discussões sobre a relação entre simulação e compreensão genuína.

---

### Questão 5

Cite dois sistemas especialistas dos anos 1970 e suas aplicações.

**Resposta:**

- **MYCIN** — diagnóstico médico de infecções bacterianas, baseado em regras lógicas.
- **DENDRAL** — análise química de moléculas, ajudando na identificação de compostos desconhecidos.

---

## Nível Intermediário

### Questão 6

Explique em que consiste o **Teste de Turing**. Qual pergunta original ele substitui e por quê?

**Resposta:**

O **Teste de Turing** é uma proposta de Alan Turing (1950) para avaliar se uma máquina pode ser considerada inteligente.

**Estrutura:**

- Três participantes: um interrogador humano, um humano e uma máquina.
- A comunicação ocorre **apenas por texto**.
- O interrogador deve identificar quem é o humano e quem é a máquina.
- Se ele falhar consistentemente, considera-se que a máquina passou no teste.

**Pergunta substituída:**

Turing percebeu que a pergunta original — *"As máquinas podem pensar?"* — é filosoficamente vaga, pois depende de definições contestadas de "pensar". Ele a substituiu por uma pergunta **operacional**: *"Uma máquina pode imitar um humano de forma indistinguível?"*. Essa reformulação transforma um problema metafísico em um experimento empírico.

**Comentário didático:** o teste mede **comportamento observável**, não consciência. Essa escolha deliberada é justamente o alvo da crítica posterior de Searle.

---

### Questão 7

Diferencie **IA simbólica** e **IA conexionista** quanto à forma de representar e manipular o conhecimento.

**Resposta:**

| Característica | IA Simbólica | IA Conexionista |
|---|---|---|
| Representação do conhecimento | Símbolos explícitos e regras lógicas | Pesos e conexões em redes neurais |
| Forma de aprendizagem | Programada por especialistas | Aprendida automaticamente a partir de dados |
| Flexibilidade | Baixa — falha em situações imprevistas | Alta — adapta-se a ruído e variações |
| Interpretabilidade | Alta — regras são explícitas | Baixa — funcionamento opaco ("caixa preta") |
| Exemplos | Sistemas especialistas (MYCIN, DENDRAL) | Redes neurais profundas, deep learning |

**Comentário didático:** essas duas abordagens não são exclusivas. Pesquisas atuais em **IA neuro-simbólica** tentam combinar a interpretabilidade da simbólica com a adaptabilidade da conexionista.

---

### Questão 8

O que é um **agente inteligente** segundo a definição de Russell e Norvig? Dê um exemplo cotidiano (diferente dos citados em aula) e identifique seus sensores e atuadores.

**Resposta:**

Um **agente inteligente** é uma entidade que **percebe seu ambiente por meio de sensores** e **age sobre ele por meio de atuadores**, tomando decisões para alcançar objetivos.

**Exemplo cotidiano — Geladeira inteligente (smart fridge):**

- **Sensores:** câmera interna (identifica produtos), sensor de temperatura, sensor de porta aberta, leitor de código de barras, sensor de umidade.
- **Atuadores:** sistema de refrigeração, alarme sonoro (porta aberta), display interativo, módulo de comunicação Wi-Fi (envia notificações ao celular do usuário).
- **Objetivos:** manter os alimentos conservados, alertar sobre validade, sugerir reposição de itens em falta.

**Outros exemplos válidos:** drone de entrega, irrigador automático de jardim, semáforo inteligente, marcapasso adaptativo.

---

### Questão 9

Descreva o experimento mental da **Sala Chinesa** de John Searle. Qual crítica ele levanta ao Teste de Turing?

**Resposta:**

**Descrição do experimento:**

Imagine uma pessoa que **não fala chinês** trancada em uma sala. Ela recebe perguntas escritas em chinês por uma fenda na porta. Dentro da sala, há um **manual de instruções** em sua língua nativa que indica, para cada combinação de símbolos chineses recebidos, qual combinação de símbolos chineses produzir como resposta. Seguindo o manual mecanicamente, a pessoa devolve respostas perfeitas em chinês — mas **não compreende absolutamente nada** do conteúdo.

**Crítica de Searle:**

Para um observador externo, o sistema parece compreender chinês. Mas internamente, **só há manipulação de símbolos sem semântica**. Searle argumenta que:

- **Sintaxe ≠ Semântica.** Manipular símbolos corretamente não é o mesmo que entender seu significado.
- **Passar no Teste de Turing não prova consciência ou compreensão.** Uma máquina pode produzir respostas indistinguíveis das humanas sem ter qualquer experiência mental subjetiva.

**Comentário didático:** essa crítica permanece extremamente relevante na era dos LLMs. Modelos como GPT e Claude produzem texto coerente e contextual, mas o debate sobre se eles "compreendem" o que dizem é, em essência, uma reedição do argumento da Sala Chinesa.

---

### Questão 10

Apresente os **quatro tipos principais de agentes inteligentes** com um exemplo de cada.

**Resposta:**

| Tipo | Funcionamento | Exemplo |
|---|---|---|
| **Reflexivo simples** | Age com base apenas na percepção atual, seguindo regras `SE-ENTÃO`. | Termostato — liga/desliga conforme temperatura. |
| **Baseado em modelos** | Mantém representação interna do mundo; considera estados não diretamente observáveis. | Carro autônomo — antecipa movimento de outros veículos. |
| **Baseado em objetivos** | Define meta explícita e escolhe ações que reduzem a distância até ela. | GPS — calcula rota até o destino. |
| **Baseado em utilidade** | Compara estados quanto à sua "qualidade", maximizando função de utilidade. | Algoritmo de investimentos — pondera risco e retorno. |

---

### Questão 11

Considerando que um **carro autônomo** precisa tomar decisões rápidas, qual tipo de aprendizado é mais adequado para essa tarefa e por quê?

**Resposta:**

Carros autônomos utilizam uma **combinação de tipos de aprendizado**, com destaque para:

1. **Aprendizado supervisionado** para reconhecimento de objetos (placas, pedestres, veículos) a partir de imagens previamente rotuladas.
2. **Aprendizado por reforço** para a tomada de decisão em tempo real (frear, acelerar, mudar de faixa), aprendendo com simulações e experiências de direção que recompensam decisões seguras e penalizam colisões.
3. **Deep learning** como ferramenta transversal para visão computacional e fusão de dados de múltiplos sensores.

**Por que reforço é central:** dirigir é uma **sequência de decisões interdependentes** em um ambiente dinâmico — exatamente o tipo de problema em que recompensas acumuladas guiam o aprendizado de políticas ótimas. Modelos puramente supervisionados teriam dificuldade em lidar com situações novas e contínuas.

---

## Nível Avançado

### Questão 12

Compare dois períodos históricos da IA — **1950–1960** (otimismo inicial) e **2010–2020** (era do Deep Learning) — destacando características técnicas, conquistas e limitações de cada um.

**Resposta:**

| Aspecto | 1950–1960 (Otimismo Inicial) | 2010–2020 (Deep Learning) |
|---|---|---|
| **Paradigma dominante** | IA simbólica; manipulação de regras lógicas. | Redes neurais profundas com múltiplas camadas. |
| **Recursos computacionais** | Computadores extremamente limitados em memória e processamento. | GPUs poderosas e clusters em nuvem. |
| **Volume de dados** | Pequeno; coletado manualmente. | Massivo (Big Data) — internet, sensores, dispositivos móveis. |
| **Conquistas notáveis** | Primeiros programas de xadrez; provadores de teoremas; Teste de Turing. | AlexNet (2012) revoluciona visão computacional; AlphaGo (2016) derrota Lee Sedol no Go. |
| **Limitações** | Sistemas frágeis; falham em ambientes ruidosos; expectativas exageradas. | Modelos pouco interpretáveis ("caixa preta"); altos custos computacionais; dependência de grandes datasets. |
| **Visão prevalente** | Otimismo: IA geral em poucas décadas. | Pragmatismo: IA poderosa em domínios específicos. |

**Síntese:** a comparação evidencia que os avanços recentes não foram resultado de novas teorias matemáticas radicalmente diferentes — muitas técnicas de redes neurais existiam desde os anos 1980. A revolução veio da **convergência entre poder computacional, abundância de dados e refinamento algorítmico**.

---

### Questão 13

Qual a diferença entre um **agente baseado em objetivos** e um **agente baseado em utilidade**? Quando um seria preferível ao outro?

**Resposta:**

**Diferença conceitual:**

- O **agente baseado em objetivos** verifica apenas se uma ação leva ao **estado desejado**. Para ele, há essencialmente duas categorias: "atinge a meta" ou "não atinge".
- O **agente baseado em utilidade** vai além: atribui um **valor numérico** (utilidade) a cada estado possível, permitindo escolher entre múltiplos caminhos que satisfazem a meta, optando pelo que maximiza a utilidade.

**Quando preferir cada um:**

- Use **agente baseado em objetivos** quando o problema é **binário** ou tem uma única solução claramente desejada — por exemplo, um GPS calculando o trajeto até um endereço fixo.
- Use **agente baseado em utilidade** quando há **múltiplos objetivos competindo entre si** ou quando é necessário balancear trade-offs — por exemplo, um GPS que considera não só "chegar ao destino" mas também "minimizar tempo", "evitar pedágios", "preferir estradas mais seguras".

**Exemplo concreto:** um algoritmo de investimentos não pode se contentar com "obter lucro" (objetivo). Ele precisa **comparar carteiras** considerando lucro esperado vs. risco vs. liquidez — uma função de utilidade que pondera todas essas variáveis.

---

### Questão 14

A **definição contemporânea de agente** (Bornet et al., 2024) apresenta diferenças importantes em relação à definição clássica de Russell e Norvig (1995). Quais são essas diferenças e o que elas refletem sobre o estado atual da IA?

**Resposta:**

**Definição clássica (Russell & Norvig, 1995):**

Um agente é uma entidade que percebe o ambiente por sensores e age sobre ele por atuadores para atingir objetivos.

**Definição contemporânea (Bornet et al., 2024):**

Uma entidade digital **autônoma**, **orientada a objetivos**, capaz de executar tarefas de **múltiplos passos** de maneira **independente**, sem depender de comandos constantes de humanos.

**Principais diferenças:**

1. **Ênfase na autonomia prolongada** — a definição contemporânea destaca a capacidade de executar **fluxos completos** de trabalho, não apenas reagir a percepções imediatas.
2. **Multipassos e planejamento** — agentes modernos não apenas reagem; eles **planejam** sequências de ações, reavaliam, ajustam e retomam.
3. **Independência de supervisão constante** — não precisam de prompt humano a cada decisão; operam com objetivos de alto nível.
4. **Foco no digital** — a definição moderna se aplica explicitamente a agentes baseados em LLMs e softwares autônomos, refletindo a realidade tecnológica atual.

**O que isso reflete sobre a IA atual:**

- A passagem de **modelos reativos** (responder a um prompt) para **agentes proativos** (executar projetos completos).
- A maturidade dos **modelos fundacionais** como base capaz de raciocinar em alto nível.
- A integração crescente entre IA e ferramentas externas (uso de APIs, navegação web, execução de código), permitindo que sistemas resolvam problemas complexos do mundo real.
- Uma redefinição da **divisão de trabalho entre humano e máquina**: o humano define objetivos e supervisiona; o agente executa.

---

### Questão 15

Discuta criticamente: a Sala Chinesa de Searle invalida o Teste de Turing? Apresente argumentos a favor e contra.

**Resposta:**

**Argumentos a favor da crítica de Searle (a Sala Chinesa invalida o Teste de Turing):**

1. **Distinção entre simulação e compreensão:** o Teste de Turing avalia comportamento externo, mas comportamento externo pode ser produzido sem qualquer entendimento interno. Logo, passar no teste não prova inteligência genuína.
2. **Problema da consciência:** inteligência humana parece envolver experiência subjetiva (qualia, intencionalidade). O Teste de Turing ignora completamente essa dimensão.
3. **Aplicação aos LLMs atuais:** modelos modernos produzem texto altamente coerente sem evidência de compreensão real — exatamente o que Searle previu.

**Argumentos contra a crítica de Searle (o Teste de Turing permanece útil):**

1. **Resposta do "sistema":** Searle critica a pessoa dentro da sala, mas talvez seja o **sistema como um todo** (pessoa + manual + sala) que compreenda chinês. Reduzir a compreensão a um único componente pode ser uma falácia.
2. **Comportamentalismo prático:** se uma máquina age inteligentemente em todos os contextos relevantes, exigir mais do que isso pode ser uma demanda metafísica sem critério verificável.
3. **Problema simétrico para humanos:** não temos acesso direto à compreensão de outras pessoas — inferimos a partir de seu comportamento. Pelo mesmo critério, inferir compreensão de máquinas via comportamento seria justificável.
4. **Utilidade operacional:** mesmo que o teste não prove "compreensão", ele permanece útil como **benchmark prático** para avaliar capacidades conversacionais.

**Posição equilibrada:**

A Sala Chinesa **não invalida**, mas **redimensiona** o Teste de Turing. O teste é válido para avaliar **comportamento inteligente observável**, mas não responde questões metafísicas sobre **consciência ou compreensão**. Essas questões permanecem em aberto e provavelmente exigem novos critérios além dos puramente comportamentais — talvez envolvendo neurociência, teoria da informação integrada, ou abordagens ainda por desenvolver.

---

## Quadro-Síntese de Revisão

| Conceito | Definição em uma frase |
|---|---|
| **Teste de Turing** | Critério comportamental: máquina é inteligente se for indistinguível de um humano em diálogo. |
| **Sala Chinesa** | Crítica filosófica: simular respostas não é compreender. |
| **IA simbólica** | Conhecimento representado por símbolos e regras lógicas. |
| **IA conexionista** | Conhecimento representado por pesos em redes neurais. |
| **Conferência de Dartmouth** | Evento de 1956 que oficializou a IA como campo de pesquisa. |
| **Sistema especialista** | Sistema que codifica conhecimento de especialistas em regras (ex.: MYCIN, DENDRAL). |
| **Agente inteligente** | Entidade que percebe o ambiente, age sobre ele e busca objetivos. |
| **Agente reflexivo simples** | Age com base apenas na percepção atual (regras SE-ENTÃO). |
| **Agente baseado em modelos** | Mantém modelo interno do mundo. |
| **Agente baseado em objetivos** | Persegue um estado-meta explícito. |
| **Agente baseado em utilidade** | Maximiza função numérica de utilidade. |
| **Modelos fundacionais** | Grandes modelos pré-treinados (GPT, Claude, Gemini, Llama). |
