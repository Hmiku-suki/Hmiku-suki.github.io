---
title: wsl_ubuntu的某些操作
date: 2021-01-20 13:39:39
tags: linux
category: System
---
此篇记录了wsl_ubuntu的某些操作
<!-- more -->

#### 设定bash
```
$ cat <<'END' >> ~/.bashrc
PROMPT_COMMAND=__prompt_command
__prompt_command() {
    local EXIT="$?"
    PS1=""
    local RCol='\[\e[0m\]'
    local Red='\[\e[0;31m\]'
    local Gre='\[\e[0;32m\]'
    local Yel='\[\e[1;33m\]'
    local Blu='\[\e[1;34m\]'
    local Pur='\[\e[0;35m\]'
    if [ $EXIT != 0 ]; then
        PS1+="${Red}$EXIT${RCol}"
    else
        PS1+="${Gre}0${RCol}"
    fi
    PS1+="${Pur}|${RCol}${Blu}\W${RCol}${Pur}>${RCol} "
}
export EDITOR=vim
export CLICOLOR=1
export LSCOLORS=gxBxhxDxfxhxhxhxhxcxcx
END
```
#### 初始化
`sudo apt-get install build-essential curl file git`

#### anaconda3环境变量
```
# add anaconda3
export PATH=/home/miku/anaconda3/bin:$PATH
export LD_LIBRARY_PATH=/home/miku/anaconda3/lib:$LD_LIBRARY_PATH
```