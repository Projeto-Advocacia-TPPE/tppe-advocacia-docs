# Documentação

Repositório da documentação do projeto de advocacia da disciplina TPPE.

## Estrutura

```text
.
├── docs/
├── .github/workflows/deploy.yml
├── mkdocs.yml
└── requirements.txt
```

## Rodando localmente

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

## Build

```bash
mkdocs build
```
