# AdventureLog

## What this stack is for

Travel and adventure logging app for tracking trips, places, and related media.

## Included services

- `db` — `postgis`
- `backend` — `adventurelog-backend`
- `frontend` — `adventurelog-frontend`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`, `${...}`) before deploying.
- Persistent database/cache volumes matter here; make sure datasets/volumes exist and are backed up.
- Public URLs and callback domains must match how you actually access the app.
- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

8015:3000, 8016:8000

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
