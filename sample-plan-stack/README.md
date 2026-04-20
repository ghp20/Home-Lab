# sample-plan-stack

Docker stack managed by Portainer

## Services

```
  • backend
  • frontend
  • sample-plan-net
```

## Volumes

- `/mnt/storagepool/apps_config/sample-plan`

## Ports

- `8094`

## Deployment

```bash
cd sample-plan-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration