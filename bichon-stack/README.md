# bichon-stack

AI digest bot — Bichon

## Services

```
  • bichon
```

## Volumes

- `/mnt/storagepool/apps_config/bichon/data`

## Ports

- `15630`

## Deployment

```bash
cd bichon-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration