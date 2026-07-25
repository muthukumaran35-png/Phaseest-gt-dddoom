# URKAE Phase 1A

A small, validated foundation for the URKAE research and knowledge platform.

## Phase 1A scope

- FastAPI application
- PostgreSQL database configuration
- SQLAlchemy 2.x models
- Alembic migration
- Projects
- Research objectives
- Basic format registry
- Health endpoint
- API tests
- Docker Compose

## Not included yet

Phase 1A intentionally excludes advanced governance, provenance graphs,
audit hash chains, recursive source discovery, extraction pipelines,
contradiction detection, retrieval projections, and the complete 120-format
registry. Those belong to the next expansion phase.

## Local setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
cp .env.example .env
alembic upgrade head
uvicorn urkae.main:app --reload
```

OpenAPI documentation is available at `/docs`.

## Tests

```bash
pytest
```

## Docker

```bash
docker compose up --build
```
