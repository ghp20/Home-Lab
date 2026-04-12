# karakeep-stack

Docker Compose stack for **karakeep-stack**.

## Services

| Service | Image |
|---------|-------|
| web | `ghcr.io/karakeep-app/karakeep:release` |
| chrome | `gcr.io/zenika-hub/alpine-chrome:124` |
| meilisearch | `getmeili/meilisearch:v1.13.3` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `BROWSER_WEB_URL` — see compose for default
- `DATA_DIR` — see compose for default
- `MEILI_ADDR` — see compose for default
- `MEILI_NO_ANALYTICS` — see compose for default
- `NEXTAUTH_SECRET` — replace with actual value
- `NEXTAUTH_URL` — see compose for default
- `OPENAI_API_KEY` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
