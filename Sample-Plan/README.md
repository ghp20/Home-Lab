# Sample Plan

## What this stack is for

Planning or workflow app with separate backend and frontend services.

## Included services

- `backend` — `sample-plan-backend`
- `frontend` — `sample-plan-frontend`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`, `${...}`) before deploying.
- Check container health status after deploy, not just whether the containers started.
- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

8094:80

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
