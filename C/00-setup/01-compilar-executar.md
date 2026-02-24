# 01 - Compilar e executar no terminal

## Objetivo

Criar `hello.c`, compilar e rodar no Windows, Linux e macOS.

## Explicacao curta

Fluxo em C e sempre esse:

1. escrever `.c`
2. compilar
3. executar

No comeco parece mais manual, depois vira rotina.

## Codigo completo (`hello.c`)

```c
#include <stdio.h>

int main(void) {
    // ponto de entrada do programa
    printf("Hello, World!\\n");
    return 0;
}
```

## Como criar o arquivo

1. Cria uma pasta tipo `aula-c`.
2. Dentro dela, cria `hello.c`.
3. Cola o codigo e salva.

> Se estiver no Windows, evita nomes de pasta complicados no inicio.

## Como compilar/executar

Comando base:

```bash
gcc arquivo.c -o programa
```

Exemplo real:

```bash
gcc hello.c -o hello
```

### O que esse comando quer dizer

- `gcc`: compilador
- `hello.c`: arquivo de entrada
- `-o hello`: nome do executavel

## Rodando em cada sistema

### Windows

```bash
gcc hello.c -o hello
hello.exe
```

No PowerShell tambem funciona:

```bash
.\hello.exe
```

### Linux/macOS

```bash
gcc hello.c -o hello
./hello
```

## `programa.exe` vs `./programa` (na pratica)

- No Windows: voce chama `programa.exe`.
- No Linux/macOS: voce chama `./programa`.

O `./` significa "roda o arquivo daqui da pasta atual".

## Saida esperada (exemplo)

```text
Hello, World!
```

## Erros comuns + como resolver

### `undefined reference to main`

Causa mais comum:

- arquivo sem `main`
- nome da funcao errado

Confere se existe isso:

```c
int main(void) {
    return 0;
}
```

### `permission denied`

Mais comum no Linux/macOS:

```bash
chmod +x hello
./hello
```

### `no such file or directory`

Normalmente:

- voce nao esta na pasta certa
- nome do arquivo foi digitado errado
- executavel nao foi criado ainda

Comandos uteis:

- Windows: `dir`
- Linux/macOS: `ls`

## Testes praticos

1. Troca a frase e roda de novo.
2. Cria `teste.c` e gera `teste`.
3. Tenta compilar um nome errado e le o erro.

## Checklist final

- [ ] Criei um `.c`
- [ ] Compilei com `gcc arquivo.c -o programa`
- [ ] Rodei no meu sistema
- [ ] Entendi `.exe` vs `./programa`
- [ ] Resolvi pelo menos 1 erro sozinho
