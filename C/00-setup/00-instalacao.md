# 00 - Instalacao do ambiente C

## Objetivo

Deixar seu computador pronto pra criar, compilar e rodar programas em C.

## Explicacao curta

Pra programar em C, voce precisa de:

- editor de codigo (VS Code, por exemplo)
- compilador (`gcc` ou `clang`)

Sem compilador, o arquivo `.c` nao vira executavel.

> Dica de monitor: terminou uma etapa? testa no terminal na hora.

---

## Windows

### O que voce vai instalar

- Editor: VS Code
- Compilador: GCC

### Recomendado (mais simples): VS Code + MSYS2

Esse e o caminho mais tranquilo hoje pra Windows.

1. Instala o VS Code:
   - https://code.visualstudio.com/
2. Instala o MSYS2:
   - https://www.msys2.org/
3. Abre o app `MSYS2 UCRT64`.
4. Atualiza pacotes:

```bash
pacman -Syu
```

5. Se ele pedir pra fechar o terminal, fecha e abre `MSYS2 UCRT64` de novo.
6. Continua a atualizacao:

```bash
pacman -Su
```

7. Instala o compilador:

```bash
pacman -S --needed base-devel mingw-w64-ucrt-x86_64-gcc
```

8. Testa:

```bash
gcc --version
```

Se aparecer versao, ta certo.

### PATH no Windows (a parte que mais da erro)

Se `gcc` nao for reconhecido, quase sempre e PATH.

1. Procura por `Variaveis de ambiente` no iniciar.
2. Entra em `Variaveis de Ambiente`.
3. Edita a variavel `Path`.
4. Adiciona este caminho:

```text
C:\msys64\ucrt64\bin
```

5. Salva tudo.
6. Fecha e abre o terminal de novo.
7. Roda `gcc --version`.

> Se o terminal falar que nao reconhece o comando, e quase sempre PATH.

### Alternativa (mais simples, menos flexivel): Code::Blocks + MinGW

1. Baixa a versao do Code::Blocks que ja vem com MinGW.
2. Instala normalmente.
3. Abre e cria um projeto console.
4. Roda o exemplo inicial.

Funciona bem pra inicio, mas o mercado usa mais VS Code + terminal.

### Opcional (mais avancado): WSL

Se voce quer estudar em ambiente Linux dentro do Windows:

1. Abre PowerShell como admin.
2. Roda:

```powershell
wsl --install
```

3. Reinicia o PC.
4. No Ubuntu (WSL), instala:

```bash
sudo apt update
sudo apt install -y build-essential
```

5. Testa:

```bash
gcc --version
```

---

## Linux

### O que voce vai instalar

- Editor (o que voce preferir)
- GCC

### Recomendado (mais simples): usar compilador da distro

#### Debian/Ubuntu

```bash
sudo apt update
sudo apt install -y build-essential
```

#### Fedora

```bash
sudo dnf groupinstall "Development Tools"
sudo dnf install -y gcc
```

#### Arch

```bash
sudo pacman -S --needed base-devel gcc
```

### Alternativa (mais avancada): clang

Se voce quiser testar com clang:

- Debian/Ubuntu:

```bash
sudo apt install -y clang
```

- Fedora:

```bash
sudo dnf install -y clang
```

- Arch:

```bash
sudo pacman -S --needed clang
```

### Como confirmar

```bash
gcc --version
```

ou

```bash
clang --version
```

---

## macOS

### O que voce vai instalar

- Editor
- Compilador (`clang` ou `gcc`)

### Recomendado (mais simples): Xcode Command Line Tools

1. Abre Terminal.
2. Roda:

```bash
xcode-select --install
```

3. Confirma a instalacao.
4. Testa:

```bash
clang --version
```

No macOS isso ja resolve quase tudo.

### Alternativa (mais avancada): Homebrew + GCC

```bash
brew install gcc
gcc --version
```

---

## Se deu ruim

### `gcc` nao encontrado

- Windows: PATH nao configurado.
- Linux: pacote nao instalado.
- macOS: Command Line Tools nao instaladas.

### PATH no Windows

Erro classico: colocou caminho errado ou nao reiniciou o terminal.

Confere letra por letra:

```text
C:\msys64\ucrt64\bin
```

### Permissao no Linux

Se aparecer `permission denied`, tenta compilar/rodar numa pasta sua (`~/Documentos`, `~/projetos`).

### `xcode-select` no macOS

Se der problema:

```bash
sudo xcode-select --reset
xcode-select --install
```

---

## Checklist rapido

- [ ] Tenho editor instalado
- [ ] Tenho compilador instalado
- [ ] `gcc --version` (ou `clang --version`) funciona

## Proximo passo

- [01 - Compilar e executar](./01-compilar-executar.md)
