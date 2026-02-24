# 01 - Ponteiros (sem drama)

## Objetivo

Entender `&` e `*` sem complicar.

## Explicacao curta

Ponteiro guarda endereco de memoria.

- `&variavel` -> pega endereco
- `*ponteiro` -> pega valor no endereco

Se isso parece estranho no inicio, normal. Todo mundo passa por isso.

## Codigo completo

```c
#include <stdio.h>

int main(void) {
    int numero = 10;
    int *p = &numero;

    printf("Valor de numero: %d\\n", numero);
    printf("Endereco de numero: %p\\n", (void *)&numero);
    printf("Valor guardado em p: %p\\n", (void *)p);
    printf("Valor apontado por p: %d\\n", *p);

    *p = 25; // altera a variavel pelo ponteiro
    printf("Novo valor de numero: %d\\n", numero);

    return 0;
}
```

## Como compilar/executar

```bash
gcc ponteiros.c -o ponteiros
```

- Windows: `ponteiros.exe`
- Linux/macOS: `./ponteiros`

## Saida esperada (exemplo)

```text
Valor de numero: 10
Endereco de numero: 0x...
Valor guardado em p: 0x...
Valor apontado por p: 10
Novo valor de numero: 25
```

## Erros comuns + como resolver

- ponteiro sem inicializar.
- confundir `p` com `*p`.
- imprimir endereco com formato errado (sempre `%p`).

> Dica: imprime tudo e vai comparando. Ajuda muito aqui.

## Exercicios

### Faceis (3)

1. Criar `int` + ponteiro e imprimir valor/endereco.
2. Alterar valor usando `*ponteiro`.
3. Mostrar endereco de duas variaveis.

### Medios (2)

1. Funcao que recebe `int *` e dobra valor.
2. Funcao que soma 10 usando endereco.

### Desafio (1)

1. Criar `trocar(int *a, int *b)` e trocar duas variaveis.
