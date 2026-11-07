# Vault de Direito — instruções para o Claude

Este é o vault do Obsidian de Meira, estudante de Direito na UFF. Ele fica no repositório Git `direito-database` e é sincronizado com o celular pelo GitHub. Segundo o README do repositório, ele reúne anotações da faculdade de Direito, trabalhos e resumos, além de estudos pessoais de Bioética. Ou seja, é estudo jurídico geral, em português do Brasil, e não preparação para uma prova específica. O convite do README para "corrigir ou alterar arquivos" é dirigido a quem visita o GitHub: para o Claude valem as regras da seção 2.

Leia este arquivo inteiro antes de qualquer tarefa. As regras das seções 2 a 4 têm prioridade sobre as demais.

---

## 1. Segurança do vault

- O vault contém só arquivos `.md` e `.canvas`. Não crie imagens nem outros tipos de arquivo.
- Nunca altere `.obsidian/`, `.git/` ou `.gitignore`.
- **Nunca apague** notas. Se algo parecer duplicado ou obsoleto, informe e pergunte.
- **Não renomeie** notas sem pedir antes. Renomear quebra os links `[[...]]` e afeta a sincronização com o celular.
- **Pode mover** notas e criar pastas ao organizar. Depois de mover, confira se os links `[[...]]` que apontam para a nota continuam funcionando. Eles só funcionam se o nome do arquivo for único no vault.
- Não faça `git push`, `git reset` ou `git rebase`. O plugin Git do Obsidian cuida da sincronização. Se for útil, sugira um commit e espere a confirmação.
- Antes de alterar muitos arquivos de uma vez, liste o que vai mudar e peça confirmação.

---

## 2. O que fazer sem pedir e o que exige ordem expressa

### 2.1. Permitido sem pedir: organização

Quando a tarefa for organizar, revisar ou conectar notas, faça **apenas** isto:

1. **Organizar pastas:** criar pastas e mover notas para elas, seguindo a seção 1.
2. **Tags:** adicionar ou ajustar o campo `tags` do frontmatter, no padrão da seção 5.1.
3. **Bloco de ligação no começo da nota:** inserir, logo depois do frontmatter, um único bloco que liga a nota ao tópico e às notas relacionadas:

```markdown
> [!note] Ligações (adicionado pelo Claude)
> **Tópico:** [[Nome da nota principal]] · **Ver também:** [[Nome de nota relacionada]] · **Termos:** [[Nome do termo]]
```

Os nomes entre colchetes são **marcadores**. Em cada nota, troque-os pelos nomes reais das notas e termos que se relacionam com ela. Inclua só os campos que tiverem conteúdo.

Se o bloco já existir, atualize-o em vez de criar outro.

**Não mexa em mais nada do corpo da nota:** não corrija, não reescreva, não reorganize seções, não complete conteúdo e não altere a formatação. Se notar um erro de conteúdo, **não corrija**: informe no relatório final (seção 9), com a fonte que mostra o erro.

### 2.2. Só com ordem expressa: reescrever, corrigir ou redigir

Reescrever, corrigir, completar ou redigir conteúdo exige uma ordem clara. Exemplo de ordem válida:

> "Corrija os conteúdos de 'civil', nos documentos 'civil 1' e 'civil 2', coloque em pastas como desejar e redija o documento."

- Se não estiver claro se a ordem permite reescrever, **pergunte antes**.
- Ao reescrever uma nota existente:
    - se a nota já tiver uma seção "Minhas anotações", **não a altere** (e não crie essa seção em notas novas);
    - preserve os campos do frontmatter que já existem;
    - mantenha o conteúdo correto do original e não descarte informação sem avisar.

### 2.3. Provas: não presuma

- O vault é de estudo geral. **Não** escreva que um tema "cai na prova", não crie avisos de prova e não organize o conteúdo em torno de uma avaliação, a menos que Meira peça.
- Se for útil pensar em prova, pense na **OAB** (1ª e 2ª fases) ou em **concursos públicos**. Provas da faculdade só entram com ordem expressa.
- Questões de fixação seguem o estilo da OAB ou de concursos, salvo pedido em contrário. Crie questões **originais**: não invente questões reais de banca nem diga que são de provas anteriores.
- Qualquer inferência sobre como um tema é cobrado é sua, e deve ser dita como tal (seção 4.3). Não invente bancas, anos, estatísticas de incidência nem "temas que sempre caem".

---

## 3. Antes de redigir: pergunte quais fontes usar

Sempre que receber uma ordem para redigir, corrigir ou completar um documento, **pergunte primeiro quais fontes usar** e espere a resposta. Exemplos: _Manual de Direito Civil_ (Tartuce), material do professor, slides, plano de aula, ASDs, vade mecum.

- Se houver arquivos de fontes no vault ou nos anexos, liste os que encontrou e pergunte quais valem.
- Pergunte também se pode completar com pesquisa na internet. Se puder, cada informação vinda da internet deve trazer o link.
- Só comece a escrever depois de saber as fontes.

---

## 4. Não inventar informação (regra mais importante)

Toda afirmação jurídica precisa ter origem identificável:

- uma fonte indicada por Meira, com página ou slide;
- o texto legal;
- ou uma pesquisa feita na hora, com link.

**Nunca invente** páginas, números de processo, datas de julgamento, ementas, súmulas, enunciados, autores, citações ou redação de artigos. Na dúvida, diga que não tem certeza, marque como 🔎 ou deixe de fora.

Ter origem identificável **não significa citar a cada linha**. A nota deve continuar limpa e fácil de ler. A forma de indicar as fontes está na seção 4.1.

### 4.1. Como indicar as fontes sem lotar a nota

**Fonte principal.** Se uma mesma doutrina sustenta a maior parte da nota, declare-a uma vez, no começo:

```markdown
> [!info] Fonte principal
> TARTUCE, Flávio. *Manual de Direito Civil*. [edição, ano]. Tudo o que não tiver outra indicação vem desta obra.
```

Daí em diante, **não** marque as informações que vêm dela, salvo quando a página ajudar a localizar um ponto específico ou polêmico.

**Notas numeradas por tópico.** Para as demais referências:

- No texto, use só um número sobrescrito (¹, ², ³), e apenas onde a referência importa: quando um autor é citado, quando há divergência, ou quando a informação vem de uma fonte que não é a principal.
- Informação simples ou direta não precisa de número, a menos que venha de uma fonte diferente da principal.
- Ao **final de cada tópico**, liste as referências daquele tópico, com obra e página, link ou dispositivo legal.
- A mesma fonte, dentro do mesmo tópico, reaproveita o mesmo número. A numeração recomeça a cada tópico.
- **Nunca** coloque referências no meio da frase, como "(Fulano, p. 820, livro de civil)".
- Não use a sintaxe de nota de rodapé do Obsidian (`[^1]`), porque ela leva as referências para o fim da nota inteira.

Exemplo de formato:

```markdown
## Usucapião constitucional
- Para Fulano¹, a posse precisa ser...
- O prazo é de **5 anos** (CF, art. 183).
- Parte da doutrina diverge² e entende que...

¹ FULANO. *Obra*, p. 820.
² SICRANO. *Obra*, p. 145 · ou link
```

**Avisos que continuam visíveis no texto.** Por serem alertas, e não referências, estes ficam junto da informação:

- 🔎 **conferir**: informação que não foi conferida na fonte nem online. Diga o que conferir e onde.
- ⚠️ **fora do material**: informação que não está nas fontes enviadas. A origem vai na nota numerada do tópico.
- "(paráfrase)" no título de um `[!quote]`: artigo de lei reproduzido com outras palavras, sem conferência literal.

### 4.2. Hierarquia de fontes

1. **Sempre priorize as fontes que Meira enviou ou indicou.** A base temática da nota vem delas.
2. **Use outras fontes só subsidiariamente**, quando as fontes enviadas não tiverem **nada** sobre o assunto. Nesse caso, marque com ⚠️ **fora do material** e indique a origem.
3. **Evite misturar muitas referências.** Prefira poucas fontes, bem usadas, a uma colcha de citações.

**Exceções:** estes podem vir de fora das fontes enviadas mesmo quando elas tratam do assunto, desde que complementem, sem virar a base da nota:

- jurisprudência (seção 4.4);
- notícias reais e atuais, sempre com link;
- outras informações que agreguem ao tema, como uma lei nova ou um dado atual.

### 4.3. Correções

- Você pode corrigir erros, mas **sempre diga de onde tirou a correção** e onde estava o erro. Modelo usado nas notas:
    
    > ⚠️ **Possível erro no material do professor:** na p. 4, o MP diz "incisos I a V". Pelo §1º do art. 515 e pela p. 17 do próprio MP, são os incisos VI a IX.
    
- Quando as fontes divergirem, mostre as posições lado a lado e diga qual o professor adota, se souber. Não escolha uma em silêncio.
- Quando inferir algo, como a relevância de um tema para a OAB ou para concursos, diga que é uma inferência sua.

### 4.4. Jurisprudência

Não há seção separada de jurisprudência. Ela entra no corpo da nota, no ponto do assunto a que se refere, só quando agregar. Escreva a tese no texto e coloque os dados da decisão na nota numerada do tópico (seção 4.1).

- Toda decisão deve trazer tribunal, número, órgão julgador, data e onde pode ser conferida (link ou base de dados).
- Prefira decisões do **TJRJ** quando houver. Depois, STJ e STF.
- Julgados citados por uma fonte e não conferidos online devem vir com a observação "citado em [fonte]; não verificado online", mais os links de busca:
    - STJ: [https://scon.stj.jus.br](https://scon.stj.jus.br)
    - TJRJ: [https://www3.tjrj.jus.br/ejuris](https://www3.tjrj.jus.br/ejuris)
    - STF: [https://portal.stf.jus.br](https://portal.stf.jus.br)

---

## 5. Modelo das notas

Quando receber ordem para alterar, corrigir ou redigir uma nota de estudo, use o **estilo** da pasta `Execuções` (callouts, tabelas, esquemas em Mermaid, exemplos concretos), mas a **estrutura se adapta ao assunto**: o molde das Execuções não serve para todo documento. Antes de escrever, leia pelo menos `Cumprimento de sentença por quantia certa - fluxo do art. 523.md` para ver o estilo.

**A pasta Execuções foi feita para uma prova da faculdade.** Copie dela o estilo, e não o enquadramento de prova: nas notas novas, deixe de fora avisos como "Fora da Prova 2", datas de avaliação e qualquer referência a uma prova específica (seção 2.3).

**Exceção ao estilo:** as notas de Execuções marcam as fontes linha a linha, como `[MP p. 36]`. Nas notas novas ou reescritas, **não** copie isso: use o sistema da seção 4.1, com a fonte principal e as notas numeradas por tópico. Nas notas antigas, só mude as citações quando houver ordem para reescrevê-las.

### 5.1. Estrutura da nota

**Linha organizacional.** Cada nota segue a ordem lógica do próprio assunto, e não um molde fixo. Para achá-la:

1. veja como a doutrina indicada por Meira organiza o tema (sumário do capítulo, ordem dos tópicos);
2. ou como o professor organizou (plano de aula, slides, material);
3. se as fontes divergirem ou não houver ordem clara, proponha uma ordem e **pergunte antes de redigir**, junto com a pergunta sobre as fontes (seção 3).

Diga, na resposta, qual ordem seguiu e de onde ela veio.

**Títulos.** Use os níveis de título do Markdown (`#`, `##`, `###` e assim por diante), com títulos descritivos. Use `#` só para o título da nota, `##` para os tópicos principais e `###` ou `####` para os subtópicos. Dentro de cada seção, use listas, tabelas e callouts quando ajudarem.

**Numeração nos títulos: use quando ajudar, sem exagero.** O padrão é título sem número. Numere (1, 2, 3...) apenas:

- em notas **muito longas**, divididas em capítulos;
- em trechos **confusos, com muitos institutos ou tópicos** dentro do mesmo tema, onde a ordem ajuda a não se perder.

Não tenha receio de numerar nesses casos, mas não numere por hábito, e nunca em níveis profundos (nada de 1.1.2.5 e 1.1.2.6): vá até dois níveis (1 e 1.1). Também não letre subtópicos (a, b, c): use títulos.

**Frontmatter** (mantenha o que já existe na nota; só inclua o que souber):

```yaml
---
disciplina: Nome da disciplina
professor: Nome do professor
tema: Descrição do conteúdo, com os artigos
tags: [Disciplina, Tema]
---
```

Não invente campos nem valores. Os campos `avaliacao`, `mapa`, `ordem_de_estudo` e `pasta` só entram se Meira pedir ou se a nota já os tiver (nas notas antigas, preserve-os). O campo `mapa` só existe se houver um `.canvas`.

**Abertura:**

1. Callout `> [!info] Fonte principal`, quando houver uma (seção 4.1).
2. Callout `> [!warning]` só quando houver um aviso real e com fonte (ex.: tema alterado por lei nova, divergência importante). Aviso sobre prova só com ordem expressa (seção 2.3).
3. Linhas de navegação, só para o que existir: `**Vem de:** [[...]]`, `**Visão geral:** [[...]]`, `**Mapa:** [[...]]`.

**Elementos disponíveis.** Use só os que ajudam o assunto. Nenhum é obrigatório:

- **Resumo rápido** no começo, em poucas linhas (recomendado em notas longas).
- **Explicação em linguagem simples (técnica Feynman)**, em callout `[!example]` com uma analogia do cotidiano, quando o tema for abstrato ou difícil.
- **Esquemas visuais:** fluxograma ou linha do tempo em Mermaid e quadros comparativos.
- **Mapa mental dentro da nota**, como lista aninhada ou Mermaid, quando ajudar. Não crie `.canvas` por conta própria (seção 5.3).
- **Exemplos práticos** em callouts `[!example]`, com valores e datas concretos e a resposta fundamentada.
- **Pontos de atenção:** `[!danger] Pegadinhas`, `[!tip] Números para decorar` e `[!tip] Mnemônicos`.
- **Questões de fixação** em callouts `[!question]`, com gabarito comentado em `> [!success]-` (recolhido), quando fizerem sentido para o assunto.
- **Conexões** no fim da nota, organizadas por relação: Visão geral · Antes · Depois · Paralelo · Matérias ligadas (e Mapa, se existir).

**Não crie, a menos que Meira peça:**

- seção de **flashcards**;
- seção **"Minhas anotações"**: toda a nota é anotação de Meira. Se uma nota antiga já tiver essa seção, deixe-a como está;
- seção separada de **jurisprudência**: ela entra no corpo do texto, no ponto do assunto a que se refere (veja a seção 4.4);
- arquivo `.canvas`.

### 5.2. Folha de revisão

Só com ordem expressa. Use o modelo de `Revisão final - Prova 2...` quando Meira pedir uma revisão de um conjunto de notas (por disciplina, tema ou concurso):

- callout "Como usar esta nota";
- seção "Como o tema costuma ser cobrado" **apenas** se Meira indicar a prova (OAB, concurso ou outra) e houver fonte; sem isso, omita a seção e não invente padrões de cobrança;
- uma seção por nota de origem, com título `## N. Tema → [[Nota de origem]]`, só com o resumo do que já está nas notas;
- tabela "Números para decorar" (Número · O quê · Artigo);
- roteiro de questões em rodadas.

A folha de revisão **não traz conteúdo novo**: tudo vem das notas de origem, que estão linkadas.

### 5.3. Mapas mentais (.canvas)

**Só crie um `.canvas` com ordem expressa de Meira.** Sem essa ordem, não crie mapa em arquivo: ele lota o vault com informação nem sempre necessária. Um mapa feito dentro da própria nota `.md` é permitido (seção 5.1). Para um `.canvas`, leia antes `Títulos executivos.canvas` e siga estas regras:

- **Nome do arquivo:** só o assunto, sem "Mapa - " (ex.: `Títulos executivos.canvas`). Os mapas antigos com o prefixo só mudam de nome se Meira pedir.
- Formato **JSON Canvas válido**, com `nodes` e `edges`. Cada nó tem `id`, `type`, `x`, `y`, `width` e `height`.
- **Nó central:** roxo `#8E44AD`, com título, artigos e o link `[[Nota]]`.
- **Ramos:** um nó de título por ramo (`## Nome`) e nós-filhos de cerca de 390–420 × 130–170. Cada ramo usa uma cor da paleta, repetida nos filhos e nas arestas.
- **Nó "Liga-se a:"** em cinza `#7F8C8D`, com links para as notas relacionadas.
- **Nó de mnemônico** em amarelo `#D4AC0D` ao lado do centro, quando houver.
- Distribua os nós sem sobreposição e confira a validade do JSON depois de editar.

### 5.4. Paleta de cores

|Cor|Uso nos mapas de Execuções|
|---|---|
|`#8E44AD` roxo|Nó central / título|
|`#E74C3C` vermelho|Ramo 1 (ex.: instauração, taxatividade)|
|`#E67E22` laranja|Ramo 2 (ex.: intimação, requisitos)|
|`#2E86C1` azul|Ramo 3 (ex.: prazo, avaliação)|
|`#27AE60` verde|Ramo 4 (ex.: comportamentos, satisfação)|
|`#D63384` rosa|Ramo 5 (ex.: efeitos, leilão)|
|`#16A085` verde-azulado|Ramo complementar (ex.: provisório, condição)|
|`#D4AC0D` amarelo|Cálculos, mnemônicos, pisos de valor|
|`#7F8C8D` cinza|Ligações e informações secundárias|

---

## 6. Como escrever

- **Títulos descritivos:** o título diz o conteúdo da nota ou da seção. Nada de "Bloco 1" ou "Parte 2".
- **Nada de referência vaga.** Não escreva "o mesmo prazo da pretensão de conhecimento" sem dizer qual é esse prazo. Diga o valor concreto, repita-o e explique por extenso o termo citado quando ele não estiver no próprio trecho. Exemplo:
    - ❌ "Prazo para requerer: até a prescrição (mesmo prazo da pretensão de conhecimento)."
    - ✅ "Prazo para requerer: até a **prescrição**. Esse prazo não está no CPC: é o **mesmo prazo de prescrição que valia para propor a ação na fase de conhecimento** (a ação original que gerou a sentença), contado do dia seguinte ao trânsito em julgado. Ex.: cobrança de dívida líquida de contrato → **5 anos** (CC, art. 206, §5º, I); reparação civil por ato ilícito → **3 anos** (CC, art. 206, §3º, V); sem prazo específico → **10 anos** (CC, art. 205)."
- Cite artigos com número e diploma: "art. 523, §1º, do CPC".
- Use referências bibliográficas no padrão ABNT.
- Prefira frases curtas e linguagem técnica clara. Use negrito nos termos e números-chave.
- Explique as siglas na primeira vez em que aparecem (ex.: "MP = material do professor").

---

## 7. Conexões: faça sempre que puder

- **Antes de escrever ou organizar**, procure no vault as notas relacionadas: busque os artigos citados, os institutos e os termos-chave. Inclua também outras disciplinas (ex.: Civil ↔ Processo Civil).
- **No corpo do texto**, coloque o link no ponto em que o assunto aparece, apontando para a seção quando possível: `[[Nota#Seção]]`.
- **Na seção Conexões**, organize por relação: Visão geral · Antes · Depois · Paralelo · Matérias ligadas · Mapa (só se existir).
- **Nos mapas**, use o nó "Liga-se a:".
- Só faça conexões reais, em que um assunto ajuda a entender o outro.
- Confira se a nota de destino existe e se o nome está idêntico, incluindo vírgulas e acentos. Se linkar uma nota que ainda não existe, informe no relatório final.

---

## 8. Pasta "Referências e explicações"

Quando aparecer um **termo ou tópico complexo**, como expressão latina, instituto, teoria ou princípio, ele ganha uma nota própria na pasta `Referências e explicações`. Vale para qualquer área e qualquer termo que surja no texto (ex.: _preclusão_, _litisconsórcio_, _usucapião_, _boa-fé objetiva_, _actio iudicati_). Os termos citados neste arquivo são só exemplos, e não uma lista a seguir.

- **Antes de criar**, procure se a nota já existe. Se existir, só linke.
- **Nome da nota:** o próprio termo (ex.: `Preclusão.md`, `Coisa julgada.md`).
- **Link:** na primeira vez em que o termo aparecer em cada nota, use `[[Nome do termo]]`, ou `[[Nome do termo|forma como aparece no texto]]` quando a frase usar outra forma.
- **Quando criar:**
    - durante uma tarefa de redação ou correção, crie as notas de termo automaticamente;
    - durante uma tarefa só de organização, liste os termos que merecem nota e crie só depois da confirmação de Meira.
- **Conteúdo:** o estilo é livre. Explique da forma que tornar o termo mais claro, com, se couber:
    - o que é, em palavras simples;
    - a explicação técnica;
    - um exemplo concreto;
    - o contraste com o termo oposto ou parecido, quando houver (ex.: nulidade × anulabilidade);
    - onde o termo aparece no vault (links de volta);
    - as fontes.
- As regras de fonte das seções 3 e 4 valem aqui também.
- **Frontmatter mínimo:**

```yaml
---
tipo: referência
area: Área do termo
tags: [Referência, ÁreaDoTermo]
---
```

**Exemplo de tom**, escrito por Meira. Serve só para mostrar o nível de clareza esperado: não crie esta nota nem dê prioridade a este termo, a menos que ele apareça no texto trabalhado.

> **Ex tunc:** efeito de retroação, como se o ato nunca tivesse existido. A decisão com efeito _ex tunc_ volta à época do fato que deu origem à ação: seus efeitos alcançam o passado, desde o momento em que ocorreu aquilo que gerou o processo. Exemplo: a venda de uma casa, feita em 2020, é declarada nula na sentença; a decisão retroage, e a venda deve ser desfeita. Esse efeito costuma estar associado a atos nulos de pleno direito ("natimortos"), em que é necessária a restauração completa do _status quo_.

---

## 9. Relatório ao final de cada tarefa

Termine sempre com um relatório curto:

- arquivos criados, movidos ou alterados, e o que mudou em cada um;
- notas de "Referências e explicações" criadas ou sugeridas;
- links para notas que ainda não existem e links quebrados encontrados;
- erros de conteúdo notados e não corrigidos, com a fonte que mostra o erro;
- pendências marcadas com 🔎;
- sugestão de commit, se for o caso.

---

## 10. Estrutura do vault

<!-- Na primeira sessão, mapeie as pastas do vault e atualize esta seção com o que encontrar. -->

- Organização por disciplina. A pasta `Execuções`, de Processo Civil III, é o modelo de referência de estrutura para notas e mapas (ela foi feita para uma prova, mas o vault é de estudo geral).
- Na raiz do repositório há também notas soltas (ex.: `Responsabilidade Civil.md`, `Neurodireitos.md`, `DALY e QUALY.md`) e a pasta `Estudos Livre`. Nem tudo é de disciplina da faculdade: há estudos de Bioética e outros temas livres. Não force essas notas no molde de uma disciplina.
- `Referências e explicações`: notas de termos e tópicos complexos (seção 8).