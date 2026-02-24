# Gabarito comentado - Lista 01

Se travou em algum, compara com calma e tenta entender o raciocinio antes de copiar.

## Como usar esse gabarito

1. Tenta resolver sozinho primeiro.
2. Compara sua logica com a solucao.
3. Se estiver diferente, tudo bem. O importante e funcionar e voce entender.

> Dica: roda cada codigo e testa com entradas diferentes.

## 1) Nome e idade

```c
#include <stdio.h>

int main(void) {
    char nome[100];
    int idade;

    printf("Digite seu nome: ");
    // limita a leitura pra nao estourar o vetor
    scanf("%99s", nome);

    printf("Digite sua idade: ");
    scanf("%d", &idade);

    printf("Ola, %s! Voce tem %d anos.\\n", nome, idade);
    return 0;
}
```

Comentario rapido: `%99s` evita estourar o vetor de nome.

## 2) Soma de dois inteiros

```c
#include <stdio.h>

int main(void) {
    int a, b;

    printf("Digite dois inteiros: ");
    scanf("%d %d", &a, &b);

    printf("Soma = %d\\n", a + b);
    return 0;
}
```

## 3) Quatro operacoes com reais

```c
#include <stdio.h>

int main(void) {
    float a, b;

    printf("Digite dois numeros reais: ");
    scanf("%f %f", &a, &b);

    printf("Soma: %.2f\\n", a + b);
    printf("Subtracao: %.2f\\n", a - b);
    printf("Multiplicacao: %.2f\\n", a * b);

    // cuidado com divisao por zero
    if (b != 0) {
        printf("Divisao: %.2f\\n", a / b);
    } else {
        printf("Divisao: impossivel (divisor zero).\\n");
    }

    return 0;
}
```

## 4) Area do retangulo

```c
#include <stdio.h>

int main(void) {
    float base, altura;

    printf("Base e altura: ");
    scanf("%f %f", &base, &altura);

    printf("Area = %.2f\\n", base * altura);
    return 0;
}
```

## 5) Par ou impar

```c
#include <stdio.h>

int main(void) {
    int n;

    printf("Digite um inteiro: ");
    scanf("%d", &n);

    // resto 0 = par, resto 1 = impar
    if (n % 2 == 0) {
        printf("Par\\n");
    } else {
        printf("Impar\\n");
    }

    return 0;
}
```

## 6) Aprovado / Recuperacao / Reprovado

```c
#include <stdio.h>

int main(void) {
    float nota;

    printf("Digite a nota final: ");
    scanf("%f", &nota);

    if (nota >= 7.0f) {
        printf("Aprovado\\n");
    } else if (nota >= 5.0f) {
        printf("Recuperacao\\n");
    } else {
        printf("Reprovado\\n");
    }

    return 0;
}
```

## 7) Mostrar de 1 ate n

```c
#include <stdio.h>

int main(void) {
    int n, i;

    printf("Digite n: ");
    scanf("%d", &n);

    // percorre de 1 ate n
    for (i = 1; i <= n; i++) {
        printf("%d ", i);
    }
    printf("\\n");

    return 0;
}
```

## 8) Soma de 1 ate n

```c
#include <stdio.h>

int main(void) {
    int n, i;
    int soma = 0;

    printf("Digite n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        soma += i;
    }

    printf("Soma = %d\\n", soma);
    return 0;
}
```

## 9) Fatorial de n

```c
#include <stdio.h>

int main(void) {
    int n, i;
    unsigned long long fat = 1;

    printf("Digite n: ");
    scanf("%d", &n);

    // sem fatorial pra numero negativo
    if (n < 0) {
        printf("Fatorial nao definido para negativos.\\n");
        return 0;
    }

    for (i = 1; i <= n; i++) {
        fat *= i;
    }

    printf("%d! = %llu\\n", n, fat);
    return 0;
}
```

## 10) Funcao quadrado

```c
#include <stdio.h>

int quadrado(int x) {
    return x * x;
}

int main(void) {
    int n;

    printf("Digite um inteiro: ");
    scanf("%d", &n);

    printf("Quadrado = %d\\n", quadrado(n));
    return 0;
}
```

## 11) Funcao media de 3 notas

```c
#include <stdio.h>

float media3(float a, float b, float c) {
    return (a + b + c) / 3.0f;
}

int main(void) {
    float n1, n2, n3;

    printf("Digite 3 notas: ");
    scanf("%f %f %f", &n1, &n2, &n3);

    printf("Media = %.2f\\n", media3(n1, n2, n3));
    return 0;
}
```

## 12) Vetor com soma e maior valor

```c
#include <stdio.h>

int main(void) {
    int v[5];
    int i;
    int soma = 0;
    int maior;

    printf("Digite 5 inteiros:\\n");
    // primeiro le os valores
    for (i = 0; i < 5; i++) {
        printf("v[%d] = ", i);
        scanf("%d", &v[i]);
    }

    maior = v[0];

    // depois calcula soma e maior
    for (i = 0; i < 5; i++) {
        soma += v[i];
        if (v[i] > maior) {
            maior = v[i];
        }
    }

    printf("Valores: ");
    for (i = 0; i < 5; i++) {
        printf("%d ", v[i]);
    }

    printf("\\nSoma = %d\\n", soma);
    printf("Maior = %d\\n", maior);
    return 0;
}
```

Se der erro em qualquer exercicio, geralmente e uma dessas tres coisas: tipo errado, `scanf` sem `&`, ou loop mal fechado.
