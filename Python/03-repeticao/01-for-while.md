# 01 - Repeticao com for e while

## Objetivo

Repetir tarefas com `for` e `while` sem duplicar codigo.

## Explicacao curta

- `for`: quando voce sabe quantas repeticoes quer
- `while`: quando depende de condicao

## Codigo completo

```python
def main():
    n = int(input("Somar de 1 ate: "))
    soma = 0

    for i in range(1, n + 1):
        soma += i

    print(f"Soma de 1 ate {n} = {soma}")


if __name__ == "__main__":
    main()
```

## Como executar

Windows: `python repeticao.py`

Linux/macOS: `python3 repeticao.py`

## Saida esperada (exemplo)

Entrada:

```text
Somar de 1 ate: 5
```

Saida:

```text
Soma de 1 ate 5 = 15
```

## Erros comuns + como resolver

- `range` com limite errado (`n` em vez de `n + 1`)
- loop infinito no `while`
- esquecer conversao `int(input(...))`

## Exercicios

### Faceis (3)

1. Mostrar de 1 ate 10 com `for`.
2. Mostrar pares de 0 a 20.
3. Fazer tabuada de um numero.

### Medios (2)

1. Calcular fatorial de `n`.
2. Ler 5 numeros e mostrar soma.

### Desafio (1)

1. Ler `n` e dizer se e primo.
