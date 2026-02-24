# 01 - Entrada e saida (`leia` e `escreva`)

## Objetivo

Ler dados do usuario e mostrar resultado no console.

## Explicacao curta

`leia` pega valor digitado.
`escreva` mostra na tela.

Esse aqui e o basico que voce usa em quase todo algoritmo.

## Codigo completo

```portugol
programa
{
    funcao inicio()
    {
        cadeia nome
        inteiro idade

        escreva("Digite seu nome: ")
        leia(nome)

        escreva("Digite sua idade: ")
        leia(idade)

        escreva("Ola, ", nome, "! Voce tem ", idade, " anos.")
    }
}
```

## Como executar

1. Cole no Portugol Studio.
2. Execute com `F6`.
3. Digite nome e idade quando pedir.

## Saida esperada (exemplo)

```text
Digite seu nome: Ana
Digite sua idade: 20
Ola, Ana! Voce tem 20 anos.
```

## Erros comuns + como resolver

- variavel com tipo errado (`inteiro` x `cadeia`)
- esquecer `leia(...)`
- tentar usar variavel sem declarar

## Exercicios

### Faceis (3)

1. Ler nome e cidade e mostrar frase.
2. Ler dois inteiros e mostrar soma.
3. Ler altura (real) e mostrar valor digitado.

### Medios (2)

1. Ler base e altura e mostrar area do retangulo.
2. Ler 3 numeros e mostrar media simples.

### Desafio (1)

1. Ler nome, idade e curso e mostrar um mini cadastro organizado.
