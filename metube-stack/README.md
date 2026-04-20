# metube-stack

Docker stack managed by Portainer

## Services

```
  • metube
```

## Volumes

- `/mnt/storagepool/master/Media/youtube`
- `/mnt/storagepool/apps_config/metube/state`
- `/mnt/storagepool/master/Media/youtube/metube-config/cookies.txt`

## Ports

- `8086`

## Deployment

```bash
cd metube-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration