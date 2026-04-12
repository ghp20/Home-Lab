# Home Assistant

## What this stack is for

Home automation platform for devices, integrations, dashboards, and automations.

## Included services

- `postgres` — `postgres`
- `homeassistant` — `home-assistant`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`, `${...}`) before deploying.
- This stack requests elevated privileges or Linux capabilities; review them before deploying.
- This stack uses host networking, so port handling differs from normal Portainer publishing.
- Persistent database/cache volumes matter here; make sure datasets/volumes exist and are backed up.
- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

No explicit host port mappings in this compose file.

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
