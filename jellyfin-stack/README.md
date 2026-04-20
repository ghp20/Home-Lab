# jellyfin-stack

Media server — Jellyfin

## Services

```
  • jellyfin
```

## Volumes

- `/mnt/storagepool/apps_config/jellyfin/config`
- `/mnt/storagepool/apps_config/jellyfin/cache`
- `/mnt/storagepool/apps_config/jellyfin/transcode`
- `/mnt/storagepool/master/Media`

## Ports

- `8096`
- `8920`

## Deployment

```bash
cd jellyfin-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration