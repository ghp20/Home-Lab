# bichon-ai-digest-stack

Docker Compose stack for **bichon-ai-digest-stack**.

## Services

| Service | Image |
|---------|-------|
| bichon-ai-digest | `python:3.12-slim` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `BICHON_ACCOUNT_IDS` — replace with actual value
- `BICHON_TOKEN` — replace with actual value
- `BICHON_URL` — replace with actual value
- `MAX_EMAILS_PER_ACCOUNT` — see compose for default
- `MAX_ITEMS_PER_CATEGORY` — see compose for default
- `MAX_PAGES_PER_ACCOUNT` — see compose for default
- `MAX_SNIPPET_CHARS` — see compose for default
- `OPENAI_API_KEY` — replace with actual value
- `OPENAI_MODEL` — replace with actual value
- `TELEGRAM_BOT_TOKEN` — replace with actual value
- `TELEGRAM_CHAT_ID` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
