# Gabarito comentado - Lista 01 (Git + GitHub)

Nao precisa decorar comando na forca.
Entende o fluxo e pratica.

## Como usar esse gabarito

1. Tenta sozinho.
2. Compara com seu fluxo.
3. Se algo der diferente, usa `git status` pra diagnosticar.

## 1) Criar repositorio local

```bash
mkdir treino-git
cd treino-git
git init
```

## 2) Criar README e commitar

```bash
echo "# Treino Git" > README.md
git add README.md
git commit -m "chore: cria README inicial"
```

## 3) Ver historico

```bash
git log --oneline
```

## 4) Criar branch e commitar

```bash
git checkout -b feat/teste

echo "linha nova" >> README.md
git add README.md
git commit -m "feat: adiciona linha no README"
```

## 5) Merge na main

```bash
git checkout main
git merge feat/teste
```

## 6) Subir para GitHub

```bash
git remote add origin https://github.com/SEU-USUARIO/SEU-REPO.git
git branch -M main
git push -u origin main
```

## 7) Pull apos alteracao no GitHub

```bash
git pull origin main
```

## 8) Abrir PR

Fluxo de terminal:

```bash
git checkout -b feat/nova-tarefa
git add .
git commit -m "feat: nova tarefa"
git push -u origin feat/nova-tarefa
```

Depois abre PR no site do GitHub.

## 9) Atualizar PR

```bash
git add .
git commit -m "fix: ajusta feedback da revisao"
git push
```

## 10) Simular e resolver conflito

Resumo do fluxo:

```bash
git merge feat/a
git merge feat/b
# resolver arquivo
git add README.md
git commit -m "fix: resolve conflito"
```

## 11) Ajustar URL do remote

```bash
git remote set-url origin https://github.com/SEU-USUARIO/REPO-CERTO.git
```

Valida com:

```bash
git remote -v
```

## 12) Clonar e sincronizar

```bash
git clone https://github.com/SEU-USUARIO/SEU-REPO.git
cd SEU-REPO

git pull origin main
# altera algo
# commit
git push origin main
```

## Resumo rapido de sobrevivencia

Se travou, roda nessa ordem:

1. `git status`
2. `git branch`
3. `git log --oneline --graph --all`

Quase sempre isso ja mostra o problema.
