# nextcloud-stack

Docker stack managed by Portainer

## Services

```
  • nextcloud
  • postgres
  • redis
  • imaginary
  • cron
```

## Deployment

```bash
cd nextcloud-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration