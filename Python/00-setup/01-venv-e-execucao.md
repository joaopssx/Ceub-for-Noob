# 01 - Ambiente virtual e execucao

## Objetivo

Criar um projeto Python, montar `venv`, instalar pacote e executar script.

## Explicacao curta

`venv` isola dependencias por projeto.
Isso evita bagunca e conflito de versao.

## Codigo completo (`hello.py`)

```python
def main():
    # primeiro script do modulo
    print("Hello, Python!")


if __name__ == "__main__":
    main()
```

## Como criar e executar

### 1) criar pasta do projeto

```bash
mkdir aula-python
cd aula-python
```

### 2) criar ambiente virtual

Windows:

```bash
python -m venv .venv
```

Linux/macOS:

```bash
python3 -m venv .venv
```

### 3) ativar ambiente virtual

Windows (PowerShell):

```powershell
.\.venv\Scripts\Activate.ps1
```

Windows (CMD):

```bat
.\.venv\Scripts\activate.bat
```

Linux/macOS:

```bash
source .venv/bin/activate
```

Quando ativar, normalmente aparece `(.venv)` no comeco da linha do terminal.

### 4) criar arquivo e rodar

Crie `hello.py` com o codigo acima e execute:

Windows:

```bash
python hello.py
```

Linux/macOS:

```bash
python3 hello.py
```

## Saida esperada (exemplo)

```text
Hello, Python!
```

## Erros comuns + como resolver

### comando de ativacao falhou no PowerShell

Tente liberar execucao de script na sessao atual:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

Depois ativa de novo.

### `No module named ...`

Quase sempre pacote nao instalado no `venv` atual.

Instale com:

```bash
python -m pip install nome-do-pacote
```

ou:

```bash
python3 -m pip install nome-do-pacote
```

### esqueceu de ativar `venv`

Sinal classico: pacote existe, mas script nao encontra.
Ativa o ambiente e tenta de novo.

## Testes praticos

1. Troque a mensagem do print.
2. Crie um segundo arquivo `teste.py`.
3. Instale `requests` dentro do `venv` e confirme com `pip list`.

## Checklist final

- [ ] Criei `venv`
- [ ] Ativei `venv`
- [ ] Rodei `hello.py`
- [ ] Entendi a diferenca entre global e ambiente virtual
