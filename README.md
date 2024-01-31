# My MacOS .bash_profile

Dependecies:

https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion

```

autoload -Uz vcs_info
precmd() { vcs_info }

zstyle ':vcs_info:git:*' formats '%b '

setopt PROMPT_SUBST
PROMPT='%F{green}%*%f %F{blue}%~%f %F{red}${vcs_info_msg_0_}%f$ '

export PATH=/opt/homebrew/bin:$PATH
export PATH=/opt/homebrew/sbin:$PATH
export PATH=$HOME/.composer/vendor/bin:$PATH
export PATH=\"\${HOME}/.pyenv/shims:\${PATH}\
PATH="/usr/local/bin:$PATH"
export PATH="/usr/local/opt/python/libexec/bin:$PATH"

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion


#Git shortcuts
alias gmas='git checkout master'
alias gmain='git checkout main'
alias gsta='git checkout staging'
alias greb='git pull --rebase'
alias gres='git reset --hard head'
alias gmer='git merge master'
alias gc='git clean -d -f'
alias gp='git push'
alias gpf='git push --force'
alias gs='git status'
alias gd='git diff'
alias gb='git branch'
alias ga='git add .'
alias gl='git log'
alias gu='git reset --soft HEAD~1'
alias gstash='git stash'
alias gpop='git stash pop'
alias gpurgebranches='git branch --delete $(git branch --merged main --no-contains main)'

#Terminal Shortcuts
alias ls='ls -GFhla'
alias cpwd='pwd | pbcopy'
alias bp='cat ~/.zshrc'
alias ebp='vi ~/.zshrc'
alias rbp='source ~/.zshrc'
alias hosts='cat /etc/hosts'
alias ehosts='sudo vi /etc/hosts'
alias path='echo $PATH'
alias b='cd ..'
alias python='python3.8'
alias docs='cd ~/Documents'


#SMF Shortcuts
alias buildall='npm run dev --app=old && npm run dev --app=um && npm run dev --app=cm && npm run dev --app=hr && npm run dev --app=pm'
alias msserve='php artisan serve --host=smf-mothership.test'
alias ms='cd ~/Documents/smf-mothership'
alias up='cd ~/Documents/smf-userportal'
alias tp='cd ~/Documents/smf-ticketpage'
alias sc='cd ~/Documents/smf-scanners'
alias clearnpm='rm -rf node_modules && rm -rf package-lock.json && npm cache clear --force'

#Bash Completion
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion  #This loads git bash-completion




```
