# AdGuard Home

## What this stack is for

Network-wide DNS ad blocking and DNS filtering for the homelab.

## Included services

- `adguardhome` — `adguardhome`

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use the folder name from this repo as the stack name, then paste or upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, `your-*`, and any `${ENV_VAR}` values.
4. Create any required bind-mount paths, datasets, secrets, and external Docker networks before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Review ports, storage paths, and environment variables before first deploy.

## Exposed ports

3080:80/tcp, 3443:443/tcp, 53:53/tcp, 53:53/udp, 784:784/udp, 8053:8053/tcp, 853:853/tcp

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
