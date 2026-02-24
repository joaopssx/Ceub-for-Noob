# 01 - Funcoes e procedimentos

## Objetivo

Separar logica em blocos menores pra organizar melhor o algoritmo.

## Explicacao curta

Funcao retorna valor.
Procedimento so executa tarefa.

Quando o algoritmo cresce, isso ajuda muito.

## Codigo completo

```portugol
programa
{
    funcao inteiro soma(inteiro a, inteiro b)
    {
        retorne a + b
    }

    procedimento mostrarCabecalho()
    {
        escreva("=== CALCULO RAPIDO ===\n")
    }

    funcao inicio()
    {
        inteiro x
        inteiro y
        inteiro resultado

        mostrarCabecalho()

        escreva("Digite dois numeros: ")
        leia(x, y)

        resultado = soma(x, y)
        escreva("Resultado = ", resultado)
    }
}
```

## Como executar

1. Execute com `F6`.
2. Digite dois inteiros.
3. Veja resultado da funcao.

## Saida esperada (exemplo)

```text
=== CALCULO RAPIDO ===
Digite dois numeros: 10 20
Resultado = 30
```

## Erros comuns + como resolver

- chamar funcao com parametros errados
- esquecer `retorne` na funcao
- confundir procedimento com funcao

## Exercicios

### Faceis (3)

1. Funcao que retorna dobro de um numero.
2. Funcao que retorna media de 2 notas.
3. Procedimento que imprime cabecalho.

### Medios (2)

1. Funcao que retorna area do retangulo.
2. Funcao que retorna se numero e par.

### Desafio (1)

1. Montar mini calculadora com funcoes de soma e subtracao.
