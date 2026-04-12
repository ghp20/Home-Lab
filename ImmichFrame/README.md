# ImmichFrame

Digital photo frame frontend for Immich.

**Ports:** 30042

## What this stack is for

ImmichFrame is a read-only digital photo frame web UI that connects to an existing Immich server and displays your photos as a slideshow — great for wall-mounted displays or a dedicated tablet.

## Included services

- `immichframe` — the ImmichFrame web application

## Deploy with Portainer

1. In Portainer, open **Stacks** and choose **Add stack**.
2. Use `ImmichFrame` as the stack name, then paste/upload the `docker-compose.yaml` from this directory.
3. Replace placeholders such as `changeme`, `/path/to/your/data`, and `your-server-ip`.
4. Create the required bind-mount paths before deployment.
5. Deploy the stack, then check **Container logs**, **Health**, and published ports in Portainer.

## Warnings & gotchas

- Replace all placeholders (`changeme`, `/path/to/your/data`, `your-*`) before deploying.
- `ImmichServerUrl` must point to your actual Immich server address and port.
- `ApiKey` must match an API key configured in your Immich server settings.
- Persistent storage for `/cache` is recommended to avoid re-downloading images on restart.

## Exposed ports

30042 (immichframe web UI)

## Files in this folder

- `docker-compose.yaml` — stack definition used by Portainer / Docker Compose.
- `README.md` — high-level notes for what the stack does and how to deploy it.
