# 01 - Repeticao com for

## Objetivo

Usar `for` pra repetir codigo sem copiar e colar linha.

## Explicacao curta

`for` funciona muito bem quando voce sabe quantas vezes quer repetir.

Estrutura:

- inicio
- condicao
- incremento

Se uma dessas partes estiver errada, vem bug.

## Codigo completo

```c
#include <stdio.h>

int main(void) {
    int n, i;
    int soma = 0;

    printf("Somar de 1 ate: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        soma += i;
    }

    printf("Soma de 1 ate %d = %d\\n", n, soma);
    return 0;
}
```

## Como compilar/executar

```bash
gcc for_soma.c -o for_soma
```

- Windows: `for_soma.exe`
- Linux/macOS: `./for_soma`

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

- esquecer `i++` e cair em loop infinito.
- usar `<` quando precisava `<=`.
- nao inicializar `soma` com `0`.

> Se o resultado sair estranho, revisa o limite do loop primeiro.

## Exercicios

### Faceis (3)

1. Mostrar numeros de 1 a 10.
2. Mostrar pares de 0 a 20.
3. Mostrar tabuada de um numero.

### Medios (2)

1. Calcular fatorial de `n`.
2. Ler 5 numeros e mostrar soma total.

### Desafio (1)

1. Ler `n` e dizer se ele e primo.
