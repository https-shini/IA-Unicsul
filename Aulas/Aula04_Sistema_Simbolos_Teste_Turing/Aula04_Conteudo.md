# Aula 04 – O Sistema de Símbolos Físicos e o Teste de Turing

> Material de estudo estruturado a partir do conteúdo da aula, organizado para consulta, revisão e aprofundamento.

---

## Sumário

1. [Por que Estudar Esses Dois Temas Juntos?](#1-por-que-estudar-esses-dois-temas-juntos)
2. [O que é um Sistema de Símbolos Físicos?](#2-o-que-é-um-sistema-de-símbolos-físicos)
3. [A Hipótese do Sistema de Símbolos Físicos (HSSF)](#3-a-hipótese-do-sistema-de-símbolos-físicos-hssf)
4. [Os Dois Componentes Fundamentais da HSSF](#4-os-dois-componentes-fundamentais-da-hssf)
5. [As Cinco Etapas de Formação da Hipótese](#5-as-cinco-etapas-de-formação-da-hipótese)
6. [LISP: A Linguagem da IA Simbólica](#6-lisp-a-linguagem-da-ia-simbólica)
7. [Exemplo Clássico: SHRDLU](#7-exemplo-clássico-shrdlu)
8. [Sistemas Especialistas: Aplicação Comercial da HSSF](#8-sistemas-especialistas-aplicação-comercial-da-hssf)
9. [Limitações e Críticas ao Paradigma Simbólico](#9-limitações-e-críticas-ao-paradigma-simbólico)
10. [Transição: Do Símbolo ao Comportamento](#10-transição-do-símbolo-ao-comportamento)
11. [Alan Turing: O Homem por Trás do Teste](#11-alan-turing-o-homem-por-trás-do-teste)
12. [O Problema de Partida do Teste de Turing](#12-o-problema-de-partida-do-teste-de-turing)
13. [O Jogo da Imitação (Versão Original)](#13-o-jogo-da-imitação-versão-original)
14. [O Teste de Turing (Versão Moderna)](#14-o-teste-de-turing-versão-moderna)
15. [O Teste Não é Sobre Verdade, é Sobre Semelhança](#15-o-teste-não-é-sobre-verdade-é-sobre-semelhança)
16. [Antecipações Históricas do Teste](#16-antecipações-históricas-do-teste)
17. [Primeiras Implementações: ELIZA (1966)](#17-primeiras-implementações-eliza-1966)
18. [A Crítica Fundamental: A Sala Chinesa (1980)](#18-a-crítica-fundamental-a-sala-chinesa-1980)
19. [O Que o Teste de Turing Não É](#19-o-que-o-teste-de-turing-não-é)
20. [Hierarquia de Testes de Turing](#20-hierarquia-de-testes-de-turing)
21. [Turing e IA Forte: Uma Associação Controversa](#21-turing-e-ia-forte-uma-associação-controversa)
22. [Relevância Contemporânea do Teste de Turing](#22-relevância-contemporânea-do-teste-de-turing)

---

## Parte I – O Sistema de Símbolos Físicos

---

### 1. Por que Estudar Esses Dois Temas Juntos?

O **Sistema de Símbolos Físicos** e o **Teste de Turing** são os dois pilares conceituais que definem o programa de pesquisa da IA Clássica.

| Conceito | Autores | Pergunta que responde |
|---|---|---|
| Sistema de Símbolos Físicos | Newell e Simon (1976) | *Como* a inteligência pode ser implementada? |
| Teste de Turing | Alan Turing (1950) | *Como saber se* uma máquina é inteligente? |

Juntos, esses dois frameworks formam a base teórica e metodológica da IA Simbólica e permanecem referências obrigatórias no campo.

---

### 2. O que é um Sistema de Símbolos Físicos?

Segundo Newell e Simon, um **Sistema de Símbolos Físicos** é composto por entidades que são padrões físicos, como bits, marcas no papel ou estados elétricos, que podem ser combinados para formar estruturas mais complexas, como expressões, listas e árvores. O sistema possui processos capazes de operar sobre essas estruturas.

- **"Físico":** pode ser realizado por qualquer matéria, seja silício, neurônios ou engrenagens.
- **"Símbolo":** padrão que se refere a algo, denotando um objeto, propriedade ou relação.

---

### 3. A Hipótese do Sistema de Símbolos Físicos (HSSF)

> *"Um sistema de símbolos físicos possui os meios necessários e suficientes para a ação inteligente geral."*
> — Newell e Simon, 1976

A HSSF é a tese central da ciência cognitiva clássica e possui duas afirmações complementares:

- **Necessário:** todo sistema inteligente, seja humano, alienígena ou artificial, é ou realiza um sistema de símbolos físicos.
- **Suficiente:** qualquer sistema de símbolos físicos de tamanho adequado pode ser organizado para exibir inteligência geral.

> **Implicação radical:** a inteligência não depende de biologia, carbono ou consciência. Ela depende apenas da arquitetura correta de processamento de símbolos.

---

### 4. Os Dois Componentes Fundamentais da HSSF

**Estruturas de Símbolos**
Combinações de símbolos relacionados que permitem representar conhecimento de forma hierárquica. Exemplo: `(gato → mamífero → tem_pelo)`.

**Processos de Operação**
Operações capazes de criar, modificar, copiar, comparar e destruir estruturas. A inteligência emerge da aplicação correta desses processos sobre as estruturas adequadas.

---

### 5. As Cinco Etapas de Formação da Hipótese

Newell e Simon identificaram cinco estágios históricos que culminaram na HSSF:

| Etapa | Marco | Contribuição |
|---|---|---|
| 1 | Leibniz, Boole, Frege, Russell | Criação de linguagens simbólicas artificiais, substituindo a linguagem natural por cálculo formal |
| 2 | Máquina de Turing (1936) | Modelo abstrato de processador de símbolos, provando que um dispositivo pode executar qualquer computação |
| 3 | Programa Armazenado de Von Neumann (1945) | Programas passam a ser dados, permitindo que o computador modifique seu próprio código |
| 4 | Processamento de Listas por Newell e Simon (1956) | Criação de estruturas de dados dinâmicas; marco zero da IA com o programa Logic Theorist |
| 5 | LISP por McCarthy (1958) | Primeira linguagem projetada para processamento de símbolos, dominando a IA por mais de 30 anos |

---

### 6. LISP: A Linguagem da IA Simbólica

Criada por John McCarthy em 1958, **LISP** (LISt Processing) foi revolucionária por quatro características centrais:

- **Código = Dados:** programas podem escrever outros programas.
- **Recursão:** estrutura fundamental de controle de fluxo.
- **Gerenciamento automático de memória** com coleta de lixo (garbage collector).
- **Simbolismo puro:** toda estrutura é uma lista de símbolos.

LISP dominou a pesquisa em IA dos anos 1960 até os anos 1990.

---

### 7. Exemplo Clássico: SHRDLU

**SHRDLU** (Terry Winograd, 1968-1970) foi um programa que operava em um "mundo dos blocos" virtual. O usuário interagia em inglês natural com o sistema, e o SHRDLU compreendia os comandos, planejava ações, executava e respondia de forma coerente.

O programa demonstrou a aplicação prática da HSSF: símbolos representavam objetos físicos, e operações sobre esses símbolos produziam comportamento aparentemente inteligente.

---

### 8. Sistemas Especialistas: Aplicação Comercial da HSSF

Os sistemas especialistas foram a aplicação comercial mais bem-sucedida da HSSF:

| Sistema | Ano | Domínio | Resultado |
|---|---|---|---|
| DENDRAL | 1965 | Química orgânica | Identificava moléculas a partir de espectrometria de massa, superando estudantes de doutorado |
| MYCIN | 1972 | Medicina | Diagnosticava infecções bacterianas com precisão superior à de médicos juniores e explicava seu raciocínio |

---

### 9. Limitações e Críticas ao Paradigma Simbólico

Apesar dos sucessos, a HSSF enfrentou cinco problemas fundamentais:

1. **Problema da Formalização:** o conhecimento de senso comum não é facilmente representável em regras explícitas.
2. **Combinação Explosiva:** o número de regras necessárias cresce exponencialmente, tornando os sistemas lentos e frágeis.
3. **Aquisição de Conhecimento:** extrair conhecimento de especialistas humanos é caro e demorado, fenômeno conhecido como "gargalo do conhecimento".
4. **Incerteza e Ambiguidade:** a lógica clássica exige verdadeiro ou falso, enquanto o mundo real é probabilístico e vago.
5. **Ausência de Aprendizado:** sistemas simbólicos não aprendem com dados e precisam ser reprogramados para cada nova situação.

---

### 10. Transição: Do Símbolo ao Comportamento

Enquanto Newell e Simon propuseram uma **arquitetura** para a inteligência por meio da HSSF, Alan Turing propôs um **critério** para identificá-la por meio do Teste de Turing. Ambas as contribuições respondem à mesma pergunta fundadora da IA: "As máquinas podem pensar?" e definiram a agenda de pesquisa do campo ao longo de todo o século XX.

---

## Parte II – O Teste de Turing

---

### 11. Alan Turing: O Homem por Trás do Teste

**Alan Turing (1912-1954)** foi matemático, lógico e criptoanalista, considerado o pai da computação moderna. Em 1950, publicou o artigo *"Computing Machinery and Intelligence"*, no qual propôs o Teste de Turing como uma alternativa operacional à pergunta filosófica sobre o pensamento das máquinas.

---

### 12. O Problema de Partida do Teste de Turing

Turing considerava a pergunta "As máquinas podem pensar?" vaga, subjetiva e filosoficamente intratável. Para evitar um debate sem solução, ele a substituiu por uma pergunta operacional e objetiva:

> *"Há como imaginar um computador digital que faria bem o jogo da imitação?"*

Essa reformulação deslocou o problema da filosofia da mente para o campo do comportamento observável.

---

### 13. O Jogo da Imitação (Versão Original)

O experimento original envolvia três participantes em salas separadas, comunicando-se exclusivamente por texto:

| Participante | Papel |
|---|---|
| Interrogador (J) | Humano que faz perguntas |
| Humano (A) | Responde naturalmente |
| Máquina (B) | Tenta se passar por humano |

Se a máquina enganasse o interrogador com frequência comparável à de um humano, Turing considerava que ela demonstrava comportamento inteligente.

---

### 14. O Teste de Turing (Versão Moderna)

Turing simplificou o experimento para a interação direta entre um julgador humano e um computador. A condição de aprovação era clara:

> *"Se um computador for capaz de enganar um terço de seus interlocutores, fazendo-os acreditar que ele é um ser humano, então estaria pensando por si próprio."*

**Ponto central:** o teste não exige respostas corretas, mas respostas indistinguíveis das de um humano. A máquina pode mentir, hesitar ou errar, exatamente como um humano faria.

---

### 15. O Teste Não é Sobre Verdade, é Sobre Semelhança

Um exemplo clássico de Turing ilustra esse princípio: se questionada sobre um cálculo complexo, uma máquina verdadeiramente "inteligente" hesitaria ou apresentaria uma resposta aproximada, imitando o comportamento humano, em vez de responder de forma instantânea e precisa, o que a denunciaria imediatamente como uma máquina.

---

### 16. Antecipações Históricas do Teste

A ideia central do Teste de Turing foi antecipada por pensadores de séculos anteriores:

- **René Descartes (1637):** já utilizava a resposta linguística apropriada como critério para distinguir um humano de um autômato.
- **Denis Diderot (1746):** antecipou o critério comportamental ao sugerir que um papagaio capaz de responder a qualquer questão deveria ser considerado inteligente.

---

### 17. Primeiras Implementações: ELIZA (1966)

**ELIZA**, desenvolvida por Joseph Weizenbaum, analisava as mensagens do usuário, identificava palavras-chave e retornava respostas genéricas ou reformulava as frases do próprio usuário como perguntas. Muitos usuários acreditavam estar conversando com um ser humano.

O programa é frequentemente citado como o primeiro a despertar o debate sobre aprovação no Teste de Turing, embora sua classificação nesse sentido seja controversa.

---

### 18. A Crítica Fundamental: A Sala Chinesa (1980)

Proposta por **John Searle**, a **Sala Chinesa** é o experimento mental mais influente contra o Teste de Turing como critério de inteligência:

**O cenário:** um homem que não compreende chinês está trancado em uma sala. Ele recebe símbolos chineses do lado de fora e, seguindo um livro de regras detalhado, devolve respostas em chinês. Para quem está fora da sala, parece que alguém entende a língua. Dentro da sala, ninguém entende nada.

**A tese de Searle:** simular respostas corretas não implica compreensão real nem consciência do conteúdo. Passar no Teste de Turing demonstra apenas que a máquina simula comportamento inteligente, não que ela compreende ou pensa.

> A crítica é dirigida especificamente à **IA Forte**: a afirmação de que uma máquina poderia genuinamente pensar. Para Searle, simulação não é duplicação.

---

### 19. O Que o Teste de Turing Não É

É importante delimitar o escopo correto do teste:

- **Não é uma definição de inteligência.** É um substituto operacional para uma pergunta filosófica mal definida.
- **Não prova que a máquina pensa.** A Sala Chinesa demonstra que isso é controverso, e o próprio Turing antecipou objeções semelhantes.
- **Não é sobre respostas corretas.** É sobre respostas indistinguíveis das humanas.
- **Não está ultrapassado.** Continua sendo referência central em filosofia da IA e inspirou diversas variações e hierarquias.

---

### 20. Hierarquia de Testes de Turing

Filósofos como **David Chalmers** propuseram uma hierarquia de níveis de indistinguibilidade entre máquina e humano:

| Nível | Nome | Descrição |
|---|---|---|
| T1 | Subtarefa | Indistinguibilidade em uma tarefa específica, como jogar xadrez |
| T2 | Simbólico | O teste original: conversa textual irrestrita (vulnerável à Sala Chinesa) |
| T3 | Total (Robótico) | Máquina com corpo, sensores e atuadores, interagindo com o mundo físico |
| T4 | Microfunção | Indistinguibilidade em nível neuronal |
| T5 | Completo | Indistinguibilidade em todo aspecto empiricamente discernível |

O nível **T3 (Robótico)** é considerado o alvo mais adequado para a pesquisa em IA e ciência cognitiva: suficientemente abrangente para ser significativo e suficientemente concreto para ser investigado.

---

### 21. Turing e IA Forte: Uma Associação Controversa

A associação do artigo de Turing à defesa da IA Forte é questionada por pesquisadores contemporâneos. Segundo Patrick Goutefangea (2017), Turing não exigiu que a máquina tivesse mente ou consciência, mas apenas que simulasse a informalidade característica do comportamento humano.

Nessa leitura, Turing seria, na verdade, um teórico da **IA Fraca**, propondo que uma máquina poderia passar no teste por meio de um processo de aprendizado e adaptação, não por programação direta de conhecimento.

---

### 22. Relevância Contemporânea do Teste de Turing

O Teste de Turing permanece uma referência ativa no debate sobre inteligência artificial. O surgimento de grandes modelos de linguagem, como o ChatGPT, reacendeu a discussão, uma vez que muitos usuários são enganados diariamente em interações textuais.

A conclusão predominante na filosofia contemporânea é que o Teste de Turing **não é a definição final de inteligência**, mas constitui um **marco zero indispensável**: toda discussão séria sobre IA começa com Turing.

---

*Material organizado para a disciplina de Fundamentos de Inteligência Artificial — Ciência da Computação, Universidade Cruzeiro do Sul.*
