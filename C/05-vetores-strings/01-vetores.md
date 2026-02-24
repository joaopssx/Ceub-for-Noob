# 01 - Vetores

## Objetivo

Aprender a guardar varios valores do mesmo tipo e percorrer com loop.

## Explicacao curta

Vetor e uma lista com posicoes (indices).
Em C, comeca em `0`.

Exemplo: vetor de 5 itens vai de indice `0` ate `4`.

## Codigo completo

```c
#include <stdio.h>

int main(void) {
    int numeros[5];
    int i;
    int maior;

    printf("Digite 5 numeros inteiros:\\n");
    for (i = 0; i < 5; i++) {
        printf("Numero %d: ", i + 1);
        scanf("%d", &numeros[i]);
    }

    maior = numeros[0];

    for (i = 1; i < 5; i++) {
        if (numeros[i] > maior) {
            maior = numeros[i];
        }
    }

    printf("Maior numero digitado: %d\\n", maior);
    return 0;
}
```

## Como compilar/executar

```bash
gcc vetores.c -o vetores
```

- Windows: `vetores.exe`
- Linux/macOS: `./vetores`

## Saida esperada (exemplo)

Entrada:

```text
Digite 5 numeros inteiros:
4
2
9
1
7
```

Saida:

```text
Maior numero digitado: 9
```

## Erros comuns + como resolver

- acessar fora do limite do vetor.
- usar `<=` no loop quando o certo era `<`.
- esquecer `&` no `scanf`.

> Aqui e erro de indice quase toda vez. Revisa com calma.

## Exercicios

### Faceis (3)

1. Ler 5 numeros e mostrar todos.
2. Ler 5 numeros e mostrar soma.
3. Ler 5 numeros e mostrar media.

### Medios (2)

1. Ler 8 numeros e contar quantos sao pares.
2. Ler 6 notas e mostrar maior e menor.

### Desafio (1)

1. Ler 10 numeros e mostrar em ordem crescente.
