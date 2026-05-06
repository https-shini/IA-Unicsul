# Aula 03 — Abordagens da Inteligência Artificial

## Enfoques Simbólico e Conexionista; Sistema de Símbolos Físicos

---

## 1. As Duas Grandes Tradições da IA

A Inteligência Artificial possui duas grandes tradições históricas que dominaram a área por mais de cinco décadas, cada uma com seus princípios, benefícios e limitações:

- **IA Simbólica** (também chamada de IA clássica)
- **IA Conexionista** (baseada em redes neurais)

---

## 2. Inteligência Artificial Simbólica

### 2.1. Definição

Na IA Simbólica, o conhecimento é representado por meio de **símbolos**, tais como:

- Palavras
- Frases
- Conceitos

Esses símbolos são organizados em **estruturas lógicas**, e o sistema manipula esses símbolos para:

- Resolver problemas
- Raciocinar
- Tomar decisões

### 2.2. Origens

- Pesquisa ativa desde a **década de 1950**
- Foi a **primeira abordagem** utilizada para criar sistemas de IA
- Dominou o campo por mais de 50 anos

### 2.3. Exemplos de Sistemas Simbólicos

- **Sistemas especialistas** (MYCIN, DENDRAL)
- **Prova automática de teoremas**
- **Lógica formal**
- **Programação em LISP**
- **Jogos de xadrez baseados em regras**

### 2.4. Como Funciona a Manipulação de Símbolos

O processo simbólico segue quatro etapas fundamentais:

1. **Representar o conhecimento como símbolos** (ex: "gato", "mamífero", "tem pelo")
2. **Estabelecer regras lógicas** (ex: "SE tem pelo E amamenta ENTÃO é mamífero")
3. **Aplicar as regras** para deduzir novo conhecimento
4. **Responder perguntas ou tomar decisões** com base nas deduções

### 2.5. Benefícios da IA Simbólica

- **Interpretabilidade**: símbolos e regras são compreensíveis para humanos
- **Raciocínio lógico**: dedução de novas informações a partir de dados existentes
- **Tomada de decisão transparente**: processo auditável
- **Manejo de incerteza**: através de lógica difusa e lógica probabilística

### 2.6. Limitações da IA Simbólica

- **Complexidade e ambiguidade**: dificuldade em formalizar conhecimento do mundo real
- **Aprendizado a partir de dados**: o sistema não aprende com exemplos
- **Escalabilidade**: problemas grandes exigem muitas regras
- **Adaptação a mudanças**: atualizar regras é lento e trabalhoso

---

## 3. O Sistema de Símbolos Físicos

### 3.1. Hipótese Fundamental

A hipótese fundamental da IA Simbólica afirma que:

> **Um sistema inteligente pode ser construído manipulando símbolos físicos que representam conhecimento.**

Segundo essa visão, **a mente humana também seria um sistema de símbolos físicos**, o que coloca a inteligência humana e a inteligência artificial sob o mesmo princípio explicativo: a manipulação simbólica.

---

## 4. Inteligência Artificial Conexionista

### 4.1. Definição

A IA Conexionista compreende sistemas inspirados na **estrutura do cérebro humano**, sendo:

- Constituídos por redes de unidades conectadas (**neurônios artificiais**)
- A comunicação ocorre através de **sinapses artificiais** (pesos)

### 4.2. Origens do Conexionismo

- Ganhou destaque a partir dos **anos 1980**
- Sinergia com o surgimento de computadores mais potentes
- Capacidade crescente de processar grandes volumes de dados

### 4.3. Redes Neurais Artificiais

As redes neurais artificiais:

- Modelam processos psicológicos e cognitivos
- Apresentam padrões de atividade distribuídos por uma rede de unidades simples
- Cada unidade processa informação e a passa adiante

### 4.4. Aprendizado nas Redes Neurais

A característica central do conexionismo é que o **conhecimento não é programado — é aprendido**. O processo segue as seguintes etapas:

1. O sistema é alimentado com dados
2. Algoritmos ajustam os pesos das conexões
3. A rede reconhece padrões
4. A rede passa a fazer previsões

### 4.5. Aplicações da IA Conexionista

A IA Conexionista é especialmente adequada para problemas em que o conhecimento não é bem estruturado ou é difícil de representar com símbolos:

- Visão computacional
- Processamento de linguagem natural
- Reconhecimento de voz
- Diagnóstico por imagem

### 4.6. Benefícios da IA Conexionista

- **Aprendizado adaptativo**: ajusta o comportamento automaticamente
- **Processamento paralelo**: realiza múltiplas tarefas simultâneas
- **Generalização**: aprende com exemplos e aplica a situações novas
- **Adaptação a mudanças**: adequada para ambientes dinâmicos
- **Reconhecimento de padrões**: excelente em imagens, sons e texto

### 4.7. Limitações da IA Conexionista

- **Interpretabilidade**: é uma "caixa-preta", sendo difícil explicar decisões
- **Requerimento de dados extensos**: precisa de grandes conjuntos de treinamento
- **Treinamento demorado**: computacionalmente intensivo
- **Custo**: caro em termos de infraestrutura

---

## 5. Tabela Comparativa: Simbólica vs. Conexionista

| Critério            | Simbólica                  | Conexionista              |
|---------------------|----------------------------|---------------------------|
| Representação       | Símbolos e regras          | Pesos e conexões          |
| Conhecimento        | Programado explicitamente  | Aprendido de dados        |
| Interpretação       | Fácil (transparente)       | Difícil ("caixa-preta")   |
| Aprendizado         | Não aprende sozinha        | Aprende com exemplos      |
| Domínio típico      | Problemas lógicos          | Padrões complexos         |
| Dados necessários   | Poucos (conhecimento)      | Muitos (exemplos)         |

---

## 6. Abordagens Complementares

As abordagens simbólica e conexionista **não constituem uma disputa por superioridade**. Ambas são importantes e complementares:

- **Simbólica**: mais apropriada para conhecimento bem estruturado e raciocínio lógico
- **Conexionista**: mais adequada para padrões complexos e grandes volumes de dados

---

## 7. Estudos de Caso

### 7.1. IBM Watson

Combina IA simbólica e conexionista:

- Compreende linguagem natural via PLN (componente conexionista)
- Gera conhecimento a partir de dados estruturados e não estruturados
- Aplica regras e raciocínio (componente simbólico)
- **Aplicações**: diagnóstico médico, análise de sentimentos, serviços financeiros

### 7.2. Tesla Autopilot

- Predominantemente **conexionista**
- Redes neurais processam informações de sensores e câmeras
- Aprendizado supervisionado para condução autônoma
- É uma IA estreita (tarefa específica), mas com aprendizado profundo

### 7.3. AlphaGo

- Combina **aprendizado por reforço + redes neurais**
- Jogou milhões de partidas contra si mesmo
- Aprendeu estratégias sem regras explícitas
- Venceu campeões mundiais
- Considerado IA fraca com elementos de IA forte (aprendizado autônomo)

### 7.4. ChatGPT

- Predominantemente **conexionista** (deep learning)
- Modelo de linguagem baseado em redes neurais profundas
- Treinado com enormes volumes de texto
- Gera respostas coerentes sem regras linguísticas explícitas

---

## 8. Tendência Atual: Abordagens Híbridas

Atualmente, pesquisadores buscam combinar o melhor das duas abordagens, dando origem a sistemas **neuro-simbólicos**, nos quais:

- Redes neurais são usadas para **percepção e padrões**
- Símbolos e regras são usados para **raciocínio e explicação**

O resultado é uma IA mais robusta, interpretável e capaz.

---

## 9. Por Que Esse Tema Importa

Conhecer as duas abordagens permite:

- Escolher a ferramenta certa para cada problema
- Entender benefícios e limitações dos sistemas atuais
- Perceber que a IA não é "mágica" — há escolhas de projeto
- Acompanhar debates sobre explicabilidade e ética

---

## 10. Resumo

- **IA simbólica**: representa conhecimento via símbolos e regras lógicas; é interpretável, mas não aprende
- **IA conexionista**: utiliza redes neurais inspiradas no cérebro; aprende com dados, mas é uma "caixa-preta"
- **Hipótese do sistema de símbolos físicos**: inteligência equivale à manipulação de símbolos
- **Cada abordagem** apresenta benefícios e limitações específicas
- **Tendência atual**: convergência para sistemas híbridos (neuro-simbólicos)
