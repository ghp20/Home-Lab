# tandoor-recipes-stack

Docker Compose stack for **tandoor-recipes-stack**.

## Services

| Service | Image |
|---------|-------|
| postgres | `postgres:18` |
| tandoor | `vabene1111/recipes:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `AI_ENABLE` — see compose for default
- `AI_PROVIDER` — see compose for default
- `ALLOWED_HOSTS` — see compose for default
- `COMMENT_PREF_DEFAULT` — see compose for default
- `DB_ENGINE` — see compose for default
- `DEBUG` — see compose for default
- `FRACTION_PREF_DEFAULT` — see compose for default
- `GUNICORN_MEDIA` — see compose for default
- `OPENAI_API_KEY` — replace with actual value
- `OPENAI_MODEL` — see compose for default
- `PGDATA` — see compose for default
- `POSTGRES_DB` — see compose for default
- `POSTGRES_HOST` — see compose for default
- `POSTGRES_PASSWORD` — replace with actual value
- `POSTGRES_PORT` — see compose for default
- `POSTGRES_USER` — see compose for default
- `SECRET_KEY` — replace with actual value
- `SHOPPING_AUTO_SYNC` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
