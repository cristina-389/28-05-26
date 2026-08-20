Aula de hoje 20/08/2026 



NOTA --- 10

Versionamento 

Professor Donald

git switch -c aluno-joao

git add README.md
git commit -m "Atividade Git - João"
git push -u origin aluno-joao

 # ATIVIDADE AVALIATIVA - GIT

**Disciplina:** Versionamento de Código
**Professor:** Donald
**Aluno(a):** João Paulo da Silva de Oliveira
**Turma:** 3°DS **Data:** 20/08/2026

## Situação-problema

Você começou a trabalhar em um projeto de desenvolvimento de um site. O projeto será controlado utilizando **Git**.

Responda às questões abaixo indicando o comando correto e explicando sua função.

### 1. Iniciando o projeto

Você criou uma pasta para o projeto e deseja começar a utilizar o Git nela.

**Qual comando deve utilizar? O que ele faz?**

Resposta: git init
Ele inicializa o Git na pasta. Cria a pasta oculta .git e começa a controlar as versões dos arquivos daquele projeto.

### 2. Verificando alterações

Você modificou alguns arquivos e quer verificar quais foram alterados antes de continuar.

**Qual comando deve utilizar? O que ele mostra?**

Resposta: git status
Ele mostra o estado atual dos arquivos: quais foram modificados, quais estão prontos para "commit" e quais ainda não estão sendo monitorados pelo Git.

### 3. Criando uma nova área de trabalho

Você precisa desenvolver uma nova funcionalidade sem alterar diretamente a versão principal do projeto.

**Qual comando relacionado a branch pode ser utilizado? Para que serve uma branch?**

Resposta: git switch -c nome-da-branch
Uma branch serve para criar uma "cópia" do projeto para trabalhar em uma nova funcionalidade sem bagunçar a versão principal main. Exemplo: git switch -c aluno-joao

### 4. Enviando alterações

Você terminou seu trabalho local e precisa enviar as alterações para o repositório remoto.

**Qual comando deve utilizar? Explique sua função.**

Resposta: git push -u origin nome-da-branch
Ele envia os commits que você fez localmente para o repositório remoto, como o GitHub. O -u origin define essa branch como padrão para os próximos pushes. Exemplo: git push -u origin aluno-joao

### 5. Recebendo alterações

Outro desenvolvedor atualizou o projeto no repositório remoto. Você precisa trazer essas alterações para seu computador.

**Qual comando deve utilizar? Explique sua função.**

Resposta: git pull
Ele busca as alterações mais novas que estão no repositório remoto e já junta/integra com os arquivos do seu computador.

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

git push é para enviar suas alterações do computador para o repositório remoto.
git pull é para baixar as alterações que outras pessoas fizeram no repositório remoto para o seu computador.
Resumindo: push = sobe, pull = desce.



Pergunta-problema

Um aluno está desenvolvendo um site em equipe. Ele criou uma pasta para o projeto, mas ainda não iniciou o controle de versão. Depois, precisa verificar os arquivos alterados, criar uma branch chamada nova-pagina para trabalhar sem modificar a main, buscar as atualizações feitas pelos colegas e, ao terminar, enviar seu trabalho para o GitHub.

Explique, na ordem correta, quais comandos Git ele deve utilizar e qual é a função de cada comando nesse processo.

Resposta: Para resolver a situação na ordem correta, o aluno deve usar os seguintes comandos Git:

*1. `git init`*  
*Função:* Inicia o controle de versão na pasta do projeto. Ele cria a pasta `.git` e passa a monitorar os arquivos para guardar o histórico de alterações.

*2. `git status`*  
*Função:* Verifica quais arquivos foram criados, modificados ou excluídos. Mostra o estado atual do projeto antes de salvar as alterações.

*3. `git switch -c nova-pagina`*  
*Função:* Cria uma nova branch chamada `nova-pagina` e já muda para ela.  
Serve para trabalhar na nova funcionalidade sem mexer na branch principal `main`. Assim a equipe não quebra o site enquanto desenvolve.

*4. `git pull`*  
*Função:* Busca as atualizações mais recentes que os colegas fizeram no repositório remoto e já junta com o código local.  
Importante rodar isso antes de começar a trabalhar e também antes de enviar, para evitar conflitos.

*5. `git add .`*  
*Função:* Adiciona todos os arquivos alterados para a "área de preparação". É o passo antes do commit.  
Obs: poderia ser `git add nome-do-arquivo` também.

*6. `git commit -m "Criação da nova página"`*  
*Função:* Salva as alterações na branch local com uma mensagem explicando o que foi feito.

*7. `git push -u origin nova-pagina`*  
*Função:* Envia a branch `nova-pagina` com todos os commits para o GitHub. O `-u origin` define essa branch como padrão para os próximos envios.

*Resumo da ordem:*  
`git init` → `git status` → `git pull` → `git switch -c nova-pagina` → `git add` → `git commit` → `git push`
