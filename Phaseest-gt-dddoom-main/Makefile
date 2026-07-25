install:
	pip install -e ".[dev]"

run:
	uvicorn urkae.main:app --reload

test:
	pytest

lint:
	ruff check .

format:
	ruff format .

migrate:
	alembic upgrade head

up:
	docker compose up --build
