# n8n-portainer-stack

Workflow automation — n8n

## Services

```
  • n8n
  • n8n-postgres
  • default
  • trading-net-ron
```

## Volumes

- `/mnt/storagepool/apps_config/n8n/portainer-restore-test`
- `/mnt/storagepool/master/n8n/know_base`
- `/mnt/storagepool/apps_config/n8n/postgres-data`

## Deployment

```bash
cd n8n-portainer-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration