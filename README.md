[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/zHqjFsRx)
# Diagnóstico de retomada - Teoria da Computação

Esta atividade serve para mapear o que você já domina sobre linguagens formais, autômatos, gramáticas e computabilidade.

Responda individualmente. Use suas palavras. Se usar IA depois da primeira tentativa, registre o uso na seção 7.

## 1. Mapa do que eu lembro

Marque cada tópico como: lembro bem, lembro parcialmente, não lembro, nunca vi ou não tenho certeza.

- alfabeto: lembro bem
- cadeia: lembro parcialmente
- linguagem: lembro bem
- gramática: lembro parcialmente
- autômato finito: lembro parcialmente
- linguagem regular: lembro parcialmente
- linguagem livre de contexto: não lembro
- linguagem sensível ao contexto: não lembro
- linguagem irrestrita: lembro parcialmente
- hierarquia de Chomsky:  não lembro
- computabilidade:  não lembro
- máquina de Turing: lembro parcialmente

## 2. Definições com exemplo

Explique, com suas palavras e com um exemplo simples, usando o alfabeto `Sigma = {a, b}`.

1. O que é um alfabeto?

Resposta: É um conjunto de simboblos usado para criar palavras e/ou cadeias
Exemplo: A = {a,b}, "a" pertence ao alfabeto mas "c" não.

2. O que é uma cadeia?
                                                                                                                     Resposta: É uma sequencia de simbolos de um alfabeto            
Exemplo: Usando A = {a,b}. Temos; "a", "ab", "bba", Etc...                                                                                                                                                      
3. O que é uma linguagem?                                                                                                                                                                                                                 
Resposta: É um conjunto de cadeias 
Exemplo: Uma linguagem B = {a, ab, bba}

4. O que é uma gramática?

Resposta: Um conjunto de regras usado para criar cadeias.
Exemplo: Usando A = {a,b}. 
S -> aB
B -> b
Começamos com S.

Aplicando a primeira regra:
S -> aB
Depois aplicamos:
B -> b
Então obtemos:
ab

## 3. Linguagens

Considere as linguagens:

```text
L1 = { w em {0,1}* | w termina com 01 }
L2 = { a^n b^n | n >= 0 }
L3 = { a^n b^n c^n | n >= 0 }
```

Para cada linguagem:

1. escreva três palavras que pertencem à linguagem;
Resposta: (01,101,1101)  
2. escreva duas palavras que não pertencem;
Resposta: (10,111)   
3. diga, se souber, em qual classe ela provavelmente se encaixa;
Não lembro do assunto direito.
4. explique o motivo em linguagem simples.
Não sei explicar direito.

## 4. Autômato finito

Considere o autômato abaixo, sobre o alfabeto `{0,1}`:

```text
Estados: q0, q1, q2
Estado inicial: q0
Estado final: q2

Transições:
q0 --0--> q1
q0 --1--> q0
q1 --0--> q1
q1 --1--> q2
q2 --0--> q1
q2 --1--> q0
```

Responda:

1. Qual linguagem esse autômato parece reconhecer?
Resposta: Acho, que palavras que teminam em 01   
2. Execute manualmente as cadeias abaixo e diga se aceita ou rejeita:
   - `01`: Aceita
q0 --0--> q1
q1 --1--> q2
   - `101`: Aceita
q0 --1--> q0
q0 --0--> q1
q1 --1--> q2
   - `100`: Rejeita
q0 --1--> q0
q0 --0--> q1
q1 --0--> q1
   - `1101`: Aceita
q0 --1--> q0
q0 --1--> q0
q0 --0--> q1
q1 --1--> q2
   - `111`: Rejeita
q0 --1--> q0
q0 --1--> q0
q0 --1--> q0

3. Monte uma tabela curta mostrando o caminho dos estados para pelo menos duas cadeias.
Eu não sei montar a tabela

## 5. Gramática

Considere a gramática:

```text
S -> aS
S -> b
```

Responda:

1. Gere cinco cadeias produzidas por essa gramática.
Resposta: (b,ab,aab,aaab,aaaab)
2. Descreva a linguagem em palavras.
Não sei explicar muito bem   
3. Essa gramática parece regular, livre de contexto ou outra classe? Justifique de forma simples.
Não lembro do assunto   

## 6. Ponto de dificuldade

Escolha um tópico da lista inicial e escreva: Alfabeto

1. o que você entende dele;
Resposta: Consigo compreender bem ele, acho que pelo fato dele ser tecnicamento o assunto inicial e o mais facil dentre os outros  
2. onde você se confunde;
Responde: Normalmente quando começa a incluir linguagem fica um pouco mais dificil pra mim
3. que tipo de explicação ajudaria: desenho, exemplo, exercício guiado, analogia, prova passo a passo ou lista curta.
Resposta: Acho que talvez exercicio guiado e prova passo a passo
## 7. Uso de IA, se houver

Se você usou IA depois da primeira tentativa, registre:

Pergunta feita: 2.4
Resumo da resposta: Oque é gramatica e exemplo
Como eu verifiquei: Pesquisei exemplos, não sabia como demonstrar direito
O que eu alterei na minha resposta: O alfabeto, os simbolos, e algumas palavras
O que ainda não entendi: Ainda não sei mt bem como demonstrar

Pergunta feita: 4.2
Resumo da resposta: Demonstrar as cadeias
Como eu verifiquei: Eu pedi pra ele demonstrar as cadeias dadas, porque eu não sabia como demonstrar
O que eu alterei na minha resposta: Coloquei as demonstrações, eu conseguia determinar se era aceita ou não, mas não sabia demonstrar
O que ainda não entendi: Como demonstrar


## Submissão no Moodle

Depois de finalizar, copie no Moodle:

```text
Repositório:
Commit final:
Autoavaliação: nível atual, maior dificuldade e tópico que precisa ser retomado.
```
