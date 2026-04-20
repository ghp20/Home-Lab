# portracker-stack

Port tracking dashboard

## Services

```
  • portracker
```

## Volumes

- `/mnt/storagepool/apps_config/portracker/data`
- `/var/run/docker.sock`

## Deployment

```bash
cd portracker-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration