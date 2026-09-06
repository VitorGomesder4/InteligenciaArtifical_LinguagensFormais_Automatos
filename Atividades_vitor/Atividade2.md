## Exercício 1

Considere:

$$
\Sigma = {a,b,c}
$$

Responda:

1. Quantos símbolos existem no alfabeto?

    3

2. Quais são os símbolos?

    a,b,c.

3. O símbolo `a` pertence ao alfabeto?

    Sim.

4. O símbolo `d` pertence ao alfabeto?

    Não.

5. Escreva uma palavra formada por símbolos desse alfabeto.

    babaca.

---

## Exercício 2

Considere:

$$
\Sigma = {0,1}
$$

Classifique cada sequência como **palavra válida** ou **não válida** e justifique sua resposta:

| Sequência | Válida? |          Justificativa                  |
| --------- | ------- | ----------------------------------------|
| `0101`    |   SIM   |   Simbolos contidas no alfabeto         |
| `00110`   |   SIM   |   Simbolos contidas no alfabeto         |
| `012`     |   NÃO   |   Simbolo "2" não contido no alfabeto   |
| `111`     |   SIM   |   Simbolos contidas no alfabeto         |
| `10a`     |   NÃO   |   Simbolo "a" não contido no alfabeto   |

---

## Exercício 3

Considere:

$$
\Sigma = {0,1}
$$

Determine se as afirmações são **verdadeiras ou falsas** e justifique cada resposta:

1. $0 \in \Sigma$

    TRUE

2. $1 \in \Sigma$

    TRUE

3. $01 \in \Sigma$

    FALSE

4. $01 \in \Sigma^*$

    TRUE

5. $2 \in \Sigma$

    FALSE

6. $101 \in \Sigma^*$

    TRUE

---

## Exercício 4

Considere:

$$
L = {0,01,011,0111}
$$

Determine se cada palavra pertence à linguagem:

1. $0 \in L$

    SIM

2. $01 \in L$

    SIM

3. $0111 \in L$

    SIM

4. $10 \in L$

    NÃO

5. $111 \in L$

    SIM

6. $011 \in L$

    SIM

---

## Exercício 5

Considere:

$$
L = {b^n \mid n \geq 1}
$$

Responda:

1. Escreva as cinco primeiras palavras.

    {b,bb,bbb,bbbb,bbbbb}

2. Explique o significado de $b^n$.

    b repetido n vezes

3. A palavra `bbbbbb` pertence à linguagem?

    SIM

4. A palavra vazia ($\varepsilon$) pertence à linguagem?

    NÃO pois n > 1

---

## Exercício 6

Explique, com suas próprias palavras, a diferença entre:

### A

$$
L=\emptyset
$$

    É uma linguagem onde o conjunto de palavras é nula

### B

$$
L={\varepsilon}
$$

    É uma linguagem onde a unica palavra é ε

Depois responda:

1. Qual delas possui uma palavra?

    L=ε

2. Qual delas não possui nenhuma palavra?

    L=∅

3. Qual é o comprimento da palavra $\varepsilon$?
    0




---

## Exercício 7

Considere:

$$
G= ({S,A},{0,1},P,S)
$$

com:

$$
P={S\rightarrow0A,\ A\rightarrow1}
$$

Identifique:

1. O conjunto de variáveis.

    {S, A}

2. O conjunto de terminais.

    {0, 1}

3. O conjunto de produções.

    P = {S→0A, A→1}

4. O símbolo inicial.

    S

5. Qual palavra pode ser gerada por essa gramática?

    S→0A→01


---

## Exercício 8

Considere:

$$
S\rightarrow0S
$$

Começando com $S$:

1. Aplique a regra uma vez.

    S→0S

2. Aplique a regra duas vezes.

    S→0S→00S

3. Aplique a regra três vezes.

    S→0S→00S→000S

4. Escreva a sequência completa de derivação.

    S→0S→00S→000S→...


---

## Exercício 9

Utilizando:

$$
G:
\begin{cases}
S\rightarrow aS\\
S\rightarrow b
\end{cases}
$$

Gere:

$$
aaab
$$

Escreva todos os passos da derivação.

S→aS
\(aS \rightarrow aaS\)
\(aaS \rightarrow aaaS\)
aaaS→aaab

---

## Exercício 10

Considere:

$$
G:
\begin{cases}
S\rightarrow0S\\
S\rightarrow1
\end{cases}
$$

Determine se cada palavra pode ser gerada:

1. `1`: SIM
2. `01`: SIM
3. `001`: SIM
4. `0001`: SIM
5. `101`: NÃO
6. `1001`: NÃO

Para as palavras que podem ser geradas, apresente a derivação completa.
