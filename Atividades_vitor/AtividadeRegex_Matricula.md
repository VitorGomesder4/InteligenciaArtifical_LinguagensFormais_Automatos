# Atividade prática — Regex de matrícula acadêmica

## Formato

A matrícula deve seguir:

```text
CURSO-ANO-NÚMERO-TURNO
```

Regras:
- CURSO = CCO, ESW ou SIS
- ANO = 2024 até 2029
- NÚMERO = exatamente 4 algarismos
- TURNO = M, T ou N
- nenhum caractere adicional é permitido

## Regex

```regex
^(CCO|ESW|SIS)-(202[4-9])-[0-9]{4}-(M|T|N)$
```

## Explicação

- `^` — início da cadeia.
- `(CCO|ESW|SIS)` — permite somente os três cursos definidos.
- `-` — hífen obrigatório.
- `202[4-9]` — aceita 2024, 2025, 2026, 2027, 2028 ou 2029.
- `[0-9]{4}` — exatamente quatro algarismos.
- `(M|T|N)` — permite os turnos M, T ou N.
- `$` — final da cadeia.

## Testes válidos

| Entrada | Resultado |
|---|---|
| CCO-2024-0001-M | Válido |
| ESW-2029-1234-N | Válido |
| SIS-2026-5678-T | Válido |
| CCO-2025-4321-M | Válido |

## Testes inválidos

| Entrada | Resultado | Motivo |
|---|---|---|
| CCO-2023-0001-M | Inválido | Ano fora do intervalo |
| ESW-2030-1234-N | Inválido | Ano fora do intervalo |
| ABC-2026-1234-M | Inválido | Curso não permitido |
| SIS-2026-123-M | Inválido | Número não possui quatro algarismos |
| CCO-2026-12345-M | Inválido | Número possui cinco algarismos |
| CCO-2026-0001-X | Inválido | Turno não permitido |
| CCO-2026-0001-MM | Inválido | Turno possui caracteres extras |
| CCO-2026-0001-M-extra | Inválido | Existem caracteres extras |

## Casos solicitados

### Limite inferior do ano
`CCO-2024-0001-M` — válido.

### Limite superior do ano
`SIS-2029-9999-N` — válido.

### Quase correto
`ESW-2029-1234-X` — inválido, pois X não é um turno permitido.

### Caracteres extras
`CCO-2026-0001-MX` — inválido devido ao caractere extra.
