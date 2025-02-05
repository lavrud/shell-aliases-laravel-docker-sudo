# Shell Aliases for Laravel, Docker, and Sudo Commands

## Laravel Aliases
```bash
alias sail='sh $( [ -f sail ] && echo sail || echo vendor/bin/sail)'
alias pa='php artisan'
alias pam='php artisan migrate'
alias fresh='php artisan migrate:fresh --seed'
alias test='php artisan test'
alias cacheclear='php artisan cache:clear'
alias routecache='php artisan route:cache'
```

## Docker Aliases
```bash
alias dk='docker'
alias dkps='docker ps'
alias dkc='docker-compose'
alias dkimg='docker images'
alias dkcon='docker container ls'
alias dkexti='docker exec -ti'
alias dkrmcona='docker rm $(docker ps -a -q)'
alias dkrmimga='docker rmi $(docker images -q)'
alias dkrmvola='docker volume rm $(docker volume ls -q)'
alias dklgs='docker logs -f'
alias dkstopall='docker stop $(docker ps -q)'
alias dkprune='docker system prune -af'
alias dknetls='docker network ls'
alias dknetrm='docker network rm'
```

## Sudo Aliases
```bash
alias sd='sudo'
alias sai='sudo apt install'
alias sau='sudo apt update'
alias sar='sudo apt autoremove'
alias saug='sudo apt upgrade'
```

## Git Aliases
```bash
alias gs='git status'
alias ga='git add .'
alias gc='git commit -m'
alias gp='git push'
alias gpl='git pull'
alias gco='git checkout'
alias gb='git branch'
alias gcm='git checkout main'
alias gch='git checkout -'
alias glog='git log --oneline --graph --decorate --all'
```

## General Aliases
```bash
alias cls='clear'
alias ll='ls -lah'
alias ..='cd ..'
alias ...='cd ../..'
alias h='history'
alias e='exit'
```

