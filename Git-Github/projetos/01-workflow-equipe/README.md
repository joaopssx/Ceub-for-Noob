# Mini-projeto 01 - Workflow de equipe com Git + GitHub

## Objetivo

Treinar um fluxo real de equipe: branch, commit, PR, revisao e merge.

## Explicacao curta

Esse mini-projeto simula trabalho em squad.
A meta nao e so "dar push". E manter historico limpo e colaboracao organizada.

## Codigo completo

Nao tem codigo fixo aqui.
Voce pode usar qualquer projeto simples (ex: README com secoes) pra praticar fluxo.

## Como executar

Fluxo sugerido:

1. Criar repo no GitHub.
2. Clonar localmente.
3. Criar branch por tarefa (`feat/...`, `fix/...`).
4. Commits pequenos e claros.
5. Subir branch e abrir PR.
6. Revisar PR de colega.
7. Mergear quando estiver ok.

## Saida esperada (exemplo)

```text
- 2 branches de feature criadas
- 2 PRs abertos e revisados
- main atualizada com merge
```

## Erros comuns + como resolver

- direto na `main`
  - corrige fluxo: branch + PR
- PR sem descricao
  - inclua contexto e como testar
- conflito ignorado
  - resolva local, teste, depois push

## Exercicios

### Faceis (3)

1. Criar branch `feat/header` e commitar.
2. Criar branch `feat/footer` e commitar.
3. Subir as duas branches.

### Medios (2)

1. Abrir PR da `feat/header` com descricao.
2. Revisar PR da `feat/footer` e pedir ajuste.

### Desafio (1)

1. Gerar conflito intencional entre duas branches e resolver antes do merge final.

## Requisitos minimos

- usar branch por tarefa
- pelo menos 3 commits com mensagem clara
- pelo menos 1 PR revisado
- merge na `main` sem conflito pendente

## Extras opcionais

- usar labels nos PRs
- usar template de PR
- testar com `git rebase` em branch de feature

## Checklist

- [ ] Repositorio remoto criado
- [ ] Branches de feature criadas
- [ ] PRs abertos
- [ ] Revisao feita
- [ ] Merge final concluido
