# 01 - Funcoes em Python

## Objetivo

Separar logica em funcoes pra deixar o codigo mais limpo.

## Explicacao curta

Funcao evita repeticao e deixa o programa facil de manter.

## Codigo completo

```python
def soma(a, b):
    return a + b


def media(n1, n2):
    return (n1 + n2) / 2


def main():
    x = 10
    y = 20
    p1 = 7.5
    p2 = 8.5

    print(f"Soma de {x} e {y} = {soma(x, y)}")
    print(f"Media de {p1} e {p2} = {media(p1, p2):.2f}")


if __name__ == "__main__":
    main()
```

## Como executar

Windows: `python funcoes.py`

Linux/macOS: `python3 funcoes.py`

## Saida esperada (exemplo)

```text
Soma de 10 e 20 = 30
Media de 7.5 e 8.5 = 8.00
```

## Erros comuns + como resolver

- chamar funcao com quantidade errada de argumentos
- esquecer `return` quando precisa resultado
- reaproveitar nome de variavel e confundir leitura

## Exercicios

### Faceis (3)

1. Funcao que retorna dobro.
2. Funcao que retorna area do retangulo.
3. Funcao que diz se numero e par.

### Medios (2)

1. Funcao de media de 3 notas.
2. Funcao de conversao Celsius -> Fahrenheit.

### Desafio (1)

1. Fazer calculadora com funcoes separadas.
