# Aula 08 — Aprendizado de Máquina Não Supervisionado e por Reforço

> Material de estudo estruturado a partir do conteúdo da aula, organizado para consulta, revisão e aprofundamento.

---

## Sumário

1. [Revisão: Tipos de Aprendizado de Máquina](#1-revisão-tipos-de-aprendizado-de-máquina)
2. [Aprendizado Não Supervisionado: Conceitos Fundamentais](#2-aprendizado-não-supervisionado-conceitos-fundamentais)
3. [Clustering (Agrupamento)](#3-clustering-agrupamento)
4. [Algoritmo K-Means](#4-algoritmo-k-means)
5. [Algoritmo DBSCAN](#5-algoritmo-dbscan)
6. [Hierarchical Clustering (Agrupamento Hierárquico)](#6-hierarchical-clustering-agrupamento-hierárquico)
7. [Métricas de Avaliação para Clustering](#7-métricas-de-avaliação-para-clustering)
8. [Redução de Dimensionalidade](#8-redução-de-dimensionalidade)
9. [Análise de Componentes Principais (PCA)](#9-análise-de-componentes-principais-pca)
10. [t-SNE (t-Distributed Stochastic Neighbor Embedding)](#10-t-sne-t-distributed-stochastic-neighbor-embedding)
11. [Detecção de Anomalias](#11-detecção-de-anomalias)
12. [Aprendizado por Reforço: Conceitos Fundamentais](#12-aprendizado-por-reforço-conceitos-fundamentais)
13. [O Problema do Agente-Ambiente](#13-o-problema-do-agente-ambiente)
14. [Elementos do Aprendizado por Reforço](#14-elementos-do-aprendizado-por-reforço)
15. [Tipos de Aprendizado por Reforço](#15-tipos-de-aprendizado-por-reforço)
16. [Algoritmo Q-Learning](#16-algoritmo-q-learning)
17. [Deep Reinforcement Learning (DRL)](#17-deep-reinforcement-learning-drl)
18. [Aplicações do Aprendizado por Reforço](#18-aplicações-do-aprendizado-por-reforço)

---

## 1. Revisão: Tipos de Aprendizado de Máquina

Conforme abordado na Aula 07, o Aprendizado de Máquina (ML) é dividido em três paradigmas principais [6]:

-   **Aprendizado Supervisionado**: Aprende com dados rotulados (entrada-saída).
-   **Aprendizado Não Supervisionado**: Descobre padrões em dados sem rótulos.
-   **Aprendizado por Reforço**: Aprende por tentativa e erro em um ambiente para maximizar recompensas.

Esta aula se aprofundará nos dois últimos tipos: Não Supervisionado e por Reforço.

## 2. Aprendizado Não Supervisionado: Conceitos Fundamentais

No Aprendizado Não Supervisionado, o algoritmo recebe um conjunto de dados **sem rótulos** (apenas entradas). O objetivo é encontrar padrões, estruturas ou relações ocultas nos dados por conta própria, sem orientação externa [6].

### 2.1. Objetivo

Descobrir a estrutura intrínseca dos dados, como agrupamentos, anomalias ou reduções de dimensionalidade. É útil para exploração de dados, pré-processamento e quando a rotulagem é inviável ou muito cara [6].

### 2.2. Principais Tarefas

-   **Clustering (Agrupamento)**: Agrupar dados semelhantes.
-   **Redução de Dimensionalidade**: Simplificar dados complexos.
-   **Detecção de Anomalias**: Identificar pontos de dados incomuns.

## 3. Clustering (Agrupamento)

Clustering é a tarefa de agrupar um conjunto de objetos de forma que objetos no mesmo grupo (cluster) sejam mais semelhantes entre si do que para aqueles em outros grupos. Não há rótulos pré-definidos; o algoritmo descobre os grupos [6].

### 3.1. Aplicações

-   Segmentação de clientes (marketing).
-   Análise de documentos (agrupar notícias por tópico).
-   Biologia (classificação de espécies).
-   Detecção de comunidades em redes sociais.

## 4. Algoritmo K-Means

### 4.1. Conceito

O K-Means é um dos algoritmos de clustering mais populares e simples. Ele particiona os dados em `k` clusters, onde `k` é um número predefinido pelo usuário [6].

### 4.2. Funcionamento

1.  **Inicialização**: Escolhe `k` centróides aleatoriamente nos dados.
2.  **Atribuição**: Cada ponto de dados é atribuído ao centróide mais próximo.
3.  **Atualização**: Os centróides são recalculados como a média de todos os pontos de dados atribuídos a eles.
4.  **Repetição**: Os passos 2 e 3 são repetidos até que os centróides não mudem significativamente ou um número máximo de iterações seja atingido.

### 4.3. Vantagens e Desvantagens

-   **Vantagens**: Simples, rápido, eficiente para grandes conjuntos de dados.
-   **Desvantagens**: Requer que `k` seja especificado previamente, sensível à inicialização dos centróides, assume clusters esféricos e de tamanho similar, sensível a outliers [6].

## 5. Algoritmo DBSCAN

### 5.1. Conceito

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) é um algoritmo de clustering baseado em densidade. Ele agrupa pontos que estão próximos uns dos outros, marcando como outliers os pontos que estão em regiões de baixa densidade [6].

### 5.2. Funcionamento

Requer dois parâmetros:

-   `epsilon (eps)`: O raio máximo para considerar um ponto como vizinho.
-   `min_samples`: O número mínimo de pontos dentro de `eps` para formar um cluster.

Classifica os pontos em:

-   **Core Point**: Tem pelo menos `min_samples` pontos (incluindo ele mesmo) dentro de `eps`.
-   **Border Point**: Está dentro do `eps` de um Core Point, mas não é um Core Point por si só.
-   **Noise Point**: Não é um Core Point nem um Border Point.

### 5.3. Vantagens e Desvantagens

-   **Vantagens**: Não requer `k` predefinido, pode encontrar clusters de formas arbitrárias, robusto a outliers.
-   **Desvantagens**: Sensível aos parâmetros `eps` e `min_samples`, dificuldade em lidar com clusters de densidades variadas [6].

## 6. Hierarchical Clustering (Agrupamento Hierárquico)

### 6.1. Conceito

Cria uma hierarquia de clusters, que pode ser visualizada como um dendrograma. Não requer que o número de clusters seja especificado previamente [6].

### 6.2. Tipos

-   **Aglomerativo (Bottom-Up)**: Começa com cada ponto como um cluster individual e os une progressivamente até formar um único cluster.
-   **Divisivo (Top-Down)**: Começa com todos os pontos em um único cluster e os divide recursivamente até que cada ponto seja um cluster individual.

### 6.3. Vantagens e Desvantagens

-   **Vantagens**: Não requer `k` predefinido, produz uma estrutura hierárquica que pode ser útil para análise, visualização clara via dendrograma.
-   **Desvantagens**: Computacionalmente caro para grandes conjuntos de dados, uma vez que um ponto é unido a um cluster, não pode ser desfeito [6].

## 7. Métricas de Avaliação para Clustering

Avaliar a qualidade de um clustering é mais desafiador do que em aprendizado supervisionado, pois não há rótulos verdadeiros. Métricas comuns incluem [6]:

-   **Silhouette Score**: Mede o quão semelhante um objeto é ao seu próprio cluster em comparação com outros clusters. Varia de -1 (máximo erro) a +1 (cluster bem separado).
-   **Davies-Bouldin Index**: Mede a similaridade média entre cada cluster e seu cluster mais semelhante. Valores menores indicam melhor agrupamento.
-   **Inertia (Soma dos Quadrados Dentro do Cluster)**: Usada no K-Means, mede a soma das distâncias quadráticas dos pontos ao centróide de seu cluster. Valores menores indicam clusters mais compactos.

## 8. Redução de Dimensionalidade

Redução de dimensionalidade é o processo de reduzir o número de variáveis aleatórias consideradas, ou seja, o número de features, através da obtenção de um conjunto de variáveis principais [6].

### 8.1. Objetivos

-   **Visualização**: Facilitar a visualização de dados de alta dimensão.
-   **Redução de Ruído**: Remover features irrelevantes ou redundantes.
-   **Melhora de Performance**: Acelerar algoritmos de ML e reduzir o risco de overfitting (maldição da dimensionalidade).

## 9. Análise de Componentes Principais (PCA)

### 9.1. Conceito

PCA (Principal Component Analysis) é uma técnica linear de redução de dimensionalidade que transforma os dados em um novo sistema de coordenadas, onde as novas dimensões (componentes principais) são ortogonais e capturam a maior parte da variância dos dados [6].

### 9.2. Funcionamento

1.  Calcula a matriz de covariância dos dados.
2.  Calcula os autovalores e autovetores da matriz de covariância.
3.  Os autovetores correspondem às direções dos componentes principais, e os autovalores indicam a quantidade de variância explicada por cada componente.
4.  Seleciona os `k` autovetores com os maiores autovalores para formar as novas `k` dimensões.

### 9.3. Vantagens e Desvantagens

-   **Vantagens**: Simples, eficaz para remover correlação entre features, útil para visualização e pré-processamento.
-   **Desvantagens**: Linear (não captura relações não lineares), os componentes são difíceis de interpretar, sensível à escala dos dados [6].

## 10. t-SNE (t-Distributed Stochastic Neighbor Embedding)

### 10.1. Conceito

t-SNE é uma técnica não linear de redução de dimensionalidade, particularmente adequada para visualização de dados de alta dimensão em um espaço de 2 ou 3 dimensões. Ela tenta preservar a estrutura local dos dados, ou seja, pontos que estão próximos no espaço de alta dimensão permanecem próximos no espaço de baixa dimensão [6].

### 10.2. Vantagens e Desvantagens

-   **Vantagens**: Excelente para visualização de clusters em dados complexos, captura relações não lineares.
-   **Desvantagens**: Computacionalmente caro para grandes conjuntos de dados, sensível aos parâmetros, não é para redução de dimensionalidade para alimentar outros modelos (apenas visualização) [6].

## 11. Detecção de Anomalias

Detecção de anomalias é a tarefa de identificar itens, eventos ou observações que não se conformam a um padrão esperado em um conjunto de dados. Essas anomalias são frequentemente chamadas de outliers [6].

### 11.1. Aplicações

-   Detecção de fraude (transações financeiras, seguros).
-   Detecção de intrusão em redes de computadores.
-   Monitoramento de saúde de equipamentos.
-   Diagnóstico médico (anomalias em exames).

### 11.2. Técnicas Comuns

-   **Baseadas em Densidade**: DBSCAN (pontos de ruído), Local Outlier Factor (LOF).
-   **Baseadas em Distância**: K-Nearest Neighbors (KNN).
-   **Baseadas em Modelos**: One-Class SVM, Isolation Forest.

## 12. Aprendizado por Reforço: Conceitos Fundamentais

No Aprendizado por Reforço (RL), um **agente** aprende a tomar decisões sequenciais em um **ambiente** para maximizar uma **recompensa** acumulada. O agente aprende por **tentativa e erro**, recebendo feedback (recompensa ou punição) após cada ação [6].

### 12.1. Diferença do Supervisionado e Não Supervisionado

-   **Supervisionado**: Aprende com um "professor" que dá a resposta correta.
-   **Não Supervisionado**: Encontra estrutura sem feedback explícito.
-   **Reforço**: Aprende com feedback atrasado (recompensa) sobre a qualidade de uma sequência de ações, não de uma única ação [6].

## 13. O Problema do Agente-Ambiente

O RL é modelado como um **Processo de Decisão de Markov (MDP)**, que envolve [6]:

-   **Agente**: O tomador de decisões.
-   **Ambiente**: O mundo com o qual o agente interage.
-   **Estado (S)**: A situação atual do ambiente.
-   **Ação (A)**: O que o agente pode fazer.
-   **Recompensa (R)**: Feedback numérico imediato.
-   **Política (π)**: A estratégia do agente, mapeando estados para ações.
-   **Função de Valor (V ou Q)**: Estima a recompensa futura esperada de um estado ou de uma ação em um estado.

O objetivo do agente é aprender uma **política ótima** que maximize a recompensa total esperada a longo prazo [6].

## 14. Elementos do Aprendizado por Reforço

-   **Política**: Mapeia estados para ações. Pode ser determinística (uma ação para cada estado) ou estocástica (probabilidade de ações).
-   **Função de Recompensa**: Define o objetivo do problema. É o feedback imediato do ambiente.
-   **Função de Valor**: Previsão da recompensa futura acumulada a partir de um estado ou de uma ação em um estado. Ajuda o agente a escolher ações que levam a recompensas maiores a longo prazo.
-   **Modelo do Ambiente (Opcional)**: Uma representação do ambiente que o agente pode usar para prever o que acontecerá a seguir (próximo estado e recompensa) se ele tomar uma determinada ação [6].

## 15. Tipos de Aprendizado por Reforço

-   **Model-Based RL**: O agente tenta aprender um modelo do ambiente (como o ambiente funciona) e usa esse modelo para planejar ações.
-   **Model-Free RL**: O agente aprende a política ótima ou a função de valor diretamente da experiência, sem construir um modelo explícito do ambiente. É mais comum e flexível [6].

## 16. Algoritmo Q-Learning

### 16.1. Conceito

Q-Learning é um algoritmo de Aprendizado por Reforço **model-free** e **off-policy**. Ele aprende uma **função Q** (Q-value) que estima o valor esperado de tomar uma ação `a` em um estado `s` e, subsequentemente, seguir a política ótima [6].

### 16.2. Funcionamento

O Q-value para um par (estado, ação) é atualizado iterativamente usando a equação de Bellman:

`Q(s, a) ← Q(s, a) + α [R + γ max Q(s', a') - Q(s, a)]`

-   `Q(s, a)`: Valor Q atual para o estado `s` e ação `a`.
-   `α (alpha)`: Taxa de aprendizado (quão rápido o agente incorpora novas informações).
-   `R`: Recompensa imediata recebida.
-   `γ (gamma)`: Fator de desconto (importância das recompensas futuras).
-   `max Q(s', a')`: O valor Q máximo do próximo estado `s'` para todas as ações `a'` possíveis.

### 16.3. Exploração vs. Explotação

Um desafio central no RL é o dilema **exploração-explotação** [6]:

-   **Exploração**: O agente tenta novas ações para descobrir recompensas potencialmente maiores.
-   **Explotação**: O agente escolhe as ações que já sabe que maximizam a recompensa.

Estratégias como `epsilon-greedy` (onde o agente explora com probabilidade `epsilon` e explota com `1-epsilon`) são usadas para balancear esses dois aspectos.

## 17. Deep Reinforcement Learning (DRL)

### 17.1. Conceito

DRL combina Aprendizado por Reforço com **Deep Learning**. Redes neurais profundas são usadas para aproximar as funções de valor ou as políticas, permitindo que o RL lide com espaços de estados e ações muito grandes ou contínuos [6].

### 17.2. Marcos

-   **Deep Q-Networks (DQN)**: Google DeepMind usou DQN para jogar jogos de Atari com desempenho super-humano (2013).
-   **AlphaGo**: Combinou DRL com busca em árvore para derrotar campeões mundiais de Go (2016).

## 18. Aplicações do Aprendizado por Reforço

-   **Jogos**: Xadrez, Go, videogames (AlphaGo, AlphaZero).
-   **Robótica**: Controle de robôs, navegação, manipulação de objetos.
-   **Veículos Autônomos**: Tomada de decisão em cenários de tráfego.
-   **Finanças**: Otimização de portfólios de investimento, estratégias de trading.
-   **Sistemas de Recomendação**: Otimização de recomendações para maximizar o engajamento do usuário a longo prazo.
-   **Gerenciamento de Recursos**: Otimização de consumo de energia em data centers.
