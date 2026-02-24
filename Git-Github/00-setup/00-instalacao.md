# 00 - Instalacao do Git

## Objetivo

Instalar Git no seu sistema e validar que o terminal reconhece o comando.

## Explicacao curta

Sem Git instalado, nada nesse modulo funciona.
Entao faz essa parte com calma e testa no final.

## Codigo completo

Comandos de verificacao:

```bash
git --version
```

## Como executar

### Windows

#### Recomendado: Git for Windows

1. Baixe: https://git-scm.com/download/win
2. Rode o instalador (pode ir de `Next` em quase tudo).
3. No fim, abra `Git Bash`.
4. Rode:

```bash
git --version
```

Se aparecer versao, acabou.

#### Alternativa: winget

```powershell
winget install Git.Git
```

Depois:

```bash
git --version
```

### Linux

#### Debian/Ubuntu

```bash
sudo apt update
sudo apt install -y git
```

#### Fedora

```bash
sudo dnf install -y git
```

#### Arch

```bash
sudo pacman -S --needed git
```

Teste:

```bash
git --version
```

### macOS

#### Recomendado: Xcode Command Line Tools

```bash
xcode-select --install
git --version
```

#### Alternativa: Homebrew

```bash
brew install git
git --version
```

## Saida esperada (exemplo)

```text
git version 2.xx.x
```

## Erros comuns + como resolver

### `git: command not found`

- Git nao foi instalado
- ou terminal nao foi reiniciado

### Windows instalou, mas comando nao funciona

Fecha e abre terminal.
Se continuar, reinstala Git for Windows com opcoes padrao.

### macOS pedindo para instalar developer tools

Aceita a instalacao e espera terminar.

## Exercicios

### Faceis (3)

1. Instalar Git no seu sistema.
2. Rodar `git --version`.
3. Tirar print mental da versao e anotar.

### Medios (2)

1. Instalar tambem no segundo sistema (ex: WSL ou outra maquina).
2. Comparar versao entre os ambientes.

### Desafio (1)

1. Explicar para colega, em 3 passos, como instalar Git do zero.
