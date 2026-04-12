# claude-code-stack

Docker Compose stack for **claude-code-stack**.

## Services

| Service | Image |
|---------|-------|
| claude-code | `node:20-slim` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `CLAUDE_DISABLE_OAUTH` — see compose for default
- `PATH` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
