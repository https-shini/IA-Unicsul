# Aula 02 — Histórico da IA e Sistemas Inteligentes

> Material de estudo estruturado a partir do conteúdo da aula, organizado para consulta, revisão e aprofundamento.

---

## Sumário

1. [Por que Estudar a História da IA?](#1-por-que-estudar-a-história-da-ia)
2. [Antecedentes Filosóficos](#2-antecedentes-filosóficos)
3. [Alan Turing: o Pai da Computação](#3-alan-turing-o-pai-da-computação)
4. [Nascimento Oficial da IA (1955–1956)](#4-nascimento-oficial-da-ia-19551956)
5. [Otimismo Inicial (1950–1960)](#5-otimismo-inicial-19501960)
6. [IA Simbólica (anos 1960–1970)](#6-ia-simbólica-anos-19601970)
7. [Crise do Simbólico (anos 1980)](#7-crise-do-simbólico-anos-1980)
8. [A Sala Chinesa (Searle, 1980)](#8-a-sala-chinesa-searle-1980)
9. [Formalização do Conceito de Agente (1995)](#9-formalização-do-conceito-de-agente-1995)
10. [Agente Inteligente](#10-agente-inteligente)
11. [Tipologia dos Agentes Inteligentes](#11-tipologia-dos-agentes-inteligentes)
12. [Linha do Tempo Consolidada](#12-linha-do-tempo-consolidada)
13. [Era Atual: Agentes Generativos e Generalistas](#13-era-atual-agentes-generativos-e-generalistas)
14. [Síntese: O que é um Sistema Inteligente?](#14-síntese-o-que-é-um-sistema-inteligente)
15. [Resumo da Aula](#15-resumo-da-aula)

---

## 1. Por que Estudar a História da IA?

- **Compreender o contexto atual** — entender como o passado moldou o presente.
- **Identificar padrões** — reconhecer tendências de sucesso e fracasso.
- **Direcionar soluções** — aprender com problemas já enfrentados.

## 2. Antecedentes Filosóficos

### 2.1 Descartes (séc. XVII)

No *Discurso sobre o Método*, Descartes afirmou que **autômatos** (máquinas) não conseguem **adaptar a linguagem conforme a situação**, ao contrário dos humanos. Essa distinção entre flexibilidade humana e rigidez mecânica antecipou, em séculos, o **Teste de Turing**.

### 2.2 Diderot (séc. XVIII)

Diderot sugeriu que **um papagaio capaz de responder a qualquer pergunta seria considerado inteligente**. A reflexão antecipou debates sobre cognição animal e estabeleceu a **capacidade de resposta** como critério de inteligência — ideia que reaparece tanto no Teste de Turing quanto na crítica da Sala Chinesa.

## 3. Alan Turing: o Pai da Computação

### 3.1 Máquina de Turing

Modelo matemático teórico que representa qualquer processo computacional, com **memória ilimitada** e capacidade de **ler e escrever símbolos**. Tornou-se a base teórica de todos os computadores modernos.

### 3.2 O Artigo de 1950

Em "*Computing Machinery and Intelligence*", Turing levanta a pergunta: **"As máquinas podem pensar?"**. Reconhecendo a ambiguidade da pergunta, ele a substitui por outra mais operacional: **uma máquina pode imitar tão bem o comportamento humano a ponto de ser indistinguível dele?**

### 3.3 O Teste de Turing (Jogo da Imitação)

**Estrutura:**

- Três participantes: um interrogador humano, um humano e uma máquina.
- Toda a comunicação ocorre **exclusivamente por texto**.
- O interrogador deve descobrir quem é o humano e quem é a máquina.

**Critério:** se o interrogador não conseguir distinguir corretamente, considera-se que a máquina exibe comportamento inteligente.

**Observação importante:** o teste avalia **imitação**, não **correção**. Não importa se as respostas são verdadeiras — importa se são humanamente plausíveis.

## 4. Nascimento Oficial da IA (1955–1956)

- **1955** — John McCarthy cunha o termo **"Inteligência Artificial"**.
- **1956** — A **Conferência de Dartmouth**, organizada por John McCarthy, Marvin Minsky, Claude Shannon e Nathaniel Rochester, estabelece a IA como campo formal de pesquisa.
- **1958** — Criação da linguagem **LISP**, fundamental para o desenvolvimento de sistemas de IA por sua flexibilidade simbólica.

## 5. Otimismo Inicial (1950–1960)

- Primeiros programas de **xadrez** computacional.
- Sistemas de **prova automática de teoremas**.
- Cientistas confiantes de que a **IA geral** seria alcançada em poucas décadas.

## 6. IA Simbólica (anos 1960–1970)

### 6.1 Características

- Representação do conhecimento por **símbolos e regras lógicas**.
- Operação em **ambientes bem definidos**.
- **Pouca capacidade de adaptação** a situações imprevistas.

### 6.2 ELIZA (1966)

Programa que simulava um **psicoterapeuta**, baseado em palavras-chave e respostas genéricas. Apesar de simples, gerou interações tão convincentes que muitos usuários acreditaram conversar com um humano.

### 6.3 Sistemas Especialistas (anos 1970)

Sistemas que codificavam o **conhecimento de especialistas humanos** em regras lógicas:

- **MYCIN** — diagnóstico médico baseado em regras.
- **DENDRAL** — análise química automatizada.

## 7. Crise do Simbólico (anos 1980)

A IA simbólica enfrentou limitações significativas:

- Dificuldade com **ambientes incertos e ruidosos**.
- Inflexibilidade diante de situações não previstas pelas regras.

Esse impasse impulsionou o **conexionismo**, abordagem baseada em **redes neurais**, mais flexível e adaptativa.

## 8. A Sala Chinesa (Searle, 1980)

### 8.1 O Experimento Mental

Imagine uma pessoa fechada em uma sala, sem saber chinês, recebendo perguntas escritas em chinês. Ela utiliza um **manual de instruções** para combinar símbolos e produzir respostas em chinês corretas. Para alguém de fora, parece haver compreensão genuína do idioma — mas a pessoa **não entende absolutamente nada**.

### 8.2 A Crítica

Searle argumenta que **simular respostas corretas não equivale a compreender**. O experimento mostra que:

- **Sintaxe** (manipulação de símbolos) ≠ **Semântica** (compreensão).
- Passar no Teste de Turing **não implica consciência ou entendimento real**.

### 8.3 Relevância Atual

A crítica da Sala Chinesa permanece central no debate sobre **modelos de linguagem (LLMs)**: eles produzem respostas coerentes, mas isso não prova que compreendem o significado do que produzem.

## 9. Formalização do Conceito de Agente (1995)

**Stuart Russell e Peter Norvig**, na obra *Artificial Intelligence: A Modern Approach*, consolidaram a definição rigorosa de **agente inteligente**, redefinindo o foco da IA: do "pensar como humanos" para o "agir racionalmente".

## 10. Agente Inteligente

### 10.1 Definição

Um **agente inteligente** é uma entidade que:

- **Percebe o ambiente** por meio de **sensores**
- **Age sobre o ambiente** por meio de **atuadores**
- **Toma decisões autônomas** para alcançar objetivos

### 10.2 Exemplos

| Agente | Sensores | Atuadores |
|---|---|---|
| Termostato inteligente | Sensor de temperatura | Controle do aquecedor |
| Robô aspirador | Sensores de colisão e proximidade | Rodas e motor de sucção |
| Assistente virtual | Microfone | Alto-falante |
| Sistema de recomendação | Histórico de uso, cliques | Interface com sugestões |

## 11. Tipologia dos Agentes Inteligentes

### 11.1 Agentes Reflexivos Simples

- **Decidem com base apenas na percepção atual**, ignorando histórico.
- Operam por regras do tipo `SE condição ENTÃO ação`.
- **Exemplo:** termostato que liga ou desliga conforme a temperatura.

### 11.2 Agentes Baseados em Modelos

- Mantêm um **modelo interno do mundo**.
- Conseguem inferir estados não diretamente observáveis e prever consequências.
- **Exemplo:** carro autônomo que antecipa o movimento de outros veículos.

### 11.3 Agentes Baseados em Objetivos

- Possuem uma **meta explícita** (estado desejado).
- Escolhem ações que **minimizam a distância** entre o estado atual e o objetivo.
- **Exemplo:** GPS que calcula a rota até o destino.

### 11.4 Agentes Baseados em Utilidade

- Vão além da meta: **diferenciam o quão bom é um estado**.
- Maximizam uma **função de utilidade**, escolhendo a melhor opção entre várias possíveis.
- **Exemplo:** algoritmo de investimentos que pondera risco e retorno.

## 12. Linha do Tempo Consolidada

| Período | Paradigma / Marco |
|---|---|
| Séc. XVII | Descartes — distinção humano/autômato |
| Séc. XVIII | Diderot — papagaio inteligente |
| 1950 | Teste de Turing |
| 1955–56 | Termo "IA" e Conferência de Dartmouth |
| 1958 | Linguagem LISP |
| 1960–70 | IA Simbólica; ELIZA (1966) |
| 1970 | Sistemas Especialistas (MYCIN, DENDRAL) |
| 1980 | Crise do simbólico; Sala Chinesa; ascensão do conexionismo |
| 1995 | Russell & Norvig formalizam o agente inteligente |
| 2000–2010 | Expansão com Machine Learning estatístico |
| 2010–2020 | Era do Deep Learning (AlexNet, 2012; AlphaGo, 2016) |
| 2020+ | Modelos fundacionais e agentes generativos (GPT, Claude, Gemini, Llama) |

## 13. Era Atual: Agentes Generativos e Generalistas

### 13.1 Modelos Fundacionais

Grandes modelos pré-treinados (GPT, Claude, Gemini, Llama) capazes de:

- Executar **múltiplas tarefas** com pouca adaptação adicional.
- Gerar **textos, imagens e código**.
- Operar com **autonomia**.
- **Colaborar** com humanos e outros agentes.

### 13.2 Definição Contemporânea de Agente (Bornet et al., 2024)

> *"Entidade digital autônoma, orientada a objetivos, capaz de executar tarefas de múltiplos passos de maneira independente, sem depender de comandos constantes dos humanos."*

**Diferença em relação à IA generativa pura:** o agente **age proativamente, planeja, ajusta e executa fluxos completos**, em vez de apenas responder a prompts isolados.

## 14. Síntese: O que é um Sistema Inteligente?

Um sistema inteligente é um agente que:

- ✅ **Percebe** o ambiente
- ✅ **Raciocina** com base em conhecimento
- ✅ **Age** em direção a objetivos
- ✅ **Aprende** com a experiência
- ✅ **Colabora** com humanos ou outros agentes

## 15. Resumo da Aula

- A IA tem raízes filosóficas que remontam a **Descartes e Diderot**.
- **Turing (1950)** e **Dartmouth (1956)** marcam o início formal do campo.
- A trajetória da IA alterna entre paradigmas: **simbólico (1960–80)**, **conexionista (1980+)**, **estatístico (2000+)** e **deep learning (2010+)**.
- A **Sala Chinesa** permanece como crítica filosófica central ao Teste de Turing.
- O conceito de **agente inteligente** unifica a área e se atualiza com os **modelos fundacionais** atuais.
