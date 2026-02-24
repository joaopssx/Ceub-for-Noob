# 01 - Registro (dados organizados)

## Objetivo

Agrupar informacoes relacionadas em um unico tipo de dado.

## Explicacao curta

Registro e como uma "ficha".
Em vez de variaveis soltas, voce junta tudo: nome, idade, curso.

## Codigo completo

```portugol
programa
{
    registro Aluno
    {
        cadeia nome
        inteiro idade
        cadeia curso
    }

    funcao inicio()
    {
        Aluno a

        escreva("Nome: ")
        leia(a.nome)

        escreva("Idade: ")
        leia(a.idade)

        escreva("Curso: ")
        leia(a.curso)

        escreva("\nResumo do aluno\n")
        escreva("Nome: ", a.nome, "\n")
        escreva("Idade: ", a.idade, "\n")
        escreva("Curso: ", a.curso)
    }
}
```

## Como executar

1. Execute.
2. Digite os dados.
3. Veja o resumo final.

## Saida esperada (exemplo)

```text
Nome: Ana
Idade: 20
Curso: ADS

Resumo do aluno
Nome: Ana
Idade: 20
Curso: ADS
```

## Erros comuns + como resolver

- esquecer campo do registro
- tentar acessar campo com nome errado
- confundir variavel simples com registro

## Exercicios

### Faceis (3)

1. Criar registro `Produto` (nome, preco).
2. Ler e mostrar um produto.
3. Criar registro `Pessoa` (nome, idade).

### Medios (2)

1. Criar vetor de 3 registros `Aluno`.
2. Mostrar todos os alunos cadastrados.

### Desafio (1)

1. Criar mini cadastro com menu: adicionar e listar registros.
