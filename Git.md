# Git

## Configuração global

```bash
git config --global user.name "Cássio Talle e Silva"`
```

```bash
git config --global user.email "cassio....@gmail.com"
```

## Comandos de repositório

Iniciar repositório

```bash
git init
```

Verificar o status do reposítório

```bash
git status
```

Adicionar arquivos modificados

```
git add .
```

```bash
git add readme.md
```

Comitar

```bash
git commit -m "descrição"
```

## Git Log

Quantidade de commits por usuário

```bash
git shortlog
```

Exibe todos os commits e suas hashes

```bash
git log
```

Exibe alterações do último commit

```bash
git show
```

Exibe alterações do commit específico através da hash

```bash
git show 67faf91448db01d4d328b0b17898f15bea1b4707
```

Exibe de forma gráfica as alteraçãoes no repositório (branches e verções)

```bash
git log graph
```

Exibe alterações de todos os arquicos antes de commitar

```bash
git diff
```

Exibe nome dos arquivos alterados

```bash
git diff --name-only
```

## Desfazer alterações

Destafazer altaração antes de commitar

```bash
git checkout Nome_do_arquivo.algumacoisa
```

Desfazer `git add`

```bash
git reset HEAD Nome_do_arquivo.algumacoisa
```

### Desfazer commits

Desfaz commit e volta para o status **staged**, pronto para ser commitado de novo

```bash
git reset --soft
```

Desfaz commit e volta para o status **modified** pronto para ser adicionado de novo

```bash
git reset --mixed
```

Desfaz commit e **apaga** todas as alterações

```bash
git reset --hard
```

##

## Git Ignore

Arquivo para indicar quais arquivos não farão parte do repositório

## Github

### SSH

Criar chave publica e privada SSH

```bash
ssh-keygen -t rsa -b 4096 -C "cassiotalle@gmail.com"
```

Exibir chave pública SSH

```bash
cat ~/.ssh/id_rsa.pub
```

## Conectar com o repositório do Github

Adicionar repositório externo (origin se refere ao nome do reposiório remoto, fica a critério do usuário)

```bash
git remote add origin git@github.com:cassiotalle/tutoriais.git
```

Exibe o nome dos repositórios remotos conectados ao projeto

```bash
git remote -v
```

Enviar alterações comitadas. A partir da segunda vez só `git push`

```bash
git push -u origin master
```

### Clonar repositório

```bash
git clone git@github.com:cassiotalle/tutoriais.git nome_do_repositorio_na maquina
```

Fork serve para compiar um projeto e submeter essa alteração para o projeto original a alteração entra como um pull request no projeto original

## Branches

Listar branch

```bash
git branch
```

Criar branch

```bash
git checkout -b nome_do_branch
```

Entrar em um branch

```bash
git checkout nome_do_branch
```

Deletar branch (todos os arquivos do branch são deletados)

```bash
git checkout -D nome_branch
```

## Merge e Rebase

Merge junta dois branches com um commit

```bash
git merge nome_do_branch
```

Rebase realinha todas as alterações de dois branches em um única linha sequnecial

```bash
git rebase nome_do_branch
```

## Gitignore

[GitHub - github/gitignore: A collection of useful .gitignore templates](https://github.com/github/gitignore)

Arquivo `.gitignore`para listar arquivos e extenções que devem ser agnorados pelo git

## Git Stash

Serve para guardar mudanças antes de commitar sem deixa-las com o status **modfied**

Para guardar alterações no stash

```bash
git stash
```

Para utilizar as mudanças que estavam guardadas 

```bash
git stash apply
```

Visualizar o stash

```bash
git stash list
```

Limpar stash

```bash
git stash clear
```

## Git Tag

Serve para indicar verções ou dar nome para grupos de commits 

```bash

```