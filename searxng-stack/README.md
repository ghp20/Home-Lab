# searxng-stack

Privacy-respecting metasearch — SearXNG

## Services

```
  • redis
  • searxng
  • searxng-network
```

## Volumes

- `/mnt/storagepool/apps_config/searxng/redis`
- `/mnt/storagepool/apps_config/searxng/config`

## Ports

- `8091`

## Deployment

```bash
cd searxng-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration