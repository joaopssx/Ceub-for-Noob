# 01 - if, elif e else

## Objetivo

Tomar decisoes no programa com condicoes.

## Explicacao curta

Mesmo raciocinio do C:

- se acontecer isso -> faz isso
- se nao -> outro caminho

## Codigo completo

```python
def main():
    nota = float(input("Digite a nota final (0 a 10): "))

    if nota >= 7:
        print("Aprovado!")
    elif nota >= 5:
        print("Recuperacao.")
    else:
        print("Reprovado.")


if __name__ == "__main__":
    main()
```

## Como executar

Windows: `python if_elif_else.py`

Linux/macOS: `python3 if_elif_else.py`

## Saida esperada (exemplo)

Entrada:

```text
Digite a nota final (0 a 10): 6.2
```

Saida:

```text
Recuperacao.
```

## Erros comuns + como resolver

- esquecer `:` no fim do `if`/`elif`/`else`
- esquecer indentacao
- comparar texto com numero sem conversao

> Aqui e onde muita gente erra em Python: `:` + indentacao.

## Exercicios

### Faceis (3)

1. Ler numero e dizer se e positivo ou negativo.
2. Ler idade e dizer se e maior de idade.
3. Ler numero e dizer se e par ou impar.

### Medios (2)

1. Ler 2 notas e dizer se media >= 6.
2. Ler salario e mostrar faixa (baixa/media/alta) com regra que voce definir.

### Desafio (1)

1. Ler 3 numeros e mostrar o maior.
