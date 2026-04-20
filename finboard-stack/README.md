# finboard-stack

Docker stack managed by Portainer

## Services

```
  • backend
  • frontend
  • internal
```

## Key Env Vars

- `APP_URL`
- `DB_BACKUP_DIR`
- `DB_PATH`
- `JWT_SECRET`
- `NODE_ENV`
- `PLAID_CLIENT_ID`
- `PLAID_ENV`
- `PLAID_SECRET`
- `PORT`
- `SMTP_FROM`
- `SMTP_HOST`
- `SMTP_PASS`
- `SMTP_PORT`
- `SMTP_SECURE`
- `SMTP_USER`

## Volumes

- `/mnt/storagepool/apps_config/finboard/db`
- `/mnt/storagepool/apps_config/finboard/backups`

## Ports

- `8092`

## Deployment

```bash
cd finboard-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration