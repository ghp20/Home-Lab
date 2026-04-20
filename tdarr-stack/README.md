# tdarr-stack

Media transcoding — Tdarr

## Services

```
  • tdarr
  • tdarr-node
```

## Volumes

- `/mnt/storagepool/apps_config/tdarr/server`
- `/mnt/storagepool/apps_config/tdarr/config`
- `/mnt/storagepool/apps_config/tdarr/log`
- `/mnt/nvmepool/appsconfig/tdarr/temp`
- `/mnt/storagepool/master/Media/`
- `/mnt/storagepool/master/Media/Movies`

## Ports

- `8265`
- `8266`

## Deployment

```bash
cd tdarr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration