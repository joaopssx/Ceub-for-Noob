# 01 - Hello, World!

## Objetivo

Fazer seu primeiro programa em C e entender o minimo pra um arquivo funcionar.

## Explicacao curta

Todo programa em C comeca na funcao `main`.
Esse exemplo e simples de proposito, so pra voce pegar o fluxo: escrever, compilar, executar.

## Codigo completo

```c
#include <stdio.h>

int main(void) {
    // ponto de entrada
    printf("Hello, World!\\n");
    return 0;
}
```

## Como compilar/executar

```bash
gcc hello.c -o hello
```

- Windows: `hello.exe`
- Linux/macOS: `./hello`

## Saida esperada (exemplo)

```text
Hello, World!
```

## Erros comuns + como resolver

- `expected ';'`
  - faltou `;` no fim de alguma linha.
- `implicit declaration of function 'printf'`
  - faltou `#include <stdio.h>`.
- texto com aspas estranhas
  - usa aspas normais do teclado (`"`).

> Se der erro aqui, quase sempre e digitacao.

## Exercicios

### Faceis (3)

1. Mostrar seu nome no terminal.
2. Mostrar sua idade numa frase.
3. Mostrar duas frases em linhas separadas.

### Medios (2)

1. Montar um mini cartao com nome, curso e semestre.
2. Usar `\n` e `\t` pra formatar melhor a saida.

### Desafio (1)

1. Mostrar um mini menu de terminal com 3 opcoes (so texto).
