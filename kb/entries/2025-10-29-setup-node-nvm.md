
```yaml
session:
  date: "2025-10-29"
  phase: "Fase 1 – Fundamentos"
  goal: "Preparar ambiente: terminal, nvm e Node LTS (macOS)"
  outcomes:
    - "nvm instalado e carregando no zsh"
    - "Node LTS v24.11.0 e npm 11.6.1 funcionando"
  commands:
    - cmd: "nvm install --lts && nvm alias default lts/*"
      output: "node v24.11.0; default -> lts/*"
  next_actions:
    - "Instalar @sap/cds-dk e rodar Hello CAP (ping)"
  risk:
    description: "Quebra ao abrir novo terminal"
    mitigation: "Verificar ~/.zshrc e rodar source ~/.zshrc"
  tags: [fase-1, setup, nvm, node, cap, btp]

```EOF
```
