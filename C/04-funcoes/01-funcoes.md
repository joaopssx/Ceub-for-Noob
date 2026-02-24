# 01 - Funcoes

## Objetivo

Quebrar o programa em partes menores e reaproveitaveis.

## Explicacao curta

Funcao deixa o codigo mais limpo.
Em vez de repetir bloco de logica, voce cria uma funcao e chama quando precisar.

## Codigo completo

```c
#include <stdio.h>

int soma(int a, int b) {
    return a + b;
}

float media(float n1, float n2) {
    return (n1 + n2) / 2.0f;
}

int main(void) {
    int x = 10;
    int y = 20;
    float p1 = 7.5f;
    float p2 = 8.5f;

    printf("Soma de %d e %d = %d\\n", x, y, soma(x, y));
    printf("Media de %.1f e %.1f = %.2f\\n", p1, p2, media(p1, p2));

    return 0;
}
```

## Como compilar/executar

```bash
gcc funcoes.c -o funcoes
```

- Windows: `funcoes.exe`
- Linux/macOS: `./funcoes`

## Saida esperada (exemplo)

```text
Soma de 10 e 20 = 30
Media de 7.5 e 8.5 = 8.00
```

## Erros comuns + como resolver

- assinatura da funcao errada (tipo de retorno/parametros).
- esquecer `return` quando a funcao deve retornar valor.
- chamar funcao sem declarar antes.

> Travou aqui? confere tipo de retorno e tipo dos parametros.

## Exercicios

### Faceis (3)

1. Funcao que retorna dobro de um numero.
2. Funcao de area do retangulo.
3. Funcao que diz se numero e par.

### Medios (2)

1. Funcao de media com 3 notas.
2. Funcao de Celsius para Fahrenheit.

### Desafio (1)

1. Fazer menu de calculadora usando funcoes separadas.
