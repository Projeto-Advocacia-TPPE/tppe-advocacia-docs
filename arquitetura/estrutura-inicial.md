# Estrutura Inicial dos Repositórios

Esta entrega organiza o projeto em duas frentes principais:

- `backend/`: API em FastAPI com estrutura MVC e Postgres no mesmo repositório
- `frontend/`: aplicação React com Vite para consumir a API

## Visão Geral

```text
.
├── backend/
│   ├── app/
│   │   ├── controllers/
│   │   ├── core/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── schemas/
│   │   └── views/
│   ├── docker-compose.yml
│   ├── Dockerfile
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   └── services/
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── docs/
└── mkdocs.yml
```

## Backend

### Stack

- Python + FastAPI
- SQLAlchemy
- Postgres
- Docker Compose

### Organização MVC

- `models/`: entidades e mapeamento ORM
- `controllers/`: regras de negócio
- `views/`: camada HTTP com endpoints
- `routes/`: agregação de rotas
- `schemas/`: contratos de entrada e saída
- `core/`: configuração e acesso ao banco

### Endpoints iniciais

- `GET /api/v1/health`
- `GET /api/v1/leads`
- `POST /api/v1/leads`

## Frontend

### Stack

- React
- Vite

### Organização inicial

- `components/`: componentes reutilizáveis da interface
- `services/`: integração com a API
- `App.jsx`: composição da página inicial

### Integração

O frontend usa a variável `VITE_API_URL` para apontar para a API. Por padrão, ela está configurada para:

```env
VITE_API_URL=http://localhost:8000/api/v1
```

## Como Executar

### Backend

```bash
cd backend
cp .env.example .env
docker compose up --build
```

### Frontend

```bash
cd frontend
cp .env.example .env
npm install
npm run dev
```
