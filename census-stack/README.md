# census-stack

Docker stack managed by Portainer

## Services

```
  • options
  • census-server
```

## Key Env Vars

- `AUTH_ENABLED`
- `AUTH_PASSWORD`
- `AUTH_USERNAME`
- `TZ`

## Volumes

- `/var/run/docker.sock`
- `/mnt/storagepool/apps_config/census/server`
- `/mnt/storagepool/apps_config/census/config`

## Ports

- `8087`

## Deployment

```bash
cd census-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration