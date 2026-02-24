# 01 - Dicionarios

## Objetivo

Guardar dados em pares `chave: valor` e acessar de forma organizada.

## Explicacao curta

Dicionario e tipo uma tabela pequena dentro do codigo.
Em vez de acessar por indice (`0`, `1`, `2`), voce acessa por chave (`nome`, `idade`).

## Codigo completo

```python
def main():
    aluno = {
        "nome": input("Nome: "),
        "idade": int(input("Idade: ")),
        "curso": input("Curso: "),
    }

    print("\nResumo do aluno")
    print(f"Nome: {aluno['nome']}")
    print(f"Idade: {aluno['idade']}")
    print(f"Curso: {aluno['curso']}")


if __name__ == "__main__":
    main()
```

## Como executar

Windows: `python dicionarios.py`

Linux/macOS: `python3 dicionarios.py`

## Saida esperada (exemplo)

```text
Nome: Ana
Idade: 20
Curso: ADS

Resumo do aluno
Nome: Ana
Idade: 20
Curso: ADS
```

## Erros comuns + como resolver

- `KeyError` por chave errada
- esquecer aspas na chave
- converter idade sem `int(...)`

> Se der `KeyError`, imprime o dicionario e confere as chaves.

## Exercicios

### Faceis (3)

1. Criar dicionario com nome, idade e cidade.
2. Mostrar so o nome e cidade.
3. Alterar idade e mostrar dicionario atualizado.

### Medios (2)

1. Ler 3 produtos (nome/preco) e guardar em lista de dicionarios.
2. Somar preco total dos produtos.

### Desafio (1)

1. Criar mini cadastro com menu: adicionar, listar, buscar por nome.
