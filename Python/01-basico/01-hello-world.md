# 01 - Hello, World! em Python

## Objetivo

Fazer o primeiro script em Python e entender a estrutura minima.

## Explicacao curta

Python e direto: escreve e executa.
Sem etapa de compilacao manual como no C.

## Codigo completo

```python
def main():
    # ponto de entrada do script
    print("Hello, World!")


if __name__ == "__main__":
    main()
```

## Como executar

Windows:

```bash
python hello.py
```

Linux/macOS:

```bash
python3 hello.py
```

## Saida esperada (exemplo)

```text
Hello, World!
```

## Erros comuns + como resolver

- `SyntaxError`
  - quase sempre faltou `:` ou parenteses no `print`
- `IndentationError`
  - bloco mal indentado
- arquivo salvo com nome errado
  - confirme se e `hello.py`

## Exercicios

### Faceis (3)

1. Mostrar seu nome.
2. Mostrar curso e semestre.
3. Mostrar 2 linhas diferentes.

### Medios (2)

1. Mostrar um mini menu com 3 opcoes.
2. Mostrar uma mensagem formatada com variavel.

### Desafio (1)

1. Criar script que mostra um "cartao" com seus dados em varias linhas.
