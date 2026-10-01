# Atividade 2 — Exercícios de Linguagens Formais e Gramáticas

## 1. Alfabeto {a,b,c}
Um exemplo de alfabeto é:
Σ = {a, b, c}

Algumas palavras pertencentes a Σ*:
ε, a, b, c, ab, abc, cba, aaac.

## 2. Palavras válidas sobre {0,1}
Considerando:
Σ = {0,1}

São válidas todas as cadeias formadas somente por 0 e 1, incluindo ε.

Exemplos:
ε, 0, 1, 00, 01, 101, 1100.

## 3. Pertinência em Σ e Σ*
Se Σ = {a,b}, então:
- a ∈ Σ
- b ∈ Σ
- ab ∈ Σ*
- aba ∈ Σ*
- c ∉ Σ
- ac ∉ Σ*

Uma cadeia com mais de um símbolo normalmente pertence a Σ*, não diretamente a Σ.

## 4. Pertinência em uma linguagem
Se:
L = {a, ab, abb, abbb}

então:
- a ∈ L
- ab ∈ L
- abb ∈ L
- b ∉ L
- aa ∉ L

## 5. Linguagem L = {bⁿ | n ≥ 1}
As palavras da linguagem são:
b, bb, bbb, bbbb, ...

A palavra vazia ε não pertence a L porque n deve ser maior ou igual a 1.

## 6. Diferença entre ∅ e {ε}
- ∅ é a linguagem vazia: não contém nenhuma palavra.
- {ε} contém exatamente uma palavra: a palavra vazia ε.

Portanto:
|∅| = 0
|{ε}| = 1

## 7. Componentes de uma gramática
Para:
G = (V, Σ, P, S)

temos:
- V: não terminais;
- Σ: terminais;
- P: produções;
- S: símbolo inicial.

## 8. Derivação usando S → 0S
Considere:
S → 0S | ε

Podemos gerar:
S ⇒ 0S ⇒ 00S ⇒ 000S ⇒ 000

Portanto, 000 é gerada pela gramática.

## 9. Derivação de aaab
Uma gramática possível para gerar palavras da forma aⁿb é:

S → aS | b

Então:
S ⇒ aS ⇒ aaS ⇒ aaaS ⇒ aaab

Logo, aaab pode ser gerada.

## 10. Verificação de palavras
Para verificar se uma palavra pode ser gerada por uma gramática, devemos iniciar em S e aplicar as regras de produção até chegar exatamente à palavra analisada.

Uma palavra pertence à linguagem da gramática quando existe pelo menos uma derivação que começa em S e termina nessa palavra.
