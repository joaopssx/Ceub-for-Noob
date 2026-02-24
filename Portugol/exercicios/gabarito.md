# Gabarito comentado - Lista 01 (Portugol)

Tenta resolver sozinho antes de olhar.
Depois compara com calma.

## 1) Nome e idade

```portugol
programa
{
    funcao inicio()
    {
        cadeia nome
        inteiro idade

        escreva("Nome: ")
        leia(nome)

        escreva("Idade: ")
        leia(idade)

        escreva("Ola, ", nome, "! Voce tem ", idade, " anos.")
    }
}
```

## 2) Soma de dois inteiros

```portugol
programa
{
    funcao inicio()
    {
        inteiro a
        inteiro b

        leia(a, b)
        escreva("Soma = ", a + b)
    }
}
```

## 3) Par ou impar

```portugol
programa
{
    funcao inicio()
    {
        inteiro n
        leia(n)

        se (n % 2 == 0)
        {
            escreva("Par")
        }
        senao
        {
            escreva("Impar")
        }
    }
}
```

## 4) Aprovado / Recuperacao / Reprovado

```portugol
programa
{
    funcao inicio()
    {
        real nota
        leia(nota)

        se (nota >= 7)
        {
            escreva("Aprovado")
        }
        senao se (nota >= 5)
        {
            escreva("Recuperacao")
        }
        senao
        {
            escreva("Reprovado")
        }
    }
}
```

## 5) Soma de 1 ate n

```portugol
programa
{
    funcao inicio()
    {
        inteiro n
        inteiro i
        inteiro soma = 0

        leia(n)

        para (i = 1; i <= n; i++)
        {
            soma = soma + i
        }

        escreva("Soma = ", soma)
    }
}
```

## 6) Vetor com soma e maior

```portugol
programa
{
    funcao inicio()
    {
        inteiro v[5]
        inteiro i
        inteiro soma = 0
        inteiro maior

        para (i = 0; i < 5; i++)
        {
            leia(v[i])
        }

        maior = v[0]

        para (i = 0; i < 5; i++)
        {
            soma = soma + v[i]

            se (v[i] > maior)
            {
                maior = v[i]
            }
        }

        escreva("Soma = ", soma, "\n")
        escreva("Maior = ", maior)
    }
}
```

## 7) Tabuada

```portugol
programa
{
    funcao inicio()
    {
        inteiro n
        inteiro i

        leia(n)

        para (i = 1; i <= 10; i++)
        {
            escreva(n, " x ", i, " = ", n * i, "\n")
        }
    }
}
```

## 8) Fatorial

```portugol
programa
{
    funcao inicio()
    {
        inteiro n
        inteiro i
        inteiro fat = 1

        leia(n)

        se (n < 0)
        {
            escreva("Nao existe fatorial negativo")
            pare
        }

        para (i = 1; i <= n; i++)
        {
            fat = fat * i
        }

        escreva(n, "! = ", fat)
    }
}
```

## 9) Funcao dobro

```portugol
programa
{
    funcao inteiro dobro(inteiro x)
    {
        retorne x * 2
    }

    funcao inicio()
    {
        inteiro n
        leia(n)
        escreva("Dobro = ", dobro(n))
    }
}
```

## 10) Funcao media de 3 notas

```portugol
programa
{
    funcao real media3(real a, real b, real c)
    {
        retorne (a + b + c) / 3
    }

    funcao inicio()
    {
        real n1
        real n2
        real n3

        leia(n1, n2, n3)
        escreva("Media = ", media3(n1, n2, n3))
    }
}
```

## 11) Matriz 2x2

```portugol
programa
{
    funcao inicio()
    {
        inteiro m[2][2]
        inteiro i
        inteiro j
        inteiro soma = 0

        para (i = 0; i < 2; i++)
        {
            para (j = 0; j < 2; j++)
            {
                leia(m[i][j])
                soma = soma + m[i][j]
            }
        }

        escreva("Soma da matriz = ", soma)
    }
}
```

## 12) Registro Aluno

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

        leia(a.nome, a.idade, a.curso)

        escreva("Nome: ", a.nome, "\n")
        escreva("Idade: ", a.idade, "\n")
        escreva("Curso: ", a.curso)
    }
}
```

Se travou, revisa isso primeiro:

- bloco com `{}`
- tipo de variavel
- condicao/loop mal fechado
