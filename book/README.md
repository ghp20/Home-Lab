# Bookshelf Stack

## What this stack is for

Book and audiobook stack combining Bookshelf, Calibre, Calibre-Web, and Audiobookshelf.

## Included services

- `bookshelf` — `bookshelf`
- `calibre` — `calibre`
- `calibre-web` — `calibre-web`
- `audiobookshelf` — `audiobookshelf`
- `calibre-importer` — `calibre`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`, `${...}`) before deploying.
- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

13378:80, 8099:8080, 8101:8083, 8787:8787

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
