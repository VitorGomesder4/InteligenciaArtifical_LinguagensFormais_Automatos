# Atividade 1 — Checklist da Aula 1

## 1. Alfabeto Σ
Um alfabeto é um conjunto finito e não vazio de símbolos.

Exemplo:
Σ = {a, b}

## 2. Cadeia
Uma cadeia é uma sequência finita de símbolos pertencentes a um alfabeto.

Exemplo:
w = abba

## 3. Palavra vazia ε
ε representa a cadeia que não possui nenhum símbolo.

Seu comprimento é:
|ε| = 0

## 4. Prefixo e sufixo
Para uma palavra w, um prefixo é obtido pegando uma parte inicial de w.
Um sufixo é obtido pegando uma parte final de w.

Para w = ab:
- Prefixos: ε, a, ab
- Sufixos: ε, b, ab

## 5. Σ*
Σ* é o conjunto de todas as cadeias finitas que podem ser formadas com símbolos de Σ, incluindo ε.

## 6. Linguagem formal
Uma linguagem formal é qualquer subconjunto de Σ*.

Portanto:
L ⊆ Σ*

## 7. Gramática formal
Uma gramática formal pode ser representada por:
G = (V, Σ, P, S)

onde:
- V = conjunto de símbolos não terminais;
- Σ = conjunto de símbolos terminais;
- P = conjunto de regras de produção;
- S = símbolo inicial.

## 8. Exemplo de produção
S → aS | ε

Essa gramática gera:
ε, a, aa, aaa, ...

Logo, ela gera palavras formadas somente por a.
