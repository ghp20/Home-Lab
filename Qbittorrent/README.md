# qBittorrent + SABnzbd

## What this stack is for

Download stack combining BitTorrent and Usenet clients.

## Included services

- `sabnzbd` — `sabnzbd`
- `qbittorrent` — `qbittorrent`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Deploy the whole stack together in Portainer; the services depend on each other.

## Exposed ports

6881:6881, 6881:6881/udp, 8080:8080, 8087:8080, 9090:9090

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
