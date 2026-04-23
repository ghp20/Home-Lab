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

- `/mnt/storagepool/apps_config/Immich/data`
- `/mnt/storagepool/master/immich_external`
- `/etc/localtime`
- `/mnt/storagepool/apps_config/Immich/postgres`

## Deployment

```bash
cd immich-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration