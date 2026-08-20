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
**Aluno(a):** Cristina
**Turma:** 3DS **Data:** 20/08/2026

## Situação-problema

Você começou a trabalhar em um projeto de desenvolvimento de um site. O projeto será controlado utilizando **Git**.

Responda às questões abaixo indicando o comando correto e explicando sua função.

### 1. Iniciando o projeto

Você criou uma pasta para o projeto e deseja começar a utilizar o Git nela.

**Qual comando deve utilizar? O que ele faz?**

Resposta: "git init" ele inicializa um novo repositório Git na pasta, cria uma pasta oculta .git que passa a controlar o versionamento dos arquivos daquele diretório.

### 2. Verificando alterações

Você modificou alguns arquivos e quer verificar quais foram alterados antes de continuar.

**Qual comando deve utilizar? O que ele mostra?**

Resposta: "git status" ele mostra o estado atual dos arquivos: quais faram modificados, quais estão prontos para commit "staged", e quais ainda não estão sendo rastreado pelo Git.

### 3. Criando uma nova área de trabalho

Você precisa desenvolver uma nova funcionalidade sem alterar diretamente a versão principal do projeto.

**Qual comando relacionado a branch pode ser utilizado? Para que serve uma branch?**

Resposta: "git branch nova-funcionalidade" ou "git checkout -b nova-funcionalidade", uma branch serve para criar uma "cópia" do projeto para trabalhar em uma nova funcionalidade ou correção isolada, sem bagunçar a branch principal main/master. Depois você junta tudo com merge.

### 4. Enviando alterações

Você terminou seu trabalho local e precisa enviar as alterações para o repositório remoto.

**Qual comando deve utilizar? Explique sua função.**

Resposta: "git push" ele envia os commits que você fez localmente para o repositório remoto, como GitHub ou GitLab, torna suas alterações disponíveis para o resto da equipe.

### 5. Recebendo alterações

Outro desenvolvedor atualizou o projeto no repositório remoto. Você precisa trazer essas alterações para seu computador.

**Qual comando deve utilizar? Explique sua função.**

Resposta: "git pull" ele busca "fetch" as alterações do repositório remoto e já integra "merge" com sua branch local. É usado para manter seu projeto atualizado com o que os outros fizeram.

## Desafio final

Complete o fluxo utilizando os comandos abaixo:

**git init | git status | git branch | git pull | git push**

a) Iniciar um repositório: git init

b) Verificar o estado dos arquivos: git status

c) Trabalhar com ramificações do projeto: git branch

d) Buscar e integrar alterações do repositório remoto: git pull

e) Enviar alterações para o repositório remoto: git push

## Para pensar

Explique com suas palavras:

**Qual é a diferença entre `git pull` e `git push`?**

---
git push é pra enviar.
Quando você termina algo na sua máquina e quer mandar pro repositório remoto, tipo GitHub. É você colocando suas alterações lá pra todo mundo acessar.git pull é pra receber.
Quando outra pessoa já mandou coisa nova pro repositório. Você usa pull pra baixar essas atualizações e deixar seu projeto igual ao da nuvem.
---

deve criar uma branch com seu primeiro nome e sobrenome, responder a atividade no README.md e enviar as alterações para sua própria branch. Não é permitido fazer alterações diretamente na branch main.



https://www.open.edu/openlearn/pluginfile.php/4488604/mod_fullscreenresource/content/1/password_check/index.html

https://coveryourtracks.eff.org/
