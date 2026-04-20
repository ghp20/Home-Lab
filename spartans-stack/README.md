# spartans-stack

Docker stack managed by Portainer

## Services

```
  • react-app
```

## Volumes

- `/mnt/storagepool/apps_config/Spartans/build`
- `/mnt/storagepool/master/build`

## Ports

- `3001`

## Deployment

```bash
cd spartans-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration