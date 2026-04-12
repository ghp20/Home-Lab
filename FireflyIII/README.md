# Firefly III

## What this stack is for

Personal finance manager for accounts, budgets, transactions, and imports.

## Included services

- `firefly-db` — `mariadb`
- `firefly-iii` — `core`
- `firefly-importer` — `data-importer`

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

8081:8080, 8083:8080

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
