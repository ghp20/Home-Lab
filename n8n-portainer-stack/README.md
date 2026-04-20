# n8n-portainer-stack

Workflow automation — n8n

## Stack: n8n-portainer-stack

### Services

```
  • n8n
  • n8n-postgres
  • default
  • trading-net-ron
```

### Key Environment Variables

- `DB_POSTGRESDB_DATABASE`
- `DB_POSTGRESDB_HOST`
- `DB_POSTGRESDB_PASSWORD`
- `DB_POSTGRESDB_PORT`
- `DB_POSTGRESDB_USER`
- `DB_TYPE`
- `GENERIC_TIMEZONE`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `TZ`
- `WEBHOOK_URL`

### Volumes

- `/mnt/storagepool/apps_config/n8n/portainer-restore-test`
- `/mnt/storagepool/master/n8n/know_base`
- `/mnt/storagepool/apps_config/n8n/postgres-data`

### Deployment

```bash
cd n8n-portainer-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
