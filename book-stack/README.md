# book-stack

Docker Compose stack for **book-stack**.

## Services

| Service | Image |
|---------|-------|
| bookshelf | `ghcr.io/pennydreadful/bookshelf:hardcover` |
| calibre | `lscr.io/linuxserver/calibre:latest` |
| calibre-web | `lscr.io/linuxserver/calibre-web:latest` |
| audiobookshelf | `ghcr.io/advplyr/audiobookshelf:latest` |
| calibre-importer | `lscr.io/linuxserver/calibre:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `PGID` — see compose for default
- `PUID` — see compose for default
- `TZ` — see compose for default

## Volumes

- /path/to/your/data

## Networks

books_net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
