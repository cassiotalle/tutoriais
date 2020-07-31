# Configurar Ambiente de Dev Linux/Wsl

## 

## Configurações Gerais

### Instalar configurar GIT

```bash
git config --global user.name "Cássio Talle e Silva"`
```

```bash
git config --global user.name "Cássio Talle e Silva"
```

### Criar chaves ssh

```bash
ssh-keygen -t rsa -b 4096 -C "cassiotalle@gmail.com"
```

## Zsh Terminal

### Istalar Zsh Terminal

```bash
sudo apt install zsh
```

### Instalar [Oh My Zsh](https://ohmyz.sh/)

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Instalar [Plugin Zsh Auto Suggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### Configurar arquivo .zshrc

```bash
nano ~.zshrc
```

No arquivo alterar os parâmetros **ZHS_THEME** e **plugins**

```bash
ZSH_THEME="af-magic"


plugins=(git ssh-agent zsh-autosuggestions zsh-nvm)
```
