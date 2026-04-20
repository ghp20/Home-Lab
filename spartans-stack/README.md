# spartans-stack

Spartans web app

## Stack: spartans-stack

### Services

```
  • react-app
```

### Volumes

- `/mnt/storagepool/apps_config/Spartans/build`
- `/mnt/storagepool/master/build`

### Ports Exposed

- `3001`

### Deployment

```bash
cd spartans-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
