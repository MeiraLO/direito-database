# Definição e Análise Modal

_Baseado em Beyleveld & Brownsword, "Human Dignity in Bioethics and Biolaw"_

---

## Parte I — Sentido Estrito vs. Sentido Amplo

### 1.1 Sentido Estrito

O texto oferece **duas versões** de sentido estrito, que convergem no mesmo critério: **capacidade atual de agência**, não pertencimento à espécie ou potencialidade.

**(a) Forma fechada (cap. 2 — dignidade como restrição)**

Dentro da fórmula "todos-portadores-de-direitos-humanos", a leitura fechada restringe a titularidade a quem **já exerce de fato** a capacidade de operar seus próprios direitos. Exclui:

- Quem ainda não desenvolveu a capacidade (fetos, embriões, crianças pequenas);
- Quem a perdeu (estado vegetativo, certos quadros de demência avançada);
- Quem tem apenas potencial futuro de tê-la.

**(b) Sentido kantiano (cap. 3)**

Para Kant, dignidade em sentido estrito é qualificada pela **capacidade moral racional** — a aptidão de reconhecer e seguir o imperativo categórico. Não é a vida em si que tem valor intrínseco, mas a racionalidade prática. Esse critério, levado a rigor, ameaça excluir animais, crianças e pessoas com deficiência intelectual.

**(c) Base comum do PGC (cap. 4)** — que os autores tratam como _princípio supremo_:

> Dig_estrito(x) ↔ A(x)

onde `A(x) = "x é agente atual"` (age com propósito, valor e voluntariedade). Dignidade em sentido estrito, nesta leitura, é **coextensiva com agência efetiva**, e é essa a definição usada como padrão de análise do livro.

**(d) Sentido positivado — constitucional e internacional (introdução e cap. 2)**

Além da fundamentação filosófica (PGC ou kantiana), o sentido estrito também corresponde à dignidade tal como **positivada em norma jurídica vinculante**, e não apenas discutida em teoria:

- **Constitucional**: no ordenamento brasileiro, o art. 1º, III, da CF/88 eleva a dignidade da pessoa humana a **fundamento da República** — não é um princípio moral flutuante, mas norma jurídica cogente, vetor interpretativo de todo o sistema, inclusive do art. 5º, _caput_, e dos direitos fundamentais.
- **Internacional**: a Declaração Universal dos Direitos Humanos (ONU, 1948) abre seu preâmbulo e art. 1º reconhecendo a dignidade inerente a todos os membros da família humana como fundamento da liberdade, da justiça e da paz; os Pactos Internacionais de 1966 (Direitos Civis e Políticos; Direitos Econômicos, Sociais e Culturais) repetem a fórmula em seus preâmbulos.
- **Biodireito específico**: o próprio livro situa a bioética moderna a partir do Código de Nuremberg (1947) e da Declaração de Helsinki (1964) — instrumentos que positivam exatamente a versão de dignidade-como-restrição (consentimento informado, proibição de submissão sem vontade) —, linhagem que mais tarde alimenta instrumentos da UNESCO (Declaração Universal sobre o Genoma Humano, 1997; Declaração Universal sobre Bioética e Direitos Humanos, 2005).

Esse sentido positivado **não é uma quarta teoria concorrente** com o PGC e Kant — é o que os próprios autores chamam, já na introdução, de vertente "restrição" quando **positivada** (o texto menciona isso expressamente ao falar da visão adotada pelo Conselho Europeu de Direitos Humanos e Biodireito). Em outras palavras: a positivação constitucional e internacional é o **veículo jurídico** pelo qual a dignidade em sentido estrito (fechado/PGC) deixa de ser apenas princípio moral e passa a ser direito vinculante e exigível.

### 1.2 Sentido Amplo (contraponto)

Basta **ser humano** — independentemente de exercer, ter exercido ou ser capaz de exercer agência — para ser titular de dignidade. Aparece em três formas no texto:

- **Empoderamento** (cap. 1): dignidade = autonomia potencial de qualquer humano;
- **Restrição comunitária** (cap. 2, versão aberta): status humano basta, com valores positivados pela comunidade;
- **Dignidade-virtude** (cap. 6): dignidade como postura/caráter, atribuível mesmo a não-agentes por meio do **princípio da proporcionalidade** (agentes parciais têm direitos genéricos na proporção em que se aproximam da agência plena).


---

## Parte II — Análise Modal da Afirmação

> **"O tratamento imposto contra a vontade do paciente capaz caracteriza paternalismo médico, incompatível com a dignidade humana em sentido estrito."**

### 2.1 Aparato formal

- **A(x)**: x é agente atual (base do sentido estrito, item 1.1c)
- **W(x,¬T)**: x manifesta vontade contrária ao tratamento T
- **Imp(T,x)**: T é imposto a x
- **Pat**: Imp(T,x) ∧ W(x,¬T) — caracteriza paternalismo médico
- **R(x)**: x é titular de direitos genéricos (PGC)
- **□d**: necessidade dialética — P é □d quando negá-la implica autocontradição performativa de quem se afirma agente (não é necessidade metafísica clássica, é necessidade indexada à autocompreensão prática do agente)
- **◇**: possibilidade — P é ◇ quando compatível, sem contradição, com ser agente

### 2.2 Leitura A — Sentido estrito = PGC (fechado)

Usando a definição de 1.1(c) e os teoremas do PGC já estabelecidos no livro:

```
1. Dig_estrito(x) ↔ A(x)                              [def. 1.1c]
2. A(x) → □d R(x)                                      [teorema do PGC, cap. 4]
3. R(x) → □d (∀T)(W(x,¬T) → ¬Imp(T,x))                 [will conception — pontos 7/7']
```

Derivação, partindo da premissa fática "paciente capaz" → A(x):

```
A(x)                                    (premissa)
Dig_estrito(x)                          [por 1]
□d R(x)                                 [por 2]
□d (W(x,¬T) → ¬Imp(T,x))                [por 3]
```

O paternalismo (Imp(T,x) ∧ W(x,¬T)) é exatamente a negação do consequente necessário acima. Logo:

```
□d ¬(A(x) ∧ W(x,¬T) ∧ Imp(T,x))
```

**Conclusão A:** a incompatibilidade não é apenas verdadeira — é **dialeticamente necessária**. Negá-la equivaleria a negar que x é agente, contradizendo a própria premissa ("paciente capaz").

### 2.3 Leitura B — Sentido estrito = kantiano (dever-para-consigo-mesmo)

```
1'. Dig_estrito_K(x) ↔ CapMoral(x)                     [def. 1.1b]
2'. Deveres perfeitos consigo mesmo NÃO são renunciáveis pela vontade momentânea (Willkür) — diferente do PGC, que permite renúncia dos direitos genéricos (cap. 5)
```

Aqui, W(x,¬T) — vontade empírica momentânea — **não coincide** com a vontade racional autolegisladora (Wille) que fundamenta a dignidade kantiana. Logo é **possível**, sem contradição, que uma imposição contrária à vontade empírica seja compatível com — ou até exigida por — essa dignidade (mesma lógica do exemplo dos "atiradores de anões"):

```
◇ (CapMoral(x) ∧ W(x,¬T) ∧ Imp(T,x))
```

**Conclusão B:** sob esta leitura, a incompatibilidade é apenas **contingente** (◇), não necessária — pode ser verdadeira ou falsa a depender do caso.

### 2.4 Leitura C — Sentido estrito positivado (constitucional/internacional)

Aqui o operador não é dialético, mas **deôntico**: **O** = "é juridicamente obrigatório" (segundo direito positivo vigente, e não segundo pura estrutura conceitual da agência).

```
4. CF/88, art. 1º, III + art. 5º, caput → O(¬Imp(T,x) | W(x,¬T))     [consentimento informado como norma cogente]
5. DUDH/1948, art. 1º + Nuremberg (1947) + Helsinki (1964) → mesma obrigação, em plano internacional
```

Isto é, a positivação (item 1.1d) não deduz a incompatibilidade de uma estrutura lógica da agência — ela a **impõe diretamente como norma vinculante**, com sanção jurídica própria:

```
O ¬(A(x) ∧ W(x,¬T) ∧ Imp(T,x))
```

**Conclusão C:** o mesmo resultado da Leitura A é alcançado por via distinta — não pela necessidade dialética intrínseca ao conceito de agência, mas pela **obrigatoriedade jurídica** decorrente da positivação constitucional e internacional da dignidade. As duas necessidades (□d e O) **convergem**, mas por fundamentos diferentes: uma é conceitual/moral (PGC), a outra é normativa/institucional (direito positivo).

### 2.5 Veredito final

A frase contém uma ambiguidade de escopo no termo "sentido estrito". Mas, considerando que o **sentido estrito relevante no livro é o do PGC** (cap. 4, tratado pelos autores como princípio supremo da bioética/biodireito) — e que essa mesma leitura é a que se encontra **positivada** tanto na Constituição (art. 1º, III, e art. 5º) quanto nos instrumentos das Nações Unidas (DUDH/1948, Pactos de 1966, Nuremberg, Helsinki) —, a leitura correta é a **Leitura A, reforçada pela Leitura C**:

> **A afirmação é verdadeira, e é ao mesmo tempo dialeticamente necessária e juridicamente obrigatória:**
> 
> ```
> A(x) ∧ W(x,¬T) ∧ Imp(T,x)  ⊢  □d ¬Dig_estrito(x)  ∧  O ¬Dig_estrito(x)
> ```

Isso confirma a metáfora da "espada de dois gumes" da introdução do livro: o mesmo aparato que empodera o paciente capaz torna qualquer imposição contrária à sua vontade uma **contradição estrutural** dentro do sistema PGC **e**, simultaneamente, uma **violação normativa** do direito positivo vigente — não é uma questão de grau, política pública ou ponderação, mas uma impossibilidade lógica _e_ uma ilicitude jurídica convergindo sobre o mesmo caso.