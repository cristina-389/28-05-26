Aula de hoje: 20/08/2026
NOTA: 10

# ATIVIDADE AVALIATIVA - GIT

**Disciplina:** Versionamento de Código
**Professor:** Donald
**Aluno(a):** Yuri
**Turma:** 3DS	**Data:** 20/08/2026

## Objetivo
Responder às questões práticas sobre uso básico do Git e melhorar este README com explicações claras, exemplos de comandos e um fluxo sugerido para uso em equipe.

---

## Situação-problema
Você começou a trabalhar em um projeto de desenvolvimento de um site. O projeto será controlado utilizando **Git**.

Responda às questões abaixo indicando o comando correto e explicando sua função.

### 1. Iniciando o projeto
Você criou uma pasta para o projeto e deseja começar a utilizar o Git nela.

Qual comando deve utilizar? O que ele faz?

Resposta:
- Comando: `git init`
- O que faz: inicializa um novo repositório Git local na pasta atual. Cria o diretório oculto `.git` que passa a armazenar o histórico de versões, possibilitando criar commits, branches e rastrear alterações.

Exemplo:
```
mkdir meu-projeto
cd meu-projeto
git init
```

---

### 2. Verificando alterações
Você modificou alguns arquivos e quer verificar quais foram alterados antes de continuar.

Qual comando deve utilizar? O que ele mostra?

Resposta:
- Comando: `git status`
- O que faz: mostra o estado do repositório em relação à área de preparação (staging) e ao último commit. Lista arquivos modificados, novos não rastreados, arquivos prontos para commit e o branch atual.

Exemplo:
```
git status
```

---

### 3. Criando uma nova área de trabalho (branch)
Você precisa desenvolver uma nova funcionalidade sem alterar diretamente a versão principal do projeto.

Qual comando relacionado a branch pode ser utilizado? Para que serve uma branch?

Resposta:
- Comandos: `git branch nome-da-branch` (cria a branch) e `git switch -c nome-da-branch` (cria e já troca para a branch). Também se pode usar `git checkout -b nome-da-branch` em versões antigas do Git.
- Para que serve: uma branch (ramificação) permite trabalhar isoladamente em uma linha de desenvolvimento sem afetar o branch principal (ex.: `main` ou `master`). Facilita o desenvolvimento de features, correções e experimentos, e depois integrações via merge ou pull request.

Exemplo:
```
# criar e trocar para a branch 'feature-login'
git switch -c feature-login
```

---

### 4. Enviando alterações
Você terminou seu trabalho local e precisa enviar as alterações para o repositório remoto.

Qual comando deve utilizar? Explique sua função.

Resposta:
- Comando: `git push [remote] [branch]`
- O que faz: envia commits do repositório local para o repositório remoto (por exemplo, `origin`). Se for a primeira vez que envia a branch, use `git push -u origin nome-da-branch` para configurar o upstream.

Exemplo:
```
# enviar a branch atual para o remoto origin e definir upstream
git push -u origin feature-login
```

---

### 5. Recebendo alterações
Outro desenvolvedor atualizou o projeto no repositório remoto. Você precisa trazer essas alterações para seu computador.

Qual comando deve utilizar? Explique sua função.

Resposta:
- Comando: `git pull [remote] [branch]`
- O que faz: busca (fetch) as alterações do remoto e tenta integrar (merge) automaticamente ao branch atual. Pode causar conflitos se houver alterações divergentes; nesses casos é necessário resolver conflitos manualmente.

Observação: em fluxos colaborativos é comum usar `git fetch` seguido de `git merge` ou `git rebase` para ter mais controle sobre a integração.

Exemplo:
```
# atualizar o branch atual com as alterações do remoto origin
git pull origin main
```

---

## Desafio final
Complete o fluxo utilizando os comandos abaixo:

`git init | git status | git branch | git pull | git push`

a) Iniciar um repositório: git init

b) Verificar o estado dos arquivos: git status

c) Trabalhar com ramificações do projeto: git branch (ou git switch -c / git checkout -b)

d) Buscar e integrar alterações do repositório remoto: git pull

e) Enviar alterações para o repositório remoto: git push

---

## Para pensar
Explique com suas palavras: Qual é a diferença entre `git pull` e `git push`?

Resposta:
- `git pull` traz (download) alterações do repositório remoto para o repositório local e tenta integrá-las ao branch atual.
- `git push` envia (upload) seus commits locais para o repositório remoto, tornando suas alterações disponíveis para outros colaboradores.

---

## Pergunta-problema (fluxo recomendado)
Um aluno está desenvolvendo um site em equipe. Ele criou uma pasta para o projeto, mas ainda não iniciou o controle de versão. Depois, precisa verificar os arquivos alterados, criar uma branch chamada `aluno-joao`, trabalhar, commitar e enviar para o remoto. Explique, na ordem correta, quais comandos Git ele deve utilizar e qual é a função de cada comando nesse processo.

Fluxo sugerido (com comandos):

1. Iniciar repositório local:
```
git init
```
2. Verificar o estado dos arquivos:
```
git status
```
3. Adicionar arquivos desejados à área de stage (preparar para commit):
```
git add README.md
# ou para adicionar tudo
git add .
```
4. Fazer o commit com mensagem explicativa:
```
git commit -m "Atividade Git - João"
```
5. Criar e trocar para a branch de trabalho (se ainda não existir):
```
git switch -c aluno-joao
# ou: git branch aluno-joao
# seguido de: git switch aluno-joao
```
6. Caso ainda não tenha configurado o repositório remoto, adicionar o remoto (uma vez):
```
git remote add origin https://github.com/usuario/repositorio.git
```
7. Enviar a branch para o remoto e definir upstream:
```
git push -u origin aluno-joao
```
8. Para manter o branch atualizado com o principal antes de abrir PR, trazer alterações do remoto:
```
git pull origin main
# ou obter e rebase: git fetch origin && git rebase origin/main
```

Função de cada comando resumida no fluxo:
- `git init`: cria o repositório local.
- `git status`: mostra o estado atual dos arquivos.
- `git add`: prepara (stage) os arquivos para commit.
- `git commit`: registra as alterações localmente com uma mensagem.
- `git branch` / `git switch`: cria/entra em uma branch para trabalhar isoladamente.
- `git remote add`: configura o repositório remoto (GitHub).
- `git push`: envia commits para o remoto.
- `git pull` / `git fetch` + `git merge`/`rebase`: integra alterações do remoto.

---

## Boas práticas (dicas rápidas)
- Escreva mensagens de commit claras e descritivas.
- Trabalhe em branches por funcionalidade e abra Pull Requests para revisão.
- Atualize sua branch frequentemente a partir do branch principal para reduzir conflitos.
- Use `.gitignore` para evitar versionar arquivos temporários, binários ou credenciais.

---

## Próximos passos (opções)
- Posso adicionar um arquivo `.gitignore` sugerido (por exemplo para projetos web).
- Posso criar um exemplo de fluxo com comandos para Windows/macOS/Linux.
- Posso abrir um Pull Request com estas mudanças nesta mesma branch ou em outra branch, se preferir.
