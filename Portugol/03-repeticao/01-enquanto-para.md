# 01 - Repeticao com `enquanto` e `para`

## Objetivo

Repetir comandos sem copiar e colar codigo.

## Explicacao curta

- `para`: quando voce sabe quantas vezes vai repetir
- `enquanto`: quando depende de condicao

## Codigo completo

```portugol
programa
{
    funcao inicio()
    {
        inteiro n
        inteiro i
        inteiro soma = 0

        escreva("Somar de 1 ate: ")
        leia(n)

        para (i = 1; i <= n; i++)
        {
            soma = soma + i
        }

        escreva("Soma de 1 ate ", n, " = ", soma)
    }
}
```

## Como executar

1. Rode com `F6`.
2. Digite um valor para `n`.
3. Compare resultado com conta manual.

## Saida esperada (exemplo)

```text
Somar de 1 ate: 5
Soma de 1 ate 5 = 15
```

## Erros comuns + como resolver

- limite errado no `para`
- esquecer incremento de controle
- variavel soma sem iniciar em zero

## Exercicios

### Faceis (3)

1. Mostrar numeros de 1 a 10.
2. Mostrar pares de 0 a 20.
3. Fazer tabuada de um numero.

### Medios (2)

1. Calcular fatorial de `n`.
2. Ler 5 numeros e mostrar soma.

### Desafio (1)

1. Ler `n` e dizer se e primo.
