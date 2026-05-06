# Aula 07 — Introdução ao Aprendizado de Máquina

> Material de estudo estruturado a partir do conteúdo da aula, organizado para consulta, revisão e aprofundamento.

---

## Sumário

1. [O que é Aprendizado de Máquina?](#1-o-que-é-aprendizado-de-máquina)
2. [Definição Formal de Aprendizado de Máquina](#2-definição-formal-de-aprendizado-de-máquina)
3. [Tipos de Aprendizado de Máquina](#3-tipos-de-aprendizado-de-máquina)
4. [Aprendizado Supervisionado](#4-aprendizado-supervisionado)
5. [Aprendizado Não Supervisionado](#5-aprendizado-não-supervisionado)
6. [Aprendizado por Reforço](#6-aprendizado-por-reforço)
7. [O Processo de Desenvolvimento de um Modelo de ML (Pipeline)](#7-o-processo-de-desenvolvimento-de-um-modelo-de-ml-pipeline)
8. [Importância da Qualidade dos Dados](#8-importância-da-qualidade-dos-dados)
9. [Overfitting e Underfitting](#9-overfitting-e-underfitting)
10. [Métricas de Avaliação (Classificação)](#10-métricas-de-avaliação-classificação)
11. [Métricas de Avaliação (Regressão)](#11-métricas-de-avaliação-regressão)
12. [Aplicações do Aprendizado de Máquina](#12-aplicações-do-aprendizado-de-máquina)

---

## 1. O que é Aprendizado de Máquina?

**Aprendizado de Máquina (Machine Learning - ML)** é uma subárea da Inteligência Artificial que permite a sistemas de computador **aprenderem a partir de dados**, identificarem padrões, tomarem decisões e melhorarem seu desempenho ao longo do tempo, **sem serem explicitamente programados** para cada tarefa específica [6].

Em vez de seguir um conjunto fixo de regras, um algoritmo de ML constrói um modelo a partir de dados de treinamento, que então pode ser usado para fazer previsões ou tomar decisões sobre novos dados [6].

## 2. Definição Formal de Aprendizado de Máquina

Arthur Samuel (1959) definiu o aprendizado de máquina como o "campo de estudo que dá aos computadores a capacidade de aprender sem serem explicitamente programados" [6].

Tom Mitchell (1997) forneceu uma definição mais formal: "Um programa de computador aprende com a experiência `E` com respeito a alguma classe de tarefas `T` e medida de desempenho `P`, se seu desempenho em `T`, medido por `P`, melhora com a experiência `E`" [6].

-   **Tarefa (T)**: A tarefa que o sistema deve realizar (ex: classificar e-mails como spam ou não spam).
-   **Experiência (E)**: Os dados de treinamento que o sistema utiliza para aprender (ex: um conjunto de e-mails rotulados como spam ou não spam).
-   **Medida de Desempenho (P)**: A métrica usada para avaliar o quão bem o sistema está realizando a tarefa (ex: a porcentagem de e-mails classificados corretamente).

## 3. Tipos de Aprendizado de Máquina

O Aprendizado de Máquina é geralmente categorizado em três tipos principais, baseados na natureza da "experiência" (dados de treinamento) e no objetivo do aprendizado [6]:

1.  **Aprendizado Supervisionado**
2.  **Aprendizado Não Supervisionado**
3.  **Aprendizado por Reforço**

## 4. Aprendizado Supervisionado

### 4.1. Conceito

No Aprendizado Supervisionado, o algoritmo é treinado com um conjunto de dados que inclui tanto as **entradas (features)** quanto as **saídas desejadas (rótulos/labels)**. É como aprender com um professor que fornece as respostas corretas para cada exemplo [6].

### 4.2. Objetivo

O objetivo é aprender um mapeamento entre as entradas e as saídas, de modo que o modelo possa prever a saída correta para novos dados não vistos [6].

### 4.3. Tipos de Problemas

-   **Classificação**: A saída é uma categoria discreta (ex: spam/não-spam, gato/cachorro, doença/não-doença). Algoritmos comuns: Regressão Logística, Máquinas de Vetores de Suporte (SVM), Árvores de Decisão, Random Forest, Redes Neurais [6].
-   **Regressão**: A saída é um valor numérico contínuo (ex: preço de uma casa, temperatura, vendas futuras). Algoritmos comuns: Regressão Linear, Regressão Polinomial, Árvores de Decisão para Regressão, Redes Neurais [6].

### 4.4. Exemplos de Aplicação

-   Detecção de spam em e-mails.
-   Reconhecimento facial.
-   Previsão de preços de imóveis.
-   Diagnóstico médico (classificar se um paciente tem uma doença).

## 5. Aprendizado Não Supervisionado

### 5.1. Conceito

No Aprendizado Não Supervisionado, o algoritmo recebe um conjunto de dados **sem rótulos** (apenas entradas). O objetivo é encontrar padrões, estruturas ou relações ocultas nos dados por conta própria, sem orientação externa [6].

### 5.2. Objetivo

Descobrir a estrutura intrínseca dos dados, como agrupamentos, anomalias ou reduções de dimensionalidade [6].

### 5.3. Tipos de Problemas

-   **Agrupamento (Clustering)**: Agrupar dados semelhantes em clusters (ex: segmentação de clientes). Algoritmos comuns: K-Means, DBSCAN, Hierarchical Clustering [6].
-   **Associação**: Descobrir regras que descrevem grandes porções dos dados (ex: "quem compra X também compra Y"). Algoritmos comuns: Apriori [6].
-   **Redução de Dimensionalidade**: Reduzir o número de features mantendo a maior parte da informação (ex: PCA - Análise de Componentes Principais). Algoritmos comuns: PCA, t-SNE [6].
-   **Detecção de Anomalias**: Identificar pontos de dados que se desviam significativamente do padrão normal (ex: detecção de fraude). Algoritmos comuns: Isolation Forest, One-Class SVM [6].

### 5.4. Exemplos de Aplicação

-   Segmentação de mercado.
-   Detecção de fraudes.
-   Sistemas de recomendação (agrupamento de usuários/itens).
-   Compressão de dados.

## 6. Aprendizado por Reforço

### 6.1. Conceito

No Aprendizado por Reforço, um **agente** aprende a tomar decisões sequenciais em um **ambiente** para maximizar uma **recompensa** acumulada. O agente aprende por **tentativa e erro**, recebendo feedback (recompensa ou punição) após cada ação [6].

### 6.2. Componentes Principais

-   **Agente**: O aprendiz ou tomador de decisões.
-   **Ambiente**: O mundo com o qual o agente interage.
-   **Estado**: A situação atual do ambiente.
-   **Ação**: O que o agente pode fazer no ambiente.
-   **Recompensa**: Feedback numérico que o ambiente dá ao agente.
-   **Política**: A estratégia que o agente usa para escolher a próxima ação [6].

### 6.3. Objetivo

O objetivo do agente é aprender uma política ótima que maximize a recompensa total a longo prazo [6].

### 6.4. Exemplos de Aplicação

-   Jogos (AlphaGo, xadrez).
-   Robótica (controle de robôs, navegação autônoma).
-   Veículos autônomos.
-   Otimização de sistemas (gerenciamento de tráfego, controle de estoque).

## 7. O Processo de Desenvolvimento de um Modelo de ML (Pipeline)

O desenvolvimento de um modelo de Machine Learning geralmente segue um pipeline estruturado [6]:

1.  **Definição do Problema**: Entender claramente o que se quer resolver, quais são os objetivos e as métricas de sucesso.
2.  **Coleta de Dados**: Reunir os dados relevantes para o problema. A qualidade e a quantidade são cruciais.
3.  **Limpeza e Pré-processamento de Dados**: Tratar valores ausentes, remover ruídos, padronizar formatos, lidar com outliers. Esta é uma das etapas mais demoradas e importantes.
4.  **Engenharia de Features**: Criar novas features a partir das existentes que possam melhorar o desempenho do modelo. Selecionar as features mais relevantes.
5.  **Divisão dos Dados**: Separar o conjunto de dados em subconjuntos de treinamento, validação e teste. Uma divisão comum é 70% treino, 15% validação, 15% teste.
6.  **Seleção e Treinamento do Modelo**: Escolher o algoritmo de ML mais adequado e treiná-lo com os dados de treinamento.
7.  **Avaliação do Modelo**: Medir o desempenho do modelo nos dados de validação e teste usando métricas apropriadas. Ajustar hiperparâmetros.
8.  **Implantação e Monitoramento**: Colocar o modelo em produção e monitorar seu desempenho continuamente, pois os dados do mundo real podem mudar (deriva de dados).

## 8. Importância da Qualidade dos Dados

> "Garbage In, Garbage Out" (Lixo entra, lixo sai).

A qualidade dos dados é o fator mais crítico para o sucesso de um modelo de ML. Dados de baixa qualidade podem levar a modelos imprecisos, vieses e decisões erradas. Aspectos importantes da qualidade dos dados incluem [6]:

-   **Completude**: Ausência de valores faltantes.
-   **Consistência**: Dados sem contradições.
-   **Precisão**: Dados corretos e sem erros.
-   **Relevância**: Dados que realmente contribuem para resolver o problema.
-   **Representatividade**: Dados que refletem a diversidade do mundo real para evitar vieses.

## 9. Overfitting e Underfitting

Dois problemas comuns no treinamento de modelos de ML [6]:

-   **Overfitting (Sobreajuste)**: O modelo aprende os dados de treinamento **muito bem**, incluindo o ruído e as particularidades específicas desse conjunto. Como resultado, ele tem um desempenho excelente nos dados de treinamento, mas **generaliza mal** para novos dados não vistos. É como um aluno que memoriza as respostas de um livro, mas não entende a matéria.
-   **Underfitting (Subajuste)**: O modelo é **muito simples** para capturar os padrões subjacentes nos dados. Ele tem um desempenho ruim tanto nos dados de treinamento quanto nos dados novos. É como um aluno que não aprendeu o suficiente para resolver nem os problemas básicos.

**Como mitigar:**

-   **Overfitting**: Mais dados de treinamento, regularização, validação cruzada, redução da complexidade do modelo, poda de árvores de decisão.
-   **Underfitting**: Aumentar a complexidade do modelo, adicionar mais features, reduzir a regularização.

## 10. Métricas de Avaliação (Classificação)

Para problemas de classificação, diversas métricas são usadas para avaliar o desempenho do modelo [6]:

-   **Acurácia**: Proporção de previsões corretas sobre o total de previsões. (Bom para classes balanceadas).
-   **Precisão (Precision)**: Proporção de verdadeiros positivos sobre o total de positivos previstos. (Quantos dos que eu previ como positivos são realmente positivos?).
-   **Recall (Sensibilidade)**: Proporção de verdadeiros positivos sobre o total de positivos reais. (Quantos dos positivos reais eu consegui detectar?).
-   **F1-Score**: Média harmônica entre Precisão e Recall. Útil quando há um desequilíbrio entre as classes.
-   **Matriz de Confusão**: Tabela que resume o desempenho do modelo, mostrando Verdadeiros Positivos (VP), Verdadeiros Negativos (VN), Falsos Positivos (FP) e Falsos Negativos (FN).
-   **Curva ROC e AUC (Area Under the Curve)**: Avalia a capacidade do modelo de distinguir entre classes em diferentes limiares de classificação.

## 11. Métricas de Avaliação (Regressão)

Para problemas de regressão, as métricas medem a diferença entre os valores previstos e os valores reais [6]:

-   **Erro Médio Absoluto (MAE - Mean Absolute Error)**: Média do valor absoluto dos erros. Menos sensível a outliers.
-   **Erro Quadrático Médio (MSE - Mean Squared Error)**: Média dos erros ao quadrado. Penaliza erros maiores mais severamente.
-   **Raiz do Erro Quadrático Médio (RMSE - Root Mean Squared Error)**: Raiz quadrada do MSE. Está na mesma unidade da variável alvo, facilitando a interpretação.
-   **R² (Coeficiente de Determinação)**: Indica a proporção da variância na variável dependente que é previsível a partir das variáveis independentes. Varia de 0 a 1, onde 1 indica um ajuste perfeito.

## 12. Aplicações do Aprendizado de Máquina

O Aprendizado de Máquina está presente em quase todos os setores [6]:

-   **Saúde**: Diagnóstico de doenças, descoberta de medicamentos, análise de imagens médicas.
-   **Finanças**: Detecção de fraudes, previsão de mercado, avaliação de risco de crédito.
-   **Varejo**: Sistemas de recomendação, previsão de demanda, otimização de preços.
-   **Transporte**: Veículos autônomos, otimização de rotas, gerenciamento de tráfego.
-   **Tecnologia**: Reconhecimento de voz, processamento de linguagem natural, visão computacional.
-   **Agricultura**: Monitoramento de culturas, previsão de colheitas, detecção de pragas.
