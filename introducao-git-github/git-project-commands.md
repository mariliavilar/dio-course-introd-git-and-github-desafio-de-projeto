# 🟠 PROJETO GIT

---



### 🔍 SABER SE PROJ JÁ TEM GIT REMOTO OU NAO

`git **remote** **-v**`

- não tem → fica vazio

- tem → resposta com origem remota do projeto

  

### ▶️ **INICIALIZAR** REPOSITORIO GIT

`git **init**`

- inicializa o repositório, e o git agora está "enxergando" todas as mudanças dele. 
  (apenas local, remotamente nao subimos nada ainda)

- ex:

  ```bash
  git init
  git add .
  git commit -m “first commit”
  git branch -M main ## Alterar nome de master para main
  ## Crio repositorio no gitlab/github e pegar referência/origin (http ou ssh)
  git remote add origin [colar-aqui-origin-do-repositorio-criado]
  git push -u origin main 
  ```



### 🔄 **TROCAR O ORIGIN** DO PROJ DO GIT (qd ja tem git)

`git remote remove origin` 

`git remote add origin <meu-projeto-aqui>`

 `git remote -v`  → para verificar se está certinho!

- ⚠️ É uma convenção utilizar `origin`  mas pode ter outro nome



### 👯‍♀️ **CLONAR** DO SERVIDOR

`git clone <meu-projeto-aqui>`