# Síntese: Fundamentos de Inteligência Artificial

## 1. Introdução à Inteligência Artificial

A **Inteligência Artificial (IA)** é um campo da ciência da computação que se dedica à criação de sistemas capazes de realizar tarefas que normalmente exigiriam inteligência humana, como analisar informações, aprender com experiências, resolver problemas e tomar decisões [1]. A IA busca simular e, em alguns casos, superar a capacidade cognitiva humana, permitindo que máquinas aprimorem seu desempenho sem programação direta, através do **Aprendizado de Máquina (ML)** [1].

O impacto da IA é vasto e crescente, revolucionando setores como saúde, indústria, educação e transporte. Exemplos cotidianos incluem o uso de IA no Google Maps para otimização de rotas, filtros inteligentes de imagem em redes sociais e sistemas de recomendação personalizados em plataformas de streaming [1].

### IA Forte vs. IA Fraca

Uma distinção fundamental na IA é entre **IA Fraca (ou Estreita)** e **IA Forte (ou Geral)** [1] [2].

| Característica       | IA Fraca (Estreita)                                                               | IA Forte (Geral)                                                                                                 |
| :------------------- | :-------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------- |
| **Definição**        | Realiza tarefas específicas sem compreender contextos complexos ou raciocínio avançado. | Busca criar máquinas com inteligência semelhante à humana, capazes de aprender e raciocinar em múltiplos contextos. |
| **Exemplos**         | Assistentes virtuais, sistemas de recomendação, reconhecimento facial.            | Atualmente não existe, é um objetivo de pesquisa.                                                                |
| **Compreensão**      | Não possui compreensão real ou consciência.                                      | Teria compreensão e consciência.                                                                                 |

## 2. Histórico da IA

A história da IA é marcada por questionamentos filosóficos e avanços tecnológicos significativos [2].

*   **Origens Filosóficas**: Pensadores como **René Descartes** (século XVII) já diferenciavam humanos de autômatos pela capacidade de adaptar a linguagem, e **Denis Diderot** (século XVIII) antecipou a ideia de que a capacidade de responder a tudo seria um critério de inteligência [2].
*   **Alan Turing e o Teste de Turing (1950)**: Considerado o pai da computação, Alan Turing propôs o "Jogo da Imitação" (Teste de Turing) para avaliar se uma máquina poderia exibir comportamento inteligente indistinguível do humano. Em vez de perguntar "As máquinas podem pensar?", Turing buscou um critério operacional: "Há como imaginar um computador digital que faria bem o jogo da imitação?" [1] [2]. Se um interrogador não consegue distinguir a máquina de um humano através de conversas textuais, a máquina é considerada inteligente. O teste não exige respostas corretas, mas sim respostas *humanas*, incluindo hesitações e erros [2].
*   **Conferência de Dartmouth (1956)**: Este evento marcou o início formal da IA como campo de pesquisa, onde o termo "Inteligência Artificial" foi cunhado por John McCarthy [1] [2].
*   **Primeiros Avanços (1950-1960)**: Surgiram os primeiros programas de xadrez e sistemas de prova de teoremas, impulsionando o otimismo na área [2].
*   **IA Simbólica (1960-1980)**: Abordagem dominante que utilizava símbolos e regras lógicas para representar conhecimento e realizar tarefas inteligentes. Exemplos incluem o programa ELIZA (1966), que simulava um psicoterapeuta, e sistemas especialistas como MYCIN e DENDRAL [2].
*   **Crise do Simbólico e Conexionismo (1980)**: A IA simbólica mostrou limitações em lidar com informações complexas e incerteza, levando ao surgimento do **Conexionismo**, que se inspira na estrutura do cérebro humano e utiliza redes neurais [2]. A "Sala Chinesa" de John Searle (1980) criticou o Teste de Turing, argumentando que simular compreensão não implica compreensão real [2].
*   **Expansão com ML (2000-2010)**: Agentes passaram a aprender a partir de dados, utilizando modelos probabilísticos e técnicas estatísticas [2].
*   **Era do Deep Learning (2010-2020)**: Redes neurais profundas revolucionaram áreas como visão computacional e Processamento de Linguagem Natural (PLN), com marcos como o AlexNet (reconhecimento de imagens em 2012) e o AlphaGo (que derrotou campeões mundiais de Go em 2016) [2].
*   **Presente: Agentes Generativos e Generalistas (2020+)**: Modelos fundacionais como ChatGPT, Claude e Gemini são capazes de múltiplas tarefas, criação de textos, imagens e código, e colaboram com humanos [2].

## 3. Abordagens da IA: Simbólica e Conexionista

As duas principais tradições da IA são a simbólica e a conexionista, cada uma com princípios, benefícios e limitações distintos [3].

### IA Simbólica

*   **Definição**: O conhecimento é representado por símbolos (palavras, frases, conceitos) organizados em estruturas lógicas. O sistema manipula esses símbolos para resolver problemas, raciocinar e tomar decisões [3].
*   **Origens**: Pesquisa ativa desde a década de 1950, dominou o campo por mais de 50 anos [3].
*   **Hipótese do Sistema de Símbolos Físicos (HSSF)**: Proposta por Newell e Simon, afirma que um sistema inteligente pode ser construído manipulando símbolos físicos que representam conhecimento. A inteligência, nessa visão, não depende de biologia, mas da arquitetura correta de processamento de símbolos [3] [4].
*   **Benefícios**: Interpretabilidade (símbolos e regras compreensíveis), raciocínio lógico, tomada de decisão transparente e manejo de incerteza [3].
*   **Limitações**: Dificuldade em formalizar conhecimento do mundo real (problema da formalização), explosão combinatória de regras, alto custo e tempo na aquisição de conhecimento de especialistas ("gargalo do conhecimento"), dificuldade com incerteza e ambiguidade, e incapacidade de aprender com dados sem reprogramação [3] [4].

### IA Conexionista

*   **Definição**: Sistemas inspirados na estrutura do cérebro humano, constituídos por redes de unidades conectadas (neurônios artificiais) que se comunicam através de sinapses artificiais (pesos) [3].
*   **Origens**: Ganhou destaque a partir dos anos 1980, sinergicamente com o surgimento de computadores mais potentes e a capacidade de processar grandes volumes de dados [3].
*   **Aprendizado**: O conhecimento não é programado, mas aprendido. O sistema é alimentado com dados, e algoritmos ajustam os pesos das conexões para que a rede reconheça padrões e faça previsões [3].
*   **Aplicações**: Problemas onde o conhecimento não é bem estruturado ou é difícil de representar com símbolos, como visão computacional, processamento de linguagem natural, reconhecimento de voz e diagnóstico por imagem [3].
*   **Benefícios**: Aprendizado adaptativo, processamento paralelo, generalização (aplica a situações novas), adaptação a mudanças e excelente reconhecimento de padrões [3].
*   **Limitações**: "Caixa-preta" (difícil explicar decisões), requerimento de grandes conjuntos de dados, treinamento demorado e custo computacional elevado [3].

### Tabela Comparativa: Simbólica vs. Conexionista

| Critério           | IA Simbólica                                  | IA Conexionista                                                              |
| :----------------- | :-------------------------------------------- | :--------------------------------------------------------------------------- |
| **Representação**  | Símbolos e regras                             | Pesos e conexões                                                             |
| **Conhecimento**   | Programado explicitamente                     | Aprendido de dados                                                           |
| **Interpretação**  | Fácil (transparente)                          | Difícil ("caixa-preta")                                                    |
| **Aprendizado**    | Não aprende sozinha                           | Aprende com exemplos                                                         |
| **Domínio Típico** | Problemas lógicos                             | Padrões complexos                                                            |
| **Dados**          | Poucos (conhecimento)                         | Muitos (exemplos)                                                            |

### Abordagens Híbridas

A tendência atual é combinar o melhor dos dois mundos, criando sistemas **neuro-simbólicos** que utilizam redes neurais para percepção e padrões, e símbolos e regras para raciocínio e explicação, resultando em IA mais robusta, interpretável e capaz [3]. Exemplos incluem IBM Watson (combina PLN conexionista com regras simbólicas) e AlphaGo (aprendizado por reforço com redes neurais) [3].

## 4. Resolução de Problemas por Busca

Em IA, "resolver um problema" significa encontrar uma sequência de ações que leve do estado inicial ao estado objetivo [5].

### Definição Formal do Problema

Um problema é definido por [5]:

*   **Estado Inicial**: O ponto de partida.
*   **Ações (Operadores)**: As operações possíveis que mudam o estado.
*   **Modelo de Transição**: O resultado de aplicar uma ação a um estado.
*   **Teste de Objetivo**: Como saber se o objetivo foi alcançado.
*   **Custo de Caminho**: O custo associado à sequência de ações.

O **Espaço de Estados** é o conjunto de todas as configurações possíveis do problema, e a **Árvore de Busca** representa as possibilidades de caminho a partir do estado inicial [5].

### Classificação das Buscas

As buscas são classificadas em [5]:

*   **Busca Sem Informação (Cega)**: O agente não tem conhecimento prévio sobre qual caminho é melhor, explorando as possibilidades de forma sistemática.
*   **Busca Com Informação (Heurística)**: O agente utiliza uma função heurística (um "palpite educado") para estimar o custo do nó atual até o objetivo, guiando a busca de forma mais eficiente.

### Critérios de Avaliação de Busca

Os algoritmos de busca são avaliados por [5]:

*   **Completude**: Se encontra uma solução caso ela exista.
*   **Otimização**: Se encontra a melhor solução (menor custo/caminho mais curto).
*   **Complexidade de Tempo**: Quanto tempo leva para encontrar a solução.
*   **Complexidade de Espaço**: Quanta memória consome.

### Algoritmos de Busca Sem Informação

*   **Busca em Largura (BFS - Breadth-First Search)**: Explora todos os nós de um nível antes de passar para o próximo. Garante o caminho mais curto (ótimo) em termos de número de passos, mas consome muita memória (usa Fila - FIFO) [5].
*   **Busca em Profundidade (DFS - Depth-First Search)**: Explora um caminho até o fim antes de retroceder e tentar outras ramificações. Consome pouca memória (usa Pilha - LIFO), mas não garante o caminho mais curto e pode ficar preso em ciclos [5].
*   **Busca de Custo Uniforme (UCS - Uniform Cost Search)**: Uma variação do BFS que expande o nó com o menor custo acumulado até o momento. Garante o menor custo total, usando uma Fila de Prioridade [5].

### Algoritmos de Busca Com Informação

*   **Busca Gulosa (Best-First Search)**: Expande o nó que parece mais próximo do objetivo (menor valor da função heurística `h(n)`). É rápida, mas não garante a otimização e pode ser enganada por obstáculos locais [5].
*   **Busca A* (A-Star)**: O algoritmo de busca informada mais famoso. Utiliza a função `f(n) = g(n) + h(n)`, onde `g(n)` é o custo real do início até o nó `n`, e `h(n)` é a estimativa heurística do custo de `n` até o objetivo. Se a heurística for admissível (nunca superestima o custo real) e consistente, o A* é completo e ótimo [5].

### Desafios

O principal desafio é a **explosão combinatória**, onde o número de possibilidades cresce exponencialmente, tornando a busca exaustiva inviável. Nesses casos, heurísticas fortes e algoritmos otimizados são essenciais [5].

## 5. Aprendizado de Máquina

O Aprendizado de Máquina (ML) é uma subárea da IA que permite que sistemas aprendam a partir de dados, sem serem explicitamente programados [1]. Existem três paradigmas principais [1] [6]:

### 5.1. Aprendizado Supervisionado

Neste paradigma, o modelo aprende a partir de **dados rotulados**, ou seja, pares de entrada e saída desejada. O objetivo é mapear entradas para saídas, fazendo previsões ou classificações precisas [1].

*   **Classificação**: Prever categorias discretas (ex: e-mail é spam ou não) [1].
*   **Regressão**: Estimar valores numéricos contínuos (ex: preço de um imóvel) [1].

### 5.2. Aprendizado Não Supervisionado

O aprendizado não supervisionado lida com **dados sem rótulos**, buscando descobrir padrões, estruturas ocultas ou relações nos dados [1] [6]. É útil quando rotular dados é caro, lento ou inviável [6].

*   **Clusterização (Agrupamento)**: Agrupar dados semelhantes em clusters, onde elementos dentro do mesmo grupo são mais parecidos entre si do que com os de outros grupos. O algoritmo **K-Means** é um exemplo clássico [6].
*   **Associação**: Descobrir itens que aparecem juntos com frequência (ex: regras do tipo "se-então" em cestas de compras) [6].
*   **Redução de Dimensionalidade**: Simplificar dados com muitas variáveis, reduzindo o número de dimensões enquanto mantém a informação mais relevante. A **Análise de Componentes Principais (PCA)** é uma técnica comum que ajuda a combater a "maldição da dimensionalidade" (dados esparsos em altas dimensões) [6].
*   **Detecção de Anomalias**: Identificar pontos que fogem drasticamente do padrão esperado (ex: fraudes em cartões) [6].

### 5.3. Aprendizado por Reforço

Neste paradigma, um **agente** aprende por **tentativa e erro** em um **ambiente**, buscando maximizar uma **recompensa** ao longo do tempo [1] [6].

*   **Elementos Fundamentais**: Agente, ambiente, estado, ação e recompensa [6].
*   **Ciclo Agente-Ambiente**: O agente observa o estado, escolhe uma ação, o ambiente muda de estado e retorna uma recompensa, e o agente atualiza seu conhecimento [6].
*   **Dilema Exploração vs. Explotação**: O agente precisa equilibrar a exploração de novas ações (que podem levar a recompensas maiores) com a explotação de ações conhecidas (que já se mostraram eficazes) [6].
*   **Q-Learning**: Um algoritmo que aprende a "qualidade" de cada ação em um determinado estado, utilizando uma **Tabela Q** e a **Equação de Bellman** para atualizar o conhecimento do agente sobre recompensas futuras [6].
*   **Deep Q-Learning (DQN)**: Combina Q-Learning com redes neurais profundas para lidar com espaços de estados muito grandes, onde uma Tabela Q tradicional seria inviável [6].
*   **Aplicações**: Jogos (AlphaGo), robótica, carros autônomos [1] [6].

## 6. Representação e Processamento do Conhecimento

A representação do conhecimento é a forma como as informações sobre o mundo são codificadas para que um sistema computacional possa raciocinar, exigindo expressividade, eficiência e legibilidade [7].

### Paradigmas Principais

*   **Lógica Proposicional**: Trabalha com proposições (sentenças verdadeiras ou falsas) e conectivos lógicos (e, ou, não, se-então). É limitada por não expressar quantificadores ou propriedades internas de objetos [7].
*   **Lógica de Predicados**: Estende a lógica proposicional com predicados (propriedades/relações) e quantificadores (universal ∀, existencial ∃), permitindo maior expressividade [7].
*   **Regras de Produção**: Formato "SE <condição> ENTÃO <ação>", usadas em sistemas especialistas. Podem ser encadeadas para frente (dos fatos às conclusões) ou para trás (da meta aos fatos necessários) [7].
*   **Sistemas Especialistas**: Programas que simulam o raciocínio de um especialista humano em um domínio restrito, compostos por uma base de conhecimento (regras), um motor de inferência e uma interface. Vantagens incluem consistência e disponibilidade, mas têm desvantagens na aquisição de conhecimento e falta de aprendizado autônomo [7].
*   **Redes Neurais Artificiais**: Inspiradas no cérebro biológico, utilizam neurônios artificiais conectados em camadas. Aprendem por ajuste de pesos (treinamento) através de algoritmos como o **backpropagation**, que minimiza o erro entre a saída desejada e a obtida [7].
*   **Lógica Fuzzy**: Lida com graus de verdade (entre 0 e 1), sendo útil para conceitos vagos como "alto" ou "quente". Permite raciocinar com imprecisão, ao contrário da lógica clássica binária [7].

### Tabela Resumo das Técnicas de Representação

| Técnica             | Base                   | Aprendizado | Explicabilidade |
| :------------------ | :--------------------- | :---------- | :-------------- |
| **Lógica**          | Símbolos               | Não         | Alta            |
| **Regras SE-ENTÃO** | Regras heurísticas     | Não         | Alta            |
| **Redes Neurais**   | Pesos (conexões)       | Sim         | Baixa           |
| **Lógica Fuzzy**    | Graus de verdade       | Não         | Média           |

## 7. IA no Dia a Dia e Implicações Éticas

A IA já está profundamente integrada ao cotidiano e continua a transformar diversos setores [1].

*   **Aplicações Práticas**: Recomendações personalizadas, filtros de imagem, análise de trânsito, assistentes virtuais, drones agrícolas para detecção de pragas, sensores para solo e clima, análise de raio-X na saúde, descoberta acelerada de medicamentos e tratamentos personalizados [1].
*   **Futuro do Trabalho**: A automação de tarefas rotineiras por IAs pode tornar alguns cargos obsoletos, mas também cria novas profissões (treinadores de IA, auditores de algoritmos). A adaptação e o desenvolvimento de novas habilidades são essenciais [1].
*   **Ética em IA**: Questões cruciais incluem a **privacidade dos dados** (que alimentam os modelos de IA), a **transparência algorítmica** (compreender como os algoritmos tomam decisões) e a **responsabilidade em erros** (definir quem é responsável por falhas da IA). O **viés em IA**, originado de dados de treinamento inadequados ou desbalanceados, pode reforçar desigualdades e levar a decisões injustas, exigindo transparência, auditorias e dados diversificados para ser minimizado [1].

## Referências

[1] Aula01_Introducao_IA.pdf
[2] Aula02_Historico_IA.pdf
[3] Aula03_Abordagens_IA.pdf
[4] Aula04_Sistema_Simbolos_Teste_Turing.pdf
[5] Aula05_Busca_Resolucao_Problemas.pdf
[6] Aula08_AM_Nao_Supervisionada_Reforco.pdf
[7] Aula10_Representacao.pdf
