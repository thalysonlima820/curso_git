# git status

Mostra quaisquer mudanças no repositório, incluindo arquivos modificados, adicionados ou removidos, e alterações em pastas.

---

# git log

Exibe o histórico de commits do repositório, com detalhes como autor, data e mensagem de cada commit.

---

# git reset

Usado para voltar o repositório a um commit anterior. Pode ser usado de diferentes formas, dependendo do que você deseja preservar:

- `git reset --hard <código-do-commit>`  
  Volta para o commit especificado e apaga todas as mudanças feitas depois dele (inclusive arquivos locais).  
  __Exemplo:__  
  `git reset --hard 1da8be72dfdf05aa4e56222088f7518c785a3434`

- `git reset --soft <código-do-commit>`  
  Volta para o commit especificado, mas mantém todas as mudanças locais (nada é perdido, apenas o ponteiro da branch é movido).  
  __Exemplo:__  
  `git reset --soft 1da8be72dfdf05aa4e56222088f7518c785a3434`

---

## Se for baseado no repositório remoto (GitHub)

- `git fetch origin`  
  Atualiza as informações do repositório remoto.

- `git reset --hard origin/main`  
  Força o código local a ser igual ao do repositório remoto (descarta tudo localmente).

- `git reset --soft origin/main`  
  Atualiza o ponteiro da branch para o remoto, mas mantém todas as mudanças locais.

---

# git mv

---

# git branch

Lista e cria branches, que são ramificações do código para desenvolvimento paralelo.

- `git branch`  
  Lista todas as branches locais existentes.

- `git branch <nome-da-branch>`  
  Cria uma nova branch com o nome especificado.

- `git branch -d <nome-da-branch>`  
  Deleta branch com o nome especificado.

---

# git checkout

Serve para mudar entre branches ou criar e mudar para uma branch nova.

- `git checkout <nome-da-branch>`  
  Muda para a branch especificada.

- `git checkout -b <nome-da-branch>`  
  Cria uma nova branch e já muda para ela.
