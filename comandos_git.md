# COMANDOS GIT

## git status
- em qual branch você está

- quais arquivos foram modificados

- quais arquivos estão prontos para commit (staged)
- quais arquivos ainda não foram adicionados para commit (unstaged)
- arquivos novos não rastreados (untracked)
- instruções do que fazer (git add, git commit, etc.)
```
git status
```

## git clone [url]
- Cria uma pasta nova com o nome do projeto
- Baixa todos os arquivos do repositório remoto
- Baixa todo o histórico de commits
- Configura o repositório remoto com o nome origin
- Te coloca automaticamente na branch principal (main ou master)

```
git clone https://github.com/usuario/projeto.git
```
```
git clone https://github.com/usuario/projeto.git nova-pasta
```

# git add
- Serve para preparar arquivos para serem incluídos no próximo commit.

Adicionando um arquivo
```
git add index.html
```

Adicionando todos arquivos modificados
```
git add .
```

Adiciona arquivos de uma pasta
```
git add nome-da-pasta/
```

 # git commit
 - salva permanentemente as alterações
- cria um ponto no histórico (um commit)
- gera um ID único (hash)
- guarda quem fez, quando fez e a mensagem do commit

```
git commit -m "mensagem do commit"
```

# git push

É usado para enviar seus commits locais para o repositório remoto.
```
git push
```

Sintaxe mais comum
```
git push origin nome-da-branch
```
ou se você criou uma branch nova
```
git push -u origin minha-feature
```


# git pull
Serve para baixar as alterações do repositório remoto e atualizar sua branch local com tudo que foi modificado lá.

```
git pull
```
git pull explícito com remoto + branch
```
git pull origin main
```

# git fetch
Serve para baixar as atualizações do repositório remoto SEM misturar (merge) com sua branch local.
```
git fetch
```

# git merge
Serve para unir o histórico de uma branch com outra.
```
git checkout main
git merge minha-feature
```
“Pegue tudo da branch minha-feature e traga para dentro da main.”