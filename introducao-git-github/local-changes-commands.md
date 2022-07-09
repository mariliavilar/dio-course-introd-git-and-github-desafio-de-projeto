# 🔄 📍 ALTERAÇÕES LOCAIS



- `untracked`  →  `Untracked`

- `tracked`  →  `Unmodified`, `Modified`, `Staged`

  

### 🌀 Estados/ File lifecycle

- 🙈 **UNTRACKED** → arq acabou de ser adicionado, mas ainda não foi visto pelo GIT (n há nenhuma versão desse arq no git)

- ❌ 🔄 **UNMODIFIED** → adicionei o arquivo, mas ele nao sofreu modificações

- ☑️ 🔄 **MODIFIED** → o arq ja está adicionado, o git está visualizando ele, mas qd modificado é necessário novamente dar o git add

- ✅ **STAGED** → arq está “pronto” para ser commitado

  

  ![lifecycle local](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b78445bf-cd92-47be-b032-b32de10aa1d1/Untitled.png)

  

### 🎮  Comandos Gerais

- `git status` aparece oq tem ainda p comitar, etc (LOCAL)
- `git add <nome-do-arquivo>` → adiciona apenas este arquivo específico, deixando pronto para commit
  - `git add -p` →  "prepara" para adicionar, porém mostrando uma revisão das alterações para confirmação do que será adicionado de fato
  - `git add *` ou `git add .`  →  adicionar todos
- `git commit -m "<minha-mensagem-do-commit>"` -> comitta localmente (git “tira uma foto” do estado)
  - `git commit -am "<minha-mensagem-do-commit>"` git add + git commit → commita, dando add no que ainda não estava no staging area



### 🔄 📝 Alterar commit feito

- ✨ alterar último commit, atualizando a mensagem do commit
  -  `git commit --amend -m "<minha-mensagem-do-commit>"` → vai dar overwriting no commit mais recente com um novo commit
- ♻️ alterar último commit, reutilizando a mensagem dele já escrita
  -  `git commit --amend --reuse-message HEAD**`



### 🗑️ 🔄 Excluir Alterações

#### Antes do commit

- `git commit .`

#### Após o commit

- [fonte](https://stackoverflow.com/questions/4630312/reset-all-changes-after-last-commit-in-git)

1. Resetar quaisquer alterações

   `git reset HEAD --hard` -> 

2. Remover novos arquivos

   `git clean -fd`