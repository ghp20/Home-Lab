# spartans-logistics

Docker stack managed by Portainer

## Services

```
  • db
  • backend
  • frontend
```

## Key Env Vars

- `ACCESS_TOKEN_EXPIRE_MINUTES`
- `ADMIN_PASSWORD`
- `ADMIN_USERNAME`
- `CORS_ORIGINS`
- `DATABASE_URL`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `SECRET_KEY`

## Deployment

```bash
cd spartans-logistics
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration