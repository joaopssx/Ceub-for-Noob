# 01 - Condicionais com `se` e `senao`

## Objetivo

Tomar decisao no algoritmo com base em condicoes.

## Explicacao curta

Mesmo esquema de qualquer linguagem:

- se for verdade, executa um bloco
- senao, executa outro

## Codigo completo

```portugol
programa
{
    funcao inicio()
    {
        real nota

        escreva("Digite a nota final (0 a 10): ")
        leia(nota)

        se (nota >= 7)
        {
            escreva("Aprovado!")
        }
        senao se (nota >= 5)
        {
            escreva("Recuperacao.")
        }
        senao
        {
            escreva("Reprovado.")
        }
    }
}
```

## Como executar

1. Execute o algoritmo.
2. Teste com nota 8.0, 6.0 e 3.0.

## Saida esperada (exemplo)

```text
Digite a nota final (0 a 10): 6
Recuperacao.
```

## Erros comuns + como resolver

- usar condicao com operador errado
- esquecer chaves no bloco
- comparar texto com numero

## Exercicios

### Faceis (3)

1. Ler numero e dizer se e positivo ou negativo.
2. Ler idade e dizer se e maior de idade.
3. Ler numero e dizer se e par ou impar.

### Medios (2)

1. Ler salario e mostrar faixa (baixa/media/alta).
2. Ler 2 numeros e mostrar o maior.

### Desafio (1)

1. Ler 3 numeros e mostrar o maior usando condicional.
