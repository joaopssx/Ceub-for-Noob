# 00 - Instalacao do ambiente Python

## Objetivo

Deixar seu ambiente pronto pra criar e executar scripts Python sem dor de cabeca.

## Explicacao curta

Pra estudar Python voce precisa de:

- Python instalado
- terminal funcionando
- editor (VS Code, por exemplo)

## Windows

### O que voce vai instalar

- Python 3
- VS Code (opcional, mas recomendado)

### Recomendado: Python oficial + VS Code

1. Baixe Python em: https://www.python.org/downloads/
2. Abra o instalador.
3. Marque a opcao `Add Python to PATH`.
4. Clique em `Install Now`.
5. No final, feche o instalador.

Agora testa no terminal:

```bash
python --version
```

Se esse comando falhar, tenta:

```bash
py --version
```

### Alternativa: instalar com winget

No PowerShell:

```powershell
winget install Python.Python.3.12
```

Depois testa:

```bash
python --version
```

### VS Code (recomendado)

1. Instale: https://code.visualstudio.com/
2. Extensao que vale muito: `Python` (Microsoft)

### Se deu ruim no Windows

- `python nao e reconhecido`
  - quase sempre e PATH
  - reinstala marcando `Add Python to PATH`
- comando abre Microsoft Store
  - desative alias de app ou use `py`
- pasta com espaco/nome estranho
  - prefira pastas simples no comeco (`C:\dev\python`)

## Linux

### O que voce vai instalar

- Python 3
- `pip`
- `venv`

### Debian/Ubuntu

```bash
sudo apt update
sudo apt install -y python3 python3-pip python3-venv
```

### Fedora

```bash
sudo dnf install -y python3 python3-pip
```

### Arch

```bash
sudo pacman -S --needed python python-pip
```

### Confirmar instalacao

```bash
python3 --version
```

E opcionalmente:

```bash
python3 -m pip --version
```

## macOS

### O que voce vai instalar

- Python 3
- `pip`

### Recomendado: Homebrew

```bash
brew install python
```

Testa:

```bash
python3 --version
```

### Alternativa: instalador oficial

Baixe em: https://www.python.org/downloads/

Depois teste no terminal:

```bash
python3 --version
```

## Se deu ruim

### `python` ou `python3` nao encontrado

- fecha e abre o terminal
- testa ambos: `python --version` e `python3 --version`
- no Windows, teste `py --version`

### `pip` nao funciona

Tenta:

```bash
python -m pip --version
```

ou:

```bash
python3 -m pip --version
```

### erro de permissao no Linux/macOS

Evita instalar pacote global sem necessidade.
Usa ambiente virtual (vamos fazer isso no proximo arquivo).

## Checklist rapido

- [ ] Python instalado
- [ ] Terminal reconhece `python` ou `python3`
- [ ] VS Code pronto (opcional)

## Proximo passo

- [01 - venv e execucao](./01-venv-e-execucao.md)
