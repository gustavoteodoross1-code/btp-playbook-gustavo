# 2025-10-29 – Setup Node/nvm e GitHub SSH (Fase 1)

```yaml
session:
  date: "2025-10-29"
  phase: "Fase 1 – Fundamentos"
  goal: "Instalar nvm/Node LTS no macOS e publicar repo no GitHub via SSH"
  outcomes:
    - "nvm instalado e carregado no zsh (~/.zshrc)"
    - "Node LTS v24.11.0 e npm 11.6.1 funcionando"
    - "Repo 'btp-playbook-gustavo' publicado na branch main"
    - "README com convenções e estrutura criado"
  commands:
    - cmd: "curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.2/install.sh | bash"
    - cmd: "export NVM_DIR=\"$HOME/.nvm\" && [ -s \"$NVM_DIR/nvm.sh\" ] && . \"$NVM_DIR/nvm.sh\""
    - cmd: "nvm install --lts && nvm alias default lts/* && nvm use --lts"
    - cmd: "ssh-keygen -t ed25519 -C \"gustavo.teodoross1@gmail.com\" && ssh-add --apple-use-keychain ~/.ssh/id_ed25519"
    - cmd: "git remote set-url origin git@github.com:gustavoteodoross1-code/btp-playbook-gustavo.git && git push -u origin main"
  next_actions:
    - "Instalar @sap/cds-dk e validar cds -v"
    - "Criar projeto Hello CAP e rodar cds watch"
  risk:
    description: "nvm não carregando em novas sessões"
    mitigation: "confirmar linhas do nvm no ~/.zshrc e rodar 'source ~/.zshrc'"
  tags: [fase-1, setup, nvm, node, github-ssh, repo]
``````
