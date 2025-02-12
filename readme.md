# Shell Aliases for Laravel, Docker, and Sudo Commands

## Laravel Aliases
```bash
alias sail='sh $( [ -f sail ] && echo sail || echo vendor/bin/sail)'  # Atalho para o comando Sail do Laravel
alias pa='php artisan'  # Atalho para o comando php artisan
alias pam='php artisan migrate'  # Executa a migração do banco de dados
alias fresh='php artisan migrate:fresh --seed'  # Restaura e semeia o banco de dados
alias test='php artisan test'  # Executa os testes no Laravel
alias cacheclear='php artisan cache:clear'  # Limpa o cache do Laravel
alias routecache='php artisan route:cache'  # Cria o cache de rotas no Laravel
```

## Docker Aliases
```bash
alias dk='docker'  # Atalho para o comando docker
alias dkps='docker ps'  # Lista os containers em execução
alias dkc='docker-compose'  # Atalho para docker-compose
alias dkimg='docker images'  # Lista as imagens disponíveis no Docker
alias dkcon='docker container ls'  # Lista todos os containers em execução
alias dkvol='docker volume ls'  # Lista todos os volumes do Docker
alias dkexti='docker exec -ti'  # Executa um comando interativo dentro de um container
alias dkrmcon='docker rm'  # Remove um container específico (exemplo de uso: dkrmcon <CONTAINER_ID>)
alias dkrmcona='docker rm $(docker ps -a -q)'  # Remove todos os containers parados
alias dkrmimg='docker rmi'  # Remove uma única imagem (exemplo de uso: dkrmimg <IMAGE_ID>)
alias dkrmimga='docker rmi $(docker images -q)'  # Remove todas as imagens do Docker
alias dkrmvol='docker volume rm'  # Remove um único volume (exemplo de uso: dkrmvol <VOLUME_NAME>)
alias dkrmvola='docker volume rm $(docker volume ls -q)'  # Remove todos os volumes do Docker
alias dkstop='docker stop'  # Para um container específico (exemplo de uso: dkstop <CONTAINER_ID>)
alias dkstopall='docker stop $(docker ps -q)'  # Para todos os containers em execução
alias dkprune='docker system prune -af'  # Remove containers, imagens e volumes não utilizados
alias dknetls='docker network ls'  # Lista todas as redes do Docker
alias dknetrm='docker network rm'  # Remove uma rede específica do Docker (exemplo de uso: dknetrm <NETWORK_ID>)
alias dklg='docker logs' # Exibe relatório de logs do container
```

## Sudo Aliases
```bash
alias sd='sudo'  # Atalho para executar comandos como superusuário
alias sai='sudo apt install'  # Instala um pacote (exemplo: sai nome-do-pacote)
alias sau='sudo apt update'  # Atualiza a lista de pacotes disponíveis
alias sar='sudo apt autoremove'  # Remove pacotes desnecessários
alias saug='sudo apt upgrade'  # Atualiza todos os pacotes instalados para as versões mais recentes
```

## Git Aliases
```bash
alias gs='git status'  # Exibe o status do repositório Git
alias ga='git add .'  # Adiciona todos os arquivos modificados ao stage
alias gc='git commit -m'  # Realiza um commit com uma mensagem (exemplo de uso: gc "Mensagem do commit")
alias gp='git push'  # Envia as alterações para o repositório remoto
alias gpl='git pull'  # Puxa as alterações do repositório remoto
alias gco='git checkout'  # Troca de branch no Git (exemplo de uso: gco <branch_name>)
alias gb='git branch'  # Lista as branches locais do Git
alias gcm='git checkout main'  # Troca para a branch principal (main)
alias gch='git checkout -'  # Troca para a última branch visitada no Git
alias glog='git log --oneline --graph --decorate --all'  # Exibe o histórico de commits de forma visual
```

## General Aliases
```bash
alias cls='clear'  # Limpa o terminal
alias ll='ls -lah'  # Lista arquivos detalhadamente, incluindo arquivos ocultos
alias ..='cd ..'  # Sobe um diretório
alias ...='cd ../..'  # Sobe dois diretórios
alias h='history'  # Exibe o histórico de comandos
alias e='exit'  # Sai do terminal
```

