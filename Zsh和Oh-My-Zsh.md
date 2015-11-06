# ZSH 和 Oh-My-Zsh

![zsh shell](https://pic4.zhimg.com/b691b3fa0ffb6d6c90761a98d3afab1b_b.jpg)

> 使用zsh
> 
> **`chsh -s /bin/zsh`**

*使用bash chsh -s /bin/bash*

## oh-my-zsh

自动安装：

``` shell
wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh
```

手动安装：

``` shell
git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
```

安装完成后，重新打开终端就可以了



我的.zshrc文件

``` shell
export ZSH=$HOME/.oh-my-zsh
export PATH="$(brew --prefix homebrew/php/php56)/bin:$PATH"
export PATH="$(brew --prefix homebrew/php/php56)/sbin:$PATH"
ZSH_THEME="robbyrussell"

plugins=(git autojump history)

export PATH=$HOME/bin:/usr/local/bin:$PATH

source $ZSH/oh-my-zsh.sh

$(boot2docker shellinit)
alias rc="subl ~/.zshrc"
alias orc="subl ~/.oh-my-zsh"
alias c=clear
alias rr="rm -rf"
export PATH="/usr/local/sbin:$PATH"
```

