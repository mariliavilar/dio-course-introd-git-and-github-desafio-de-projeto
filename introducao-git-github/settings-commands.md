# ⚙️ COMANDOS DE CONFIGURAÇÕES 

## 👤 config usuario

- ➕ 🎲  **Incluir dados**:

  🚨 Podemos setar as configurações de **maneira global** (add 🚩 `--global` ),
  ou **apenas para o repositório onde estamos** (sem add 🚩 `--global` abaixo)

  - nome do usuario → `git config --global user.name "My Name"`

  - email do usuário → `git config --global user.email "myemail@email.com"`

  - ⚠️ É importante/interessante que seu *user.name* e seu *user.email* sejam os mesmos da sua conta do github ou plataforma similar, para poder preservar corretamente o histórico e versionamento.

  - add editor de sua preferencia: `git config --global <comando-do-editor>`

    

- 👁️ 🎲 **Conferir dados**:

  `git config --list`→ lista todos dados

  `git config <nome-da-chave-que-quero-saber>` → resp. dado solicitado

  

- 🗑️ 🎲 Remover dado   → add 🚩 `--unset`

  - nome do usuario → `git config --global --unset user.name`
  - email do usuário → `git config --global --unset user.email`