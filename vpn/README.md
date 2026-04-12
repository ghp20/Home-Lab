# VPN + Download Stack

## What this stack is for

Combined VPN gateway, download clients, and Bitmagnet-related services.

## Included services

- `gluetun` — `gluetun`
- `qbittorrent` — `qbittorrent`
- `sabnzbd` — `sabnzbd`
- `postgres-bitmagnet` — `postgres`
- `bitmagnet-process` — `bitmagnet`
- `bitmagnet-worker` — `bitmagnet`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`, `${...}`) before deploying.
- This stack requests elevated privileges or Linux capabilities; review them before deploying.
- It references the `arrnet` network; create it first if it does not already exist.
- Persistent database/cache volumes matter here; make sure datasets/volumes exist and are backed up.
- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

3333:3333, 6881:6881, 6881:6881/udp, 8085:8085, 8089:8080

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
