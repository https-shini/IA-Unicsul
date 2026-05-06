# Aula 03 — Exercícios

## Abordagens da Inteligência Artificial: Simbólica e Conexionista

---

## Nível Básico

### Exercício 1

**Pergunta:** O que caracteriza a abordagem simbólica da Inteligência Artificial em relação à forma como o conhecimento é representado?

**Resposta:** Na IA Simbólica, o conhecimento é representado por meio de **símbolos** (palavras, frases, conceitos) organizados em **estruturas lógicas**. O sistema manipula esses símbolos por meio de regras explícitas para resolver problemas, raciocinar e tomar decisões.

---

### Exercício 2

**Pergunta:** Em que década a IA Simbólica começou a ser desenvolvida e por quanto tempo dominou a área?

**Resposta:** A IA Simbólica começou a ser pesquisada ativamente a partir da **década de 1950**, sendo a primeira abordagem utilizada para criar sistemas de IA. Ela dominou o campo por **mais de 50 anos**.

---

### Exercício 3

**Pergunta:** Cite três exemplos de sistemas baseados na abordagem simbólica.

**Resposta:** Exemplos de sistemas simbólicos:

1. Sistemas especialistas (MYCIN, DENDRAL)
2. Prova automática de teoremas
3. Programação em LISP

Outros exemplos válidos: lógica formal e jogos de xadrez baseados em regras.

---

### Exercício 4

**Pergunta:** Em que a IA Conexionista se inspira?

**Resposta:** A IA Conexionista se inspira na **estrutura do cérebro humano**, sendo constituída por redes de unidades conectadas (neurônios artificiais) que se comunicam por meio de sinapses artificiais (pesos).

---

### Exercício 5

**Pergunta:** Qual é a principal diferença entre IA Simbólica e IA Conexionista no que se refere à aquisição de conhecimento?

**Resposta:** Na IA Simbólica, o conhecimento é **programado explicitamente** por humanos. Na IA Conexionista, o conhecimento é **aprendido a partir de dados**, por meio do ajuste automático dos pesos das conexões entre os neurônios.

---

## Nível Intermediário

### Exercício 6

**Pergunta:** Explique, com suas próprias palavras, o que é Inteligência Artificial Simbólica, abordando: (a) como o conhecimento é representado; (b) qual foi seu período histórico de surgimento e predominância; (c) dois exemplos de sistemas que utilizam essa abordagem.

**Resposta:**

**(a) Representação do conhecimento:** Na IA Simbólica, o conhecimento é representado por símbolos (palavras, conceitos, frases) organizados em estruturas lógicas. O raciocínio ocorre por meio da aplicação de regras explícitas (geralmente do tipo "SE-ENTÃO") sobre esses símbolos.

**(b) Período histórico:** A abordagem surgiu na década de 1950 e dominou a pesquisa em IA por mais de 50 anos, sendo a primeira tradição utilizada para construir sistemas inteligentes.

**(c) Exemplos:**
- **MYCIN**: sistema especialista para diagnóstico de infecções bacterianas
- **DENDRAL**: sistema especialista para identificação de moléculas orgânicas

---

### Exercício 7

**Pergunta:** O que é a Hipótese do Sistema de Símbolos Físicos? Qual é sua importância para a IA Simbólica?

**Resposta:** A Hipótese do Sistema de Símbolos Físicos é a tese fundamental da IA Simbólica, segundo a qual **um sistema inteligente pode ser construído manipulando símbolos físicos que representam conhecimento**. Sua importância está em três pontos:

1. Fornece uma base teórica para a construção de sistemas de IA
2. Estabelece uma equivalência conceitual entre a mente humana e máquinas — segundo essa visão, a mente humana também seria um sistema de símbolos físicos
3. Define o programa de pesquisa da IA Clássica: produzir inteligência por meio de manipulação simbólica

---

### Exercício 8

**Pergunta:** Descreva dois benefícios e duas limitações da IA Simbólica, justificando cada item com exemplos concretos.

**Resposta:**

**Benefícios:**

1. **Interpretabilidade:** Por usar símbolos e regras compreensíveis, é possível auditar o raciocínio do sistema. Por exemplo, no MYCIN, é possível rastrear exatamente quais regras levaram a um diagnóstico.
2. **Raciocínio lógico transparente:** O sistema deduz novas informações a partir de regras explícitas, permitindo justificar cada conclusão (importante em aplicações jurídicas e médicas).

**Limitações:**

1. **Dificuldade em formalizar conhecimento do mundo real:** Conhecimento de senso comum é difícil de codificar. Por exemplo, formalizar regras como "não coloque o pé na mesa" requer um número impraticável de regras de contexto.
2. **Não aprende a partir de dados:** O sistema precisa ser reprogramado para cada nova situação. Um sistema simbólico de diagnóstico não consegue aprender automaticamente novos padrões a partir de novos casos clínicos, ao contrário de uma rede neural.

---

### Exercício 9

**Pergunta:** Caracterize a IA Conexionista, explicando: (a) sua inspiração; (b) como o conhecimento é representado e adquirido; (c) por que ganhou destaque a partir dos anos 1980.

**Resposta:**

**(a) Inspiração:** A IA Conexionista se inspira na estrutura do cérebro humano, modelando redes de neurônios artificiais conectados por sinapses (pesos).

**(b) Representação e aquisição do conhecimento:** O conhecimento é representado de forma **distribuída** nos pesos das conexões entre os neurônios artificiais. Ele é **adquirido por aprendizado**: o sistema é alimentado com dados, algoritmos ajustam os pesos, e a rede passa a reconhecer padrões e fazer previsões.

**(c) Razões para destaque a partir dos anos 1980:**
- Surgimento de computadores mais potentes
- Maior capacidade de processamento de grandes volumes de dados
- Sinergia entre avanços em hardware e novos algoritmos de treinamento

---

### Exercício 10

**Pergunta:** Identifique e explique duas vantagens e duas desvantagens da IA Conexionista.

**Resposta:**

**Vantagens:**

1. **Aprendizado adaptativo e generalização:** Aprende com exemplos e aplica o conhecimento a situações novas, sendo excelente em reconhecimento de padrões em imagens, sons e textos. Isso explica seu sucesso em visão computacional e processamento de linguagem natural.
2. **Processamento paralelo:** Múltiplas unidades operam simultaneamente, permitindo lidar com grandes volumes de dados de forma eficiente.

**Desvantagens:**

1. **Caixa-preta (baixa interpretabilidade):** É difícil explicar por que a rede tomou determinada decisão, o que gera problemas em áreas que exigem auditoria, como medicina e direito.
2. **Alto custo computacional e necessidade de dados extensos:** Treinar redes neurais profundas exige enormes conjuntos de dados rotulados e infraestrutura cara, o que limita a aplicação em domínios com poucos dados disponíveis.

---

## Nível Avançado

### Exercício 11

**Pergunta:** Para cada um dos sistemas a seguir, indique qual abordagem (simbólica, conexionista ou híbrida) caracteriza predominantemente seu funcionamento e justifique sua resposta:

a) IBM Watson  
b) Tesla Autopilot  
c) AlphaGo  
d) ChatGPT

**Resposta:**

**a) IBM Watson — Híbrida:** Combina elementos das duas abordagens. Utiliza redes neurais para compreensão de linguagem natural (PLN — componente conexionista) e aplica regras lógicas e raciocínio simbólico para inferência sobre dados estruturados e não estruturados.

**b) Tesla Autopilot — Conexionista:** Predominantemente baseado em redes neurais profundas que processam informações de sensores e câmeras. Utiliza aprendizado supervisionado para condução autônoma, sendo um caso de IA estreita com aprendizado profundo.

**c) AlphaGo — Conexionista (com elementos híbridos):** Combina aprendizado por reforço com redes neurais profundas. Aprendeu estratégias jogando milhões de partidas contra si mesmo, sem regras explícitas programadas. Embora a busca em árvore (Monte Carlo Tree Search) tenha caráter algorítmico, o componente que avalia posições e escolhe jogadas é conexionista.

**d) ChatGPT — Conexionista:** Modelo de linguagem baseado em redes neurais profundas (deep learning), treinado com enormes volumes de texto. Gera respostas coerentes sem regras linguísticas explícitas, sendo um caso paradigmático de abordagem puramente conexionista em larga escala.

---

### Exercício 12 — Estudo de Caso

**Pergunta:** Você é contratado por uma empresa que precisa desenvolver dois sistemas de IA:

- **Problema A:** Sistema para diagnosticar doenças raras com base em sintomas descritos textualmente por médicos. É necessário que o sistema **justifique suas decisões passo a passo**, indicando quais regras e evidências levaram ao diagnóstico. Há **poucos dados históricos disponíveis**.

- **Problema B:** Sistema para identificar se uma radiografia apresenta indícios de câncer. Há um **grande banco de dados** com milhares de imagens já diagnosticadas por especialistas. **Não é necessário** que o sistema explique suas decisões, apenas que tenha alta precisão.

Para cada problema, indique qual abordagem seria mais adequada e justifique.

**Resposta:**

**Problema A — Abordagem Simbólica (ou Híbrida com forte componente simbólico):**

Justificativa:
- A **necessidade de justificar decisões passo a passo** é o fator decisivo. A abordagem simbólica oferece interpretabilidade nativa: cada regra aplicada e cada evidência considerada podem ser auditadas.
- A **escassez de dados históricos** desfavorece a abordagem conexionista, que exige grandes volumes de exemplos para um treinamento eficaz.
- Sistemas especialistas (como o MYCIN) são exatamente o tipo de solução adequada para esse cenário: codificam o conhecimento de especialistas em regras lógicas e produzem diagnósticos auditáveis.

**Problema B — Abordagem Conexionista:**

Justificativa:
- A **disponibilidade de grandes volumes de dados rotulados** (milhares de imagens diagnosticadas) é exatamente o cenário ideal para redes neurais profundas, especialmente redes convolucionais (CNNs), aplicadas em diagnóstico por imagem.
- A **dispensa de explicabilidade** elimina a maior limitação da abordagem conexionista (caixa-preta).
- Reconhecimento de padrões em imagens médicas é uma das áreas em que a IA Conexionista historicamente supera abordagens simbólicas, pois é difícil formalizar em regras o que distingue uma imagem com câncer de uma sem.

---

### Exercício 13

**Pergunta:** Explique o que são abordagens neuro-simbólicas e por que representam uma tendência atual da pesquisa em IA.

**Resposta:** As abordagens **neuro-simbólicas** combinam características das duas tradições históricas, buscando obter o melhor de ambos os paradigmas:

- **Componente conexionista (redes neurais):** responsável pela **percepção e reconhecimento de padrões** em dados não estruturados (imagens, sons, texto bruto). Aproveita a capacidade de aprendizado a partir de grandes volumes de dados.
- **Componente simbólico (regras e símbolos):** responsável pelo **raciocínio lógico e geração de explicações**. Permite que o sistema justifique suas decisões e manipule conhecimento estruturado.

**Por que é tendência:**

1. **Robustez:** sistemas puramente conexionistas falham em tarefas que exigem raciocínio explícito; sistemas puramente simbólicos falham em percepção. A combinação supera ambas as limitações.
2. **Interpretabilidade:** a crescente exigência regulatória por explicabilidade (ex.: GDPR na Europa) torna a "caixa-preta" das redes neurais um obstáculo. O componente simbólico oferece transparência.
3. **Eficiência em dados:** a integração de regras pode reduzir a quantidade de dados necessária para o treinamento, pois parte do conhecimento já vem codificada.
4. **Capacidade ampliada:** sistemas híbridos podem realizar tarefas que nenhuma abordagem isolada conseguiria — combinando percepção e raciocínio em um pipeline coerente.

---

### Exercício 14 — Discursivo

**Pergunta:** Avalie criticamente a afirmação: *"A IA Conexionista, por aprender automaticamente, é sempre superior à IA Simbólica."*

**Resposta:** A afirmação é **incorreta** e simplifica indevidamente a relação entre as duas abordagens. Embora a IA Conexionista tenha alcançado resultados notáveis em áreas como visão computacional e processamento de linguagem natural, ela apresenta limitações que tornam a IA Simbólica preferível em diversos contextos:

1. **Domínios com poucos dados:** redes neurais exigem grandes volumes de dados rotulados. Em problemas com dados escassos (doenças raras, conhecimento jurídico especializado), a abordagem simbólica é mais eficiente.

2. **Necessidade de explicabilidade:** em medicina, direito, finanças e governo, a auditabilidade das decisões é essencial. A IA Simbólica oferece interpretabilidade nativa, enquanto a IA Conexionista é uma "caixa-preta".

3. **Raciocínio lógico estruturado:** problemas que exigem dedução formal (prova de teoremas, verificação de software, sistemas de regras de negócio) são naturalmente abordados pela IA Simbólica.

4. **Custo computacional:** sistemas conexionistas demandam infraestrutura cara para treinamento, o que pode ser inviável em pequenas empresas ou aplicações embarcadas.

Por isso, a comunidade científica reconhece atualmente que **as duas abordagens são complementares**, e a tendência é justamente integrá-las em sistemas híbridos (neuro-simbólicos), aproveitando as forças de cada uma conforme o problema exige.
