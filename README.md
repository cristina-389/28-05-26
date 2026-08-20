# Atividade Avaliativa - Git

**Disciplina:** Versionamento de Código  
**Professor:** Donald  
**Aluno(a):** Cristina  
**Turma:** 3DS  
**Data:** 20/08/2026
NOTA---10
## Situação-problema

Você começou a trabalhar em um projeto de desenvolvimento de um site. O projeto será controlado utilizando **Git**.

Responda às questões abaixo indicando o comando correto e explicando sua função.

### 1. Iniciando o projeto

Você criou uma pasta para o projeto e deseja começar a utilizar o Git nela.

Qual comando deve utilizar? O que ele faz?

Resposta: `git init` — inicializa um novo repositório Git na pasta atual. Cria a pasta oculta `.git` que passa a controlar o versionamento dos arquivos desse diretório.

### 2. Verificando alterações

Você modificou alguns arquivos e quer verificar quais foram alterados antes de continuar.

Qual comando deve utilizar? O que ele mostra?

Resposta: `git status` — mostra o estado atual dos arquivos: quais foram modificados, quais estão staged (prontos para commit) e quais não estão sendo rastreados pelo Git.

### 3. Criando uma nova área de trabalho (branch)

Você precisa desenvolver uma nova funcionalidade sem alterar diretamente a versão principal do projeto.

Qual comando relacionado a branch pode ser utilizado? Para que serve uma branch?

Resposta: Para criar e mudar para uma nova branch você pode usar:
- `git switch -c nova-funcionalidade` (moderno), ou
- `git checkout -b nova-funcionalidade` (alternativa ainda usada).

Uma branch serve para isolar trabalhos (nova funcionalidade, correção de bug) sem afetar a branch principal (por exemplo `main` ou `master`). Também é possível apenas criar a branch sem trocar para ela com `git branch nome-da-branch`.

### 4. Preparando e enviando alterações

Você terminou seu trabalho local e precisa enviar as alterações para o repositório remoto.

Quais comandos deve utilizar? Explique suas funções.

Resposta:
- `git add <arquivo>` — adiciona arquivos à área de stage (prepara para commit). Use `git add .` para adicionar todas as alterações.
- `git commit -m "mensagem"` — cria um commit com as alterações staged e registra a mensagem explicativa.
- `git push` — envia os commits locais para o repositório remoto. Se for a primeira vez que envia uma branch criada localmente, use `git push -u origin nome-da-branch` para definir o upstream.

### 5. Recebendo alterações

Outro desenvolvedor atualizou o projeto no repositório remoto. Você precisa trazer essas alterações para seu computador.

Qual comando deve utilizar? Explique sua função.

Resposta: `git pull` — busca (fetch) as alterações do repositório remoto e integra (merge) com sua branch local. Alternativamente, para mais controle, use `git fetch` seguido de `git merge` ou `git rebase`.

## Desafio final

Complete o fluxo utilizando os comandos abaixo:

`git init | git status | git branch | git pull | git push`

a) Iniciar um repositório: `git init`

b) Verificar o estado dos arquivos: `git status`

c) Trabalhar com ramificações do projeto: `git branch` (ou `git switch -c ...` para criar+trocar)

d) Buscar e integrar alterações do repositório remoto: `git pull`

e) Enviar alterações para o repositório remoto: `git push`

## Para pensar

Explique com suas palavras: Qual é a diferença entre `git pull` e `git push`?

Resposta:
- `git push` envia seus commits locais ao repositório remoto (coloca suas alterações na nuvem).
- `git pull` traz do remoto as alterações de outras pessoas e as incorpora na sua cópia local (atualiza seu repositório com o que está no remoto).

---

Observações adicionais:
- Corrigi erros de digitação e clareei algumas explicações.
- Removi trechos incompletos e instruções confusas (por exemplo o trecho truncado "Não é permitido fazer alterações diretamente na branc[...]").
- Se o exercício pede que a branch seja criada com "primeiro nome + sobrenome", substitua `nome-da-branch` por `cristina-sobrenome` (ex.: `cristina-silva`) conforme o sobrenome real.
