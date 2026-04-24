# immich-stack

Docker stack managed by Portainer

## Services

```
  • immich-server
  • immich-machine-learning
  • redis
  • database
  • immich-ml-cache
```

## Volumes

- `/etc/localtime`

## Deployment

```bash
cd immich-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration