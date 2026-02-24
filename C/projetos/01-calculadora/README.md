# Mini-projeto 01 - Calculadora no terminal

## Objetivo

Juntar os assuntos iniciais num projeto pequeno que faz sentido.

## Explicacao curta

Aqui voce vai usar tudo junto: entrada, condicional, repeticao e funcoes.
Se esse projeto sair redondo, sua base ta boa.

## Codigo completo

Nao tem codigo pronto aqui de proposito.
A ideia e voce construir.

## Como compilar/executar

Quando criar `calculadora.c`:

```bash
gcc calculadora.c -o calculadora
```

- Windows: `calculadora.exe`
- Linux/macOS: `./calculadora`

## Saida esperada (exemplo)

```text
=== CALCULADORA ===
1) Somar
2) Subtrair
3) Multiplicar
4) Dividir
Escolha: 1
Digite dois numeros: 10 5
Resultado: 15.00
Deseja continuar? (s/n): n
```

## Erros comuns + como resolver

- divisao por zero sem tratamento
- menu em loop infinito
- entrada invalida quebrando fluxo

> Se ficar estranho, printa variavel no terminal e descobre onde a logica saiu do trilho.

## Exercicios

### Faceis (3)

1. Fazer soma e subtracao.
2. Adicionar multiplicacao.
3. Adicionar divisao com verificacao de zero.

### Medios (2)

1. Criar menu numerico.
2. Permitir repetir operacao sem fechar programa.

### Desafio (1)

1. Separar operacoes em funcoes e manter `main` limpo.

## Requisitos minimos

- ler dois numeros
- ler operacao (`+`, `-`, `*`, `/`)
- mostrar resultado
- tratar divisao por zero
- perguntar se quer continuar

## Extras opcionais

- historico de operacoes
- validacao melhor de entrada
- separar funcoes em outro arquivo

## Checklist

- [ ] Compila sem erro
- [ ] 4 operacoes funcionando
- [ ] Divisao por zero tratada
- [ ] Loop de continuidade funcionando
- [ ] Codigo organizado

## Entrega sugerida

1. Subir o codigo.
2. Colocar exemplos de entrada e saida no README.
3. Escrever o que deu mais trabalho e como resolveu.
