# 01 - Vetores e matrizes

## Objetivo

Guardar varios valores e percorrer com repeticao.

## Explicacao curta

Vetor e lista de uma dimensao.
Matriz e tabela (duas dimensoes).

## Codigo completo

```portugol
programa
{
    funcao inicio()
    {
        inteiro numeros[5]
        inteiro i
        inteiro maior

        para (i = 0; i < 5; i++)
        {
            escreva("Numero ", i + 1, ": ")
            leia(numeros[i])
        }

        maior = numeros[0]

        para (i = 1; i < 5; i++)
        {
            se (numeros[i] > maior)
            {
                maior = numeros[i]
            }
        }

        escreva("Maior valor = ", maior)
    }
}
```

## Como executar

1. Rode o algoritmo.
2. Digite 5 valores.
3. Confira se maior valor bate com sua conta.

## Saida esperada (exemplo)

```text
Numero 1: 4
Numero 2: 2
Numero 3: 9
Numero 4: 1
Numero 5: 7
Maior valor = 9
```

## Erros comuns + como resolver

- acessar indice fora do limite
- loop com condicao errada
- esquecer declarar tamanho do vetor

## Exercicios

### Faceis (3)

1. Ler 5 numeros e mostrar todos.
2. Ler 5 numeros e mostrar soma.
3. Ler 5 numeros e mostrar media.

### Medios (2)

1. Ler matriz 2x2 e mostrar soma dos elementos.
2. Ler 6 notas e mostrar maior e menor.

### Desafio (1)

1. Ler 10 numeros e mostrar em ordem crescente.
