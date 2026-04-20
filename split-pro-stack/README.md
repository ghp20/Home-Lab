# split-pro-stack

Split expense tracker

## Stack: split-pro-stack

### Services

```
  • postgres
  • splitpro
```

### Key Environment Variables

- `AUTH_EMAIL_ENABLED`
- `DATABASE_URL`
- `DISABLE_EMAIL_SIGNUP`
- `EMAIL_SERVER_HOST`
- `EMAIL_SERVER_PASSWORD`
- `EMAIL_SERVER_PORT`
- `EMAIL_SERVER_USER`
- `ENABLE_SENDING_INVITES`
- `FROM_EMAIL`
- `NEXTAUTH_SECRET`
- `NEXTAUTH_URL`
- `NEXTAUTH_URL_INTERNAL`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`

### Volumes

- `/mnt/storagepool/apps_config/split-pro/postgres17`
- `/mnt/storagepool/apps_config/split-pro/uploads`

### Ports Exposed

- `3020`

### Deployment

```bash
cd split-pro-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
