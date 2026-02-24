# 01 - Listas e strings

## Objetivo

Aprender a guardar varios valores em lista e manipular texto com string.

## Explicacao curta

Lista em Python e tipo vetor, mas mais flexivel.
String e texto. E voce vai usar isso o tempo inteiro.

## Codigo completo

```python
def main():
    numeros = []

    for i in range(5):
        valor = int(input(f"Numero {i + 1}: "))
        numeros.append(valor)

    maior = max(numeros)
    soma = sum(numeros)

    print(f"Lista: {numeros}")
    print(f"Soma: {soma}")
    print(f"Maior: {maior}")

    nome = input("Digite seu nome: ").strip()
    print(f"Nome em maiusculo: {nome.upper()}")


if __name__ == "__main__":
    main()
```

## Como executar

Windows: `python listas_strings.py`

Linux/macOS: `python3 listas_strings.py`

## Saida esperada (exemplo)

```text
Numero 1: 4
Numero 2: 2
Numero 3: 9
Numero 4: 1
Numero 5: 7
Lista: [4, 2, 9, 1, 7]
Soma: 23
Maior: 9
Digite seu nome: joao
Nome em maiusculo: JOAO
```

## Erros comuns + como resolver

- esquecer conversao pra `int`
- tentar acessar indice inexistente
- usar metodos de string em variavel que nao e string

## Exercicios

### Faceis (3)

1. Ler 5 numeros e mostrar a lista.
2. Ler 5 numeros e mostrar soma.
3. Ler um nome e mostrar em maiusculo e minusculo.

### Medios (2)

1. Ler 6 notas e mostrar maior, menor e media.
2. Ler frase e contar quantas letras `a` existem.

### Desafio (1)

1. Ler 10 numeros e mostrar lista ordenada sem usar `sort`.
