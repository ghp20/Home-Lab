# anything_llm-stack

Docker Compose stack for **anything_llm-stack**.

## Services

| Service | Image |
|---------|-------|
| anything-llm | `mintplexlabs/anythingllm:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `DATABASE_URL` — see compose for default
- `DISABLE_TELEMETRY` — see compose for default
- `ENCRYPTION_KEY` — replace with actual value
- `SERVER_PORT` — see compose for default
- `STORAGE_DIR` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
