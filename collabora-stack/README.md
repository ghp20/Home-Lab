# collabora-stack

Online docs — Collabora Online

## Services

```
  • options
  • collabora
```

## Volumes

- `/mnt/storagepool/apps_config/collabora/config`

## Ports

- `9980`

## Deployment

```bash
cd collabora-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration