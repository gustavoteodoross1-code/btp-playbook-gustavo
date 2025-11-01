# BTP Playbook – Gustavo

Repositório de estudos e portfólio focado em **SAP BTP** (Application Dev & Integration, Data & Analytics, AI & Automation, Security & Ops).

## Estrutura
- `kb/entries/` — Diário de sessões (YAML + resumo)
- `projects/` — POCs/labs (CAP, Integration Suite, Kyma, etc.)
- `artifacts/` — Diagramas, templates, checklists

## Convenção de arquivos (KB)
`kb/entries/YYYY-MM-DD-titulo.md`  
Bloco inicial em YAML + resumo. Exemplo:
```yaml
session:
  date: "YYYY-MM-DD"
  phase: "Fase X – Nome"
  goal: "Objetivo da sessão"
  outcomes: ["resultado 1", "resultado 2"]
  commands:
    - cmd: "comando principal"
  next_actions: ["próximo passo 1"]
  risk:
    description: "risco"
    mitigation: "mitigação"
  tags: [fase-x, tag1, tag2]

eof
