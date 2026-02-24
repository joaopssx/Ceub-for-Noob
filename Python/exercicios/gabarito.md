# Gabarito comentado - Lista 01 (Python)

Use esse gabarito como apoio.
Primeiro tenta resolver sozinho, depois compara.

## 1) Nome e idade

```python
def main():
    nome = input("Digite seu nome: ")
    idade = int(input("Digite sua idade: "))
    print(f"Ola, {nome}! Voce tem {idade} anos.")


if __name__ == "__main__":
    main()
```

## 2) Soma de dois inteiros

```python
def main():
    a = int(input("Primeiro inteiro: "))
    b = int(input("Segundo inteiro: "))
    print(f"Soma = {a + b}")


if __name__ == "__main__":
    main()
```

## 3) Par ou impar

```python
def main():
    n = int(input("Digite um inteiro: "))

    # resto 0 = par
    if n % 2 == 0:
        print("Par")
    else:
        print("Impar")


if __name__ == "__main__":
    main()
```

## 4) Aprovado / Recuperacao / Reprovado

```python
def main():
    nota = float(input("Nota final: "))

    if nota >= 7:
        print("Aprovado")
    elif nota >= 5:
        print("Recuperacao")
    else:
        print("Reprovado")


if __name__ == "__main__":
    main()
```

## 5) Soma de 1 ate n

```python
def main():
    n = int(input("Digite n: "))
    soma = 0

    for i in range(1, n + 1):
        soma += i

    print(f"Soma = {soma}")


if __name__ == "__main__":
    main()
```

## 6) Lista com soma e maior

```python
def main():
    numeros = []

    for i in range(5):
        numeros.append(int(input(f"Numero {i + 1}: ")))

    print(f"Lista: {numeros}")
    print(f"Soma: {sum(numeros)}")
    print(f"Maior: {max(numeros)}")


if __name__ == "__main__":
    main()
```

## 7) Tabuada

```python
def main():
    n = int(input("Tabuada de: "))

    for i in range(1, 11):
        print(f"{n} x {i} = {n * i}")


if __name__ == "__main__":
    main()
```

## 8) Fatorial

```python
def main():
    n = int(input("Digite n: "))

    if n < 0:
        print("Nao existe fatorial de numero negativo")
        return

    fat = 1
    for i in range(1, n + 1):
        fat *= i

    print(f"{n}! = {fat}")


if __name__ == "__main__":
    main()
```

## 9) Funcao quadrado

```python
def quadrado(x):
    return x * x


def main():
    n = int(input("Digite um inteiro: "))
    print(f"Quadrado = {quadrado(n)}")


if __name__ == "__main__":
    main()
```

## 10) Funcao media3

```python
def media3(a, b, c):
    return (a + b + c) / 3


def main():
    n1 = float(input("Nota 1: "))
    n2 = float(input("Nota 2: "))
    n3 = float(input("Nota 3: "))

    print(f"Media = {media3(n1, n2, n3):.2f}")


if __name__ == "__main__":
    main()
```

## 11) Contar vogais

```python
def main():
    frase = input("Digite uma frase: ").lower()
    vogais = "aeiou"
    total = 0

    for letra in frase:
        if letra in vogais:
            total += 1

    print(f"Total de vogais: {total}")


if __name__ == "__main__":
    main()
```

## 12) Dicionario de aluno

```python
def main():
    aluno = {
        "nome": input("Nome: "),
        "idade": int(input("Idade: ")),
        "curso": input("Curso: "),
    }

    print("\nResumo")
    print(f"Nome: {aluno['nome']}")
    print(f"Idade: {aluno['idade']}")
    print(f"Curso: {aluno['curso']}")


if __name__ == "__main__":
    main()
```

Se der erro em Python, quase sempre e uma dessas tres coisas:

- indentacao
- tipo errado (`str`/`int`/`float`)
- nome de variavel/chave digitado diferente
