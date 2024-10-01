# alias

```bash
vi ~/.zshrc
###

all_git_pull() {
  for dir in *; do
    if [[ -d "$dir/.git" ]]; then
      echo "⚡️ [ $dir ] 'git pull'을 수행합니다..."
      cd "$dir"
      git pull
      cd ..
    fi
  done
}

alias python="python3"
alias pip="pip3"
alias zvi="vi ~/.zshrc"
alias zsource="source ~/.zshrc"
alias tfmt="terraform fmt --recursive"
alias lsal="lsd -al"
alias allpull=all_git_pull
alias k=kubectl
export do="--dry-run=client -o yaml"

###
source ~/.zshrc
```
