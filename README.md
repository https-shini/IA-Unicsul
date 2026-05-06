<h1 align="center">🤖 Fundamentos de Inteligência Artificial</h1>

<p align="center">
  <a href="#-sobre-a-disciplina">Sobre</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-conteúdo-programático">Conteúdo</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-aulas-e-materiais">Aulas</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-avisos-do-professor">Avisos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-licença">Licença</a>
</p>

## 📖 Sobre a disciplina
A disciplina **Fundamentos de Inteligência Artificial** apresenta os conceitos essenciais que estruturam o campo da IA, desde sua origem histórica e filosófica até as abordagens modernas de aprendizado e representação do conhecimento. O objetivo é capacitar o aluno a compreender, comparar e aplicar os principais paradigmas da IA — simbólico, conexionista e híbrido — relacionando teoria com casos de uso reais e implicações éticas do uso dessas tecnologias.

### 🎯 Objetivos de aprendizagem
- **Cognitivos:** compreender os fundamentos teóricos e históricos da Inteligência Artificial, suas abordagens e paradigmas de aprendizado.
- **Habilidades:** analisar, comparar e selecionar técnicas de IA adequadas para diferentes classes de problemas.
- **Atitudes:** refletir criticamente sobre o impacto da IA na sociedade, no mercado de trabalho e nas questões éticas envolvidas.

**Professor:** Edidio Rubens Dantas Lima <br>
**Curso:** Ciência da Computação – Universidade Cruzeiro do Sul

---

## 📚 Conteúdo programático
1. **Unidades 1 a 3**
   - Introdução à Inteligência Artificial: definição, IA Fraca vs. IA Forte
   - Histórico da IA: das origens filosóficas ao Deep Learning e modelos generativos
   - Abordagens da IA: Simbólica, Conexionista e Híbrida (Neuro-Simbólica)

2. **Unidades 4 a 6**
   - Sistema de Símbolos Físicos (HSSF) e Teste de Turing
   - Resolução de Problemas por Busca: BFS, DFS, UCS, Busca Gulosa e A*
   - Aprendizado de Máquina supervisionado: classificação e regressão

3. **Unidades 7 a 10**
   - Aprendizado Não Supervisionado: K-Means, PCA, detecção de anomalias
   - Aprendizado por Reforço: Q-Learning, Equação de Bellman, Deep Q-Learning
   - Representação e Processamento do Conhecimento: lógica, regras, redes neurais, lógica fuzzy
   - IA no dia a dia e implicações éticas: privacidade, viés e responsabilidade algorítmica

---

## 📊 Aulas e Materiais

### 📝 Aula 01 — Introdução à Inteligência Artificial
A **Aula 01** apresentou a definição de Inteligência Artificial como o campo da computação dedicado a sistemas que realizam tarefas normalmente associadas à cognição humana. Foi explorada a distinção entre **IA Fraca (Estreita)**, que opera em domínios específicos, e **IA Forte (Geral)**, ainda um objetivo de pesquisa. O impacto da IA em setores como saúde, educação e transporte foi contextualizado com exemplos do cotidiano, e o **Aprendizado de Máquina (ML)** foi introduzido como o mecanismo pelo qual sistemas aprimoram seu desempenho a partir de dados.

👉 [Acessar Conteudo: Aula01_Introducao_IA](Aula01_Introducao_IA.pdf)

### 📝 Aula 02 — Histórico da Inteligência Artificial
A **Aula 02** percorreu a evolução histórica da IA, desde as reflexões filosóficas de **Descartes** e **Diderot** sobre autômatos e linguagem, passando pelo **Teste de Turing (1950)** e pela **Conferência de Dartmouth (1956)** — marco fundador do campo. Foram abordados os períodos da IA Simbólica (programas como ELIZA e sistemas especialistas), a crise do simbolismo e o surgimento do Conexionismo nos anos 1980, a era do Deep Learning com AlexNet e AlphaGo, até os modelos fundacionais generativos e generalistas da atualidade.

👉 [Acessar Conteudo: Aula02_Historico_IA](Aula02_Historico_IA.pdf)

### 📝 Aula 03 — Abordagens da IA: Simbólica e Conexionista
A **Aula 03** aprofundou as duas grandes tradições da IA. A **IA Simbólica** representa o conhecimento via símbolos e regras lógicas, sendo interpretável e transparente, mas rígida e com dificuldade em lidar com incerteza e grandes volumes de dados. A **IA Conexionista** inspira-se no cérebro humano, aprendendo a partir de dados por meio de redes neurais com ajuste de pesos, sendo poderosa para reconhecimento de padrões, porém com baixa explicabilidade. As **abordagens híbridas neuro-simbólicas**, como IBM Watson e AlphaGo, foram apresentadas como a tendência atual de combinar o melhor dos dois paradigmas.

👉 [Acessar Conteudo: Aula03_Abordagens_IA](Aula03_Abordagens_IA.pdf)

### 📝 Aula 04 — Sistema de Símbolos Físicos e Teste de Turing
A **Aula 04** detalhou a **Hipótese do Sistema de Símbolos Físicos (HSSF)**, proposta por Newell e Simon, segundo a qual a inteligência emerge da manipulação de símbolos físicos — independentemente de substrato biológico. Em contraponto, foi estudado o **Teste de Turing** em profundidade, com seu critério operacional de indistinguibilidade comportamental entre máquina e humano, incluindo a crítica da **Sala Chinesa** de John Searle (1980), que argumenta que simular compreensão não equivale a compreender de fato.

👉 [Acessar Conteudo: Aula04_Sistema_Simbolos_Teste_Turing](Aula04_Sistema_Simbolos_Teste_Turing.pdf)

### 📝 Aula 05 — Resolução de Problemas por Busca
A **Aula 05** introduziu a formulação formal de problemas em IA: estado inicial, ações (operadores), modelo de transição, teste de objetivo e custo de caminho. Foram estudados os algoritmos de **Busca Sem Informação** — BFS (garante menor número de passos, custo de memória alto), DFS (baixo consumo de memória, sem garantia de otimalidade) e UCS (menor custo acumulado via fila de prioridade) — e os algoritmos de **Busca Com Informação**, com destaque para a **Busca Gulosa** e o **A\***, cuja função `f(n) = g(n) + h(n)` garante completude e otimalidade quando a heurística é admissível e consistente.

👉 [Acessar Conteudo: Aula05_Busca_Resolucao_Problemas](Aula05_Busca_Resolucao_Problemas.pdf)

### 📝 Aula 06 — IA e Programação
A **Aula 06** abordou a interface entre Inteligência Artificial e programação de computadores, explorando como conceitos e técnicas de IA são implementados na prática por meio de linguagens e paradigmas de programação. O conteúdo estabeleceu a ponte entre os fundamentos teóricos das aulas anteriores e a construção concreta de sistemas inteligentes.

👉 [Acessar Conteudo: Aula06_IA_Programacao](Aula06_IA_Programacao.pdf)

### 📝 Aula 07 — Introdução ao Aprendizado de Máquina
A **Aula 07** introduziu formalmente o **Aprendizado de Máquina (ML)** como subárea da IA, apresentando sua definição, motivação e os três paradigmas principais: **supervisionado** (dados rotulados, tarefas de classificação e regressão), **não supervisionado** (dados sem rótulos, descoberta de padrões) e **por reforço** (aprendizado por tentativa e erro com maximização de recompensa). Foram discutidos os critérios para escolha do paradigma mais adequado conforme a natureza do problema e dos dados disponíveis.

👉 [Acessar Conteudo: Aula07_AM_Introducao](Aula07_AM_Introducao.pdf)

### 📝 Aula 08 — Aprendizado Não Supervisionado e por Reforço
A **Aula 08** cobriu dois paradigmas complementares do Aprendizado de Máquina. No **Aprendizado Não Supervisionado**, foram apresentadas técnicas como **K-Means** (clusterização), **PCA** (redução de dimensionalidade e combate à maldição da dimensionalidade), regras de associação e detecção de anomalias — todas aplicadas a dados sem rótulos. No **Aprendizado por Reforço**, o ciclo agente-ambiente foi formalizado com o dilema exploração vs. explotação, e os algoritmos **Q-Learning** (com Tabela Q e Equação de Bellman) e **Deep Q-Learning (DQN)** foram estudados como base para aplicações em jogos, robótica e veículos autônomos.

👉 [Acessar Conteudo: Aula08_AM_Nao_Supervisionada_Reforco](Aula08_AM_Nao_Supervisionada_Reforco.pdf)

### 📝 Aula 09 — Aprendizado de Máquina: Árvores de Decisão e Teorema de Bayes
A **Aula 09** aprofundou técnicas de aprendizado supervisionado com foco em dois modelos fundamentais. As **Árvores de Decisão** foram apresentadas como estruturas hierárquicas que particionam os dados com base em atributos, permitindo classificação e regressão de forma interpretável e transparente. O **Teorema de Bayes** foi introduzido como fundamento probabilístico para classificação, com destaque para o **Classificador Naive Bayes**, que assume independência condicional entre atributos e é amplamente utilizado em filtragem de spam e análise de texto.

👉 [Acessar Conteudo: Aula09_AM_Arvores_Bayes](Aula09_AM_Arvores_Bayes.pdf)

### 📝 Aula 10 — Representação e Processamento do Conhecimento
A **Aula 10** apresentou as principais formas de codificar conhecimento para sistemas computacionais. Foram comparados a **Lógica Proposicional** e a **Lógica de Predicados** (com quantificadores ∀ e ∃), as **Regras de Produção SE-ENTÃO** usadas em sistemas especialistas com encadeamento para frente e para trás, as **Redes Neurais Artificiais** com aprendizado via **backpropagation**, e a **Lógica Fuzzy**, que modela graus de verdade para raciocinar sobre conceitos vagos e imprecisos. A aula encerrou o conteúdo programático conectando os diferentes paradigmas de representação com os contextos de aplicação mais adequados a cada um.

👉 [Acessar Conteudo: Aula10_Representacao_Conhecimento](Aula10_Representacao_Conhecimento.pdf)

### 📝 Aula 11 — Avaliação A2
A **Aula 11** é destinada à realização da **Avaliação A2** da disciplina. Não haverá exposição de conteúdo novo nesta data. Consulte a seção de [Avisos do Professor](#-avisos-do-professor) para informações completas sobre as instruções e regras da prova.

---

## 📢 Avisos do Professor

### 🗓️ Avaliação A2 — Instruções Oficiais

> Comunicado emitido pelo **Prof. Edidio Rubens Dantas Lima** aos alunos da disciplina.

As instruções a seguir devem ser lidas com atenção e cumpridas integralmente no dia da avaliação:

1. A prova terá início às **19h10**, com tolerância de entrada até as **19h30**. Após esse horário, não será permitida a entrada de nenhum aluno.
2. É obrigatório o uso de **caneta azul ou preta**.
3. O aluno deverá **assinar a lista de chamada** ao ingressar na sala.
4. **Aparelhos eletrônicos** (celular e similares) devem permanecer dentro da mochila, e a mochila deve ser mantida **no chão** durante toda a avaliação.
5. A saída da sala será permitida a partir das **19h40**.
6. Ao concluir a prova, o aluno deverá **entregá-la ao professor** e permanecer em seu local até que a saída seja sinalizada.
7. O **visto de prova** ocorrerá na semana seguinte à realização da avaliação. Alunos ausentes poderão realizar a prova nessa mesma data, **somente mediante apresentação de justificativa de falta**.
8. No **dia do visto de prova** não haverá aula regular — a data é destinada exclusivamente ao visto e à aplicação da prova para os alunos faltantes.
9. O **entendimento das perguntas** da avaliação faz parte da avaliação. Leia cada questão com atenção antes de responder.
10. A duração total da prova é de **1 hora**.

---

## 📄 Licença

Distribuído sob a **Licença MIT**. Veja o arquivo `LICENSE` para mais informações.

---

> *Este repositório registra de forma organizada as aulas, sínteses e materiais desenvolvidos na disciplina de Fundamentos de Inteligência Artificial, servindo como referência de estudo e consulta ao longo do curso.*
