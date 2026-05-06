# Aula 05 – Resolução de Problemas por meio de Buscas em Inteligência Artificial

> Material de estudo estruturado a partir do conteúdo da aula, organizado para consulta, revisão e aprofundamento.

---

## Sumário

1. [O Problema da Decisão em IA](#1-o-problema-da-decisão-em-ia)
2. [Definição Formal do Problema](#2-definição-formal-do-problema)
3. [O Espaço de Estados](#3-o-espaço-de-estados)
4. [Árvore de Busca](#4-árvore-de-busca)
5. [Classificação das Buscas](#5-classificação-das-buscas)
6. [Critérios de Avaliação de Busca](#6-critérios-de-avaliação-de-busca)
7. [Fronteira (Open List)](#7-fronteira-open-list)
8. [Busca Sem Informação (Cega)](#8-busca-sem-informação-cega)
9. [Busca Com Informação (Heurística)](#9-busca-com-informação-heurística)
10. [Desafios Reais: Explosão Combinatória](#10-desafios-reais-explosão-combinatória)
11. [Implementação e Contexto em IA](#11-implementação-e-contexto-em-ia)
12. [Aplicações no Mundo Real](#12-aplicações-no-mundo-real)

---

## 1. O Problema da Decisão em IA

Em Inteligência Artificial, "resolver um problema" significa encontrar uma sequência de ações que conduza do ponto inicial, chamado **Estado Inicial**, ao ponto desejado, chamado **Estado Objetivo**. O processo é análogo a navegar em um labirinto sem mapa: tenta-se um caminho e, caso não funcione, retorna-se e tenta-se outro. Essa é a essência da **busca**.

---

## 2. Definição Formal do Problema

Um problema em IA é formalmente definido por cinco componentes:

| Componente | Definição | Exemplo |
|---|---|---|
| **Estado Inicial** | Ponto de partida do agente | Posição inicial do jogador em um mapa |
| **Ações (Operadores)** | Operações disponíveis para mudar o estado | Andar para frente, virar à direita |
| **Modelo de Transição** | Resultado de aplicar uma ação a um estado | Se fizer a Ação X no Estado Y, qual é o novo estado? |
| **Teste de Objetivo** | Critério que indica se o objetivo foi alcançado | Chegou à bandeira final |
| **Custo de Caminho** | Custo acumulado para chegar ao objetivo | Tempo, distância ou recursos consumidos |

---

## 3. O Espaço de Estados

O **Espaço de Estados** é o conjunto de todas as configurações possíveis que um problema pode assumir. O objetivo do agente é navegar nesse espaço, partindo do estado inicial e chegando ao estado objetivo.

> **Exemplo:** no jogo da velha, o espaço de estados é composto por todas as grades 3x3 possíveis, com cada combinação de X, O e casas vazias representando um estado distinto.

O espaço de estados pode ser representado como um grafo, onde cada nó é um estado e cada aresta é uma ação que conecta dois estados.

---

## 4. Árvore de Busca

A **Árvore de Busca** representa as possibilidades de caminho a partir do estado inicial:

- A **raiz** corresponde ao estado inicial.
- Os **ramos** representam as ações possíveis em cada estado.
- Os **nós** representam os estados resultantes após cada ação.

> **Atenção:** a árvore pode crescer de forma exponencial. A estratégia de busca define como navegar por ela sem se perder ou consumir recursos desnecessários.

---

## 5. Classificação das Buscas

As estratégias de busca são divididas em duas grandes categorias:

| Categoria | Descrição |
|---|---|
| **Busca Sem Informação (Cega)** | O agente não possui conhecimento prévio sobre qual caminho é melhor. Explora as possibilidades de forma sistemática, sem direcionamento. |
| **Busca Com Informação (Heurística)** | O agente utiliza uma função heurística como estimativa de qual direção é mais promissora, guiando a busca de forma mais eficiente. |

---

## 6. Critérios de Avaliação de Busca

Para comparar e selecionar estratégias de busca, utilizam-se quatro critérios:

| Critério | Pergunta correspondente |
|---|---|
| **Completude** | O algoritmo encontra uma solução se ela existir? |
| **Otimização** | O algoritmo encontra a melhor solução, ou seja, a mais curta ou de menor custo? |
| **Complexidade de Tempo** | Quanto tempo o algoritmo leva para encontrar a solução? |
| **Complexidade de Espaço** | Quanta memória o algoritmo consome durante a execução? |

---

## 7. Fronteira (Open List)

A **Fronteira**, também chamada de *Open List*, é a estrutura de dados que armazena os nós aguardando exploração. O algoritmo não processa todos os nós de uma vez, mas mantém essa lista de "próximos estados a visitar" e a expande progressivamente.

A diferença central entre os algoritmos de busca está na **ordem em que a fronteira é organizada**:

- **Fila (FIFO):** utilizada na BFS, expande os nós na ordem em que foram inseridos.
- **Pilha (LIFO):** utilizada na DFS, expande sempre o nó inserido por último.
- **Fila de Prioridade:** utilizada na UCS e no A*, expande o nó de menor custo ou melhor estimativa.

---

## Parte I – Busca Sem Informação (Cega)

---

### 8. Busca Sem Informação (Cega)

#### 8.1. Busca em Largura (BFS – Breadth-First Search)

**Funcionamento:** expande todos os nós de um nível antes de avançar para o próximo, propagando-se como ondas a partir da raiz. Utiliza uma **Fila (FIFO)**.

| Aspecto | Avaliação |
|---|---|
| Completude | Sim, sempre encontra uma solução se ela existir |
| Otimização | Sim, garante o caminho com menor número de passos |
| Memória | Alta, pois armazena todos os nós do nível atual antes de avançar |

---

#### 8.2. Busca em Profundidade (DFS – Depth-First Search)

**Funcionamento:** percorre um caminho até seu limite antes de retroceder e explorar outras ramificações. Utiliza uma **Pilha (LIFO)**.

| Aspecto | Avaliação |
|---|---|
| Completude | Não, pode entrar em ciclos ou caminhos infinitos |
| Otimização | Não, não garante o caminho mais curto |
| Memória | Baixa, armazena apenas o caminho atual |

> **Boas práticas:** manter uma **Closed List** com os estados já visitados é essencial para evitar loops e revisitar estados desnecessariamente.

---

#### 8.3. Busca de Custo Uniforme (UCS – Uniform Cost Search)

**Funcionamento:** variação da BFS que expande sempre o nó com o **menor custo acumulado** até o momento. Indicada quando as ações possuem custos distintos. Utiliza uma **Fila de Prioridade** ordenada pelo custo acumulado `g(n)`.

| Aspecto | Avaliação |
|---|---|
| Completude | Sim |
| Otimização | Sim, garante o menor custo total |
| Memória | Alta |

---

## Parte II – Busca Com Informação (Heurística)

---

### 9. Busca Com Informação (Heurística)

#### 9.1. O que é Heurística?

Uma **heurística** `h(n)` é uma função que estima o custo restante do nó atual `n` até o objetivo. Por definição, `h(objetivo) = 0`. Uma boa heurística reduz drasticamente o espaço de busca explorado.

> **Analogia:** a distância em linha reta no GPS é uma heurística. Ela não representa o caminho real pelas ruas, mas orienta o algoritmo na direção correta.

Uma heurística é considerada **admissível** quando nunca superestima o custo real até o objetivo, e **consistente** quando satisfaz a desigualdade triangular entre nós adjacentes.

---

#### 9.2. Busca Gulosa (Best-First Search)

**Estratégia:** expande sempre o nó com o menor valor de `h(n)`, ou seja, o que parece mais próximo do objetivo, ignorando o custo já percorrido.

| Aspecto | Avaliação |
|---|---|
| Completude | Não |
| Otimização | Não, pode ser enganada por obstáculos locais |
| Memória | Média |

---

#### 9.3. Busca A* (A-Star)

O **A\*** é o algoritmo de busca informada mais utilizado e estudado. Combina o custo real percorrido com a estimativa heurística em uma única função de avaliação:

```
f(n) = g(n) + h(n)
```

| Variável | Significado |
|---|---|
| `g(n)` | Custo real acumulado do estado inicial até o nó `n` |
| `h(n)` | Estimativa heurística do custo restante de `n` até o objetivo |
| `f(n)` | Estimativa do custo total do caminho passando por `n` |

> **Garantia:** se a heurística for **admissível** e **consistente**, o A\* é simultaneamente **completo** e **ótimo**. Ele equilibra o que já foi percorrido com o que ainda falta, evitando tanto desperdício quanto atalhos enganosos.

---

#### 9.4. Comparativo Geral dos Algoritmos

| Algoritmo | Completude | Otimização | Memória |
|---|---|---|---|
| **BFS** | Sim | Sim (por passos) | Alta |
| **DFS** | Não | Não | Baixa |
| **UCS** | Sim | Sim (por custo) | Alta |
| **Busca Gulosa** | Não | Não | Média |
| **A\*** | Sim | Sim (por custo) | Alta |

---

## 10. Desafios Reais: Explosão Combinatória

A **explosão combinatória** é o fenômeno pelo qual o número de estados possíveis cresce de forma exponencial ou fatorial conforme o tamanho do problema aumenta. Isso torna a busca exaustiva inviável na maioria dos cenários reais.

> **Exemplo:** o jogo de xadrez possui mais estados possíveis do que átomos no universo observável. Nenhum computador pode explorá-los todos.

Para contornar esse problema, utilizam-se heurísticas fortes, algoritmos com restrições de memória, como o IDA*, e técnicas de poda que eliminam ramos improváveis antes de expandi-los.

---

## 11. Implementação e Contexto em IA

Na prática, cada **nó** em um algoritmo de busca armazena as seguintes informações:

| Campo | Descrição |
|---|---|
| **Estado** | Configuração atual representada pelo nó |
| **Nó pai** | Nó que gerou o atual, permitindo reconstruir o caminho |
| **Ação** | Operação aplicada ao nó pai para chegar ao nó atual |
| **Custo acumulado** `g` | Soma dos custos desde o estado inicial |
| **Profundidade** | Nível do nó na árvore de busca |

A **Fronteira** é a estrutura que define o comportamento do algoritmo: Fila para BFS, Pilha para DFS e Fila de Prioridade para UCS e A*.

---

## 12. Aplicações no Mundo Real

Algoritmos de busca estão presentes em diversas aplicações cotidianas e industriais:

| Aplicação | Algoritmo | Descrição |
|---|---|---|
| **GPS (Waze, Google Maps)** | A* | Heurística de distância em linha reta combinada com dados de tráfego em tempo real |
| **Jogos digitais (IA de inimigos)** | A* | Cálculo do caminho mais eficiente até o jogador em mapas complexos |
| **Roteamento de redes** | Dijkstra / UCS | Envio de pacotes de dados pelo trajeto de menor latência |
| **Robótica** | A* e variações | Planejamento de trajetória para evitar obstáculos físicos |
| **Problemas clássicos de IA** | BFS / DFS | Problema do missionário e canibais, quebra-cabeças de 8 peças |

---

> *Material organizado para a disciplina de Fundamentos de Inteligência Artificial - Ciência da Computação, Universidade Cruzeiro do Sul.*
