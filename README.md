# My MacOS .bash_profile

Dependecies:

https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion

```

#Terminal color patterns
export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]\$ "
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad

#Git shortcuts
alias gmas='git checkout master'
alias greb='git pull --rebase'
alias gres='git reset --hard head'
alias gmer='git merge master'
alias gc='git clean -d -f'
alias gp='git push'
alias gs='git status'
alias gd='git diff'
alias gb='git branch'

#Terminal Shortcuts
alias ls='ls -GFhla'
alias cpwd='pwd | pbcopy'
alias bp='cat ~/.bash_profile'
alias ebp='vi ~/.bash_profile'
alias hosts='cat /etc/hosts'
alias ehosts='sudo vi /etc/hosts'

#Maven Shortcuts
alias mci='mvn clean install'

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion  #This loads git bash-completion

#THIS MUST BE AT THE END OF THE FILE FOR SDKMAN TO WORK!!!
export SDKMAN_DIR="/Users/calvinchan/.sdkman"
[[ -s "/Users/calvinchan/.sdkman/bin/sdkman-init.sh" ]] && source "/Users/calvinchan/.sdkman/bin/sdkman-init.sh"

```
