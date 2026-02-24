# 01 - if, else e else if

## Objetivo

Aprender a fazer o programa tomar decisao.

## Explicacao curta

Condicional e a base de quase tudo:
"se isso acontecer, faz isso".

Esse e o tipo de assunto que cai em prova e aparece em todo projeto.

## Codigo completo

```c
#include <stdio.h>

int main(void) {
    float nota;

    // le a nota do usuario
    printf("Digite a nota final (0 a 10): ");
    scanf("%f", &nota);

    if (nota >= 7.0f) {
        printf("Aprovado!\\n");
    } else if (nota >= 5.0f) {
        printf("Recuperacao.\\n");
    } else {
        printf("Reprovado.\\n");
    }

    return 0;
}
```

## Como compilar/executar

```bash
gcc if_else.c -o if_else
```

- Windows: `if_else.exe`
- Linux/macOS: `./if_else`

## Saida esperada (exemplo)

Entrada:

```text
Digite a nota final (0 a 10): 6.5
```

Saida:

```text
Recuperacao.
```

## Erros comuns + como resolver

- Usar `=` no lugar de `==` ao comparar.
- Inverter sinal (`>=` / `<=`) e quebrar a logica.
- Esquecer `&` no `scanf`.

> Aqui e onde a maioria erra. Le a condicao em voz alta e confere.

## Exercicios

### Faceis (3)

1. Ler um numero e dizer se e positivo ou negativo.
2. Ler idade e dizer se e maior de idade.
3. Ler numero e dizer se e par ou impar.

### Medios (2)

1. Ler duas notas e mostrar se media >= 6.
2. Ler ano e dizer se e bissexto (regra simplificada: divisivel por 4).

### Desafio (1)

1. Ler tres numeros e mostrar o maior com `if/else`.
