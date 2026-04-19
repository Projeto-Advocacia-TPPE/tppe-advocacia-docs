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

## Validacao Rapida

Para validar os tres repositorios em uma maquina limpa:

- `tppe-advocacia-backend`: copie `.env.example` para `.env`, ajuste `API_HOST_PORT` e `POSTGRES_PORT` se necessario e execute `docker compose up --build`
- `tppe-advocacia-frontend`: copie `.env.example` para `.env`, execute `npm install` e depois `npm run dev`
- `tppe-advocacia-docs`: crie `.venv`, instale `requirements.txt` e execute `mkdocs serve`
