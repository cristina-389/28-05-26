Aula de hoje 20/08/2026

Versionamento 

Professor Donald

git switch -c aluno-joao

git add README.md
git commit -m "Atividade Git - João"
git push -u origin aluno-joao

 # ATIVIDADE AVALIATIVA - GIT

**Disciplina:** Versionamento de Código
**Professor:** Donald
**Aluno(a):** _Yuri_________________________________
**Turma:** _____3DS__________ **Data:** 20/08/_2026___

## Situação-problema

Você começou a trabalhar em um projeto de desenvolvimento de um site. O projeto será controlado utilizando **Git**.

Responda às questões abaixo indicando o comando correto e explicando sua função.

### 1. Iniciando o projeto

Você criou uma pasta para o projeto e deseja começar a utilizar o Git nela.

**Qual comando deve utilizar? O que ele faz?**

Resposta: _O comando é git init. Ele inicia um novo repositório Git na pasta do projeto, permitindo que os arquivos e suas alterações sejam controlados pelo Git._____________________________________________________

### 2. Verificando alterações

Você modificou alguns arquivos e quer verificar quais foram alterados antes de continuar.

**Qual comando deve utilizar? O que ele mostra?**

Resposta: _O comando é git status. Ele mostra o estado atual do repositório, informando quais arquivos foram modificados, adicionados ou ainda não estão sendo rastreados._____________________________________________________

### 3. Criando uma nova área de trabalho

Você precisa desenvolver uma nova funcionalidade sem alterar diretamente a versão principal do projeto.

**Qual comando relacionado a branch pode ser utilizado? Para que serve uma branch?**

Resposta: Pode ser utilizado o comando git branch nome-da-branch ou, como foi utilizado na aula, git switch -c aluno-joao. Uma branch serve para criar uma ramificação do projeto, permitindo desenvolver uma nova funcionalidade sem alterar diretamente a versão principal.______________________________________________________

### 4. Enviando alterações

Você terminou seu trabalho local e precisa enviar as alterações para o repositório remoto.

**Qual comando deve utilizar? Explique sua função.**

O comando é git push. Sua função é enviar os commits e alterações do repositório local para o repositório remoto, como o GitHub._____________________________________________________

### 5. Recebendo alterações

Outro desenvolvedor atualizou o projeto no repositório remoto. Você precisa trazer essas alterações para seu computador.

**Qual comando deve utilizar? Explique sua função.**

Resposta: O comando é git pull. Sua função é buscar as alterações do repositório remoto e trazê-las para o repositório local, integrando-as ao projeto.______________________________________________________

## Desafio final

Complete o fluxo utilizando os comandos abaixo:

**git init | git status | git branch | git pull | git push**

a) Iniciar um repositório: ____git init__________________

b) Verificar o estado dos arquivos: _git status_____________________

c) Trabalhar com ramificações do projeto: _git branch_____________________

d) Buscar e integrar alterações do repositório remoto: ___git pull___________________

e) Enviar alterações para o repositório remoto: ____git push__________________

## Para pensar

Explique com suas palavras:

**Qual é a diferença entre `git pull` e `git push`?**

---
O comando git pull é utilizado para buscar e trazer as alterações do repositório remoto para o computador. Já o comando git push é utilizado para enviar as alterações feitas no computador para o repositório remoto.
---

