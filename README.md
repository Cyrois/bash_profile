export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]\$ "
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad
alias ls='ls -GFhla'
alias gmas='git checkout master'
alias greb='git pull --rebase'
alias gres='git reset --hard head'
alias gc='git clean -d -f'
alias gp='git push'
alias gs='git status'
alias gd='git diff'
alias bp='cat ~/.bash_profile'
alias map='cd ~/Documents/moola-admin-portal'

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion  #This loads git bash-completion
