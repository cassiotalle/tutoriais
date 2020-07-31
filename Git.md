# Git

## Configuração global

```bash
git config --global user.name "Cássio Talle e Silva"`
```

```bash
git config --global user.name "Cássio Talle e Silva"
```

## Comandos de repositório

Iniciar diretório

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

Exibe todos os comits e suas hashes

```bash
git log
```

Exibe alterações do commit através da hash

```bash
git show 67faf91448db01d4d328b0b17898f15bea1b4707
```

Exibe de forma gráfica as alteraçãoes no repositório de branches e verções

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

Desfaz commit e volta para o status staged, pronto para ser commitado de novo

```bash
git reset --soft
```

Desfaz commit e volta para o status modified pronto para ser adicionado de novo

```bash
git reset --mixed
```

Desfaz commit e apaga todas as alterações

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

## Copiar repositório na nuvem