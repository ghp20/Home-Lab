# plex-stack

Media server — Plex

## Services

```
  • plex
```

## Volumes

- `/mnt/storagepool/apps_config/plex/config`
- `/mnt/storagepool/apps_config/plex/transcode`
- `/mnt/storagepool/master/Media`
- `/dev/dri`

## Ports

- `32400`

## Deployment

```bash
cd plex-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration