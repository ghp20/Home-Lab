# onlyoffice-stack

Online office suite — OnlyOffice

## Stack: onlyoffice-stack

### Services

```
  • onlyoffice-document-server
```

### Key Environment Variables

- `JWT_ENABLED`
- `JWT_SECRET`

### Volumes

- `/mnt/storagepool/apps_config/onlyoffice/data`
- `/mnt/storagepool/apps_config/onlyoffice/logs`

### Ports Exposed

- `8082`

### Deployment

```bash
cd onlyoffice-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
