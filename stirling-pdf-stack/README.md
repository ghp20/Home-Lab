# stirling-pdf-stack

PDF toolkit — Stirling-PDF

## Stack: stirling-pdf-stack

### Services

```
  • stirling-pdf
```

### Key Environment Variables

- `ALLOWED_HOSTS`
- `DOCKER_ENABLE_SECURITY`
- `LANGS`
- `PASSWORD`
- `PASSWORD_PROTECT`
- `SECURITY_ENABLELOGIN`
- `SERVER_PORT`
- `USERNAME`

### Volumes

- `/mnt/storagepool/apps_config/stirlingpdf/tesseract_data`
- `/mnt/storagepool/apps_config/stirlingpdf/config`
- `/mnt/storagepool/apps_config/stirlingpdf/files_storage`
- `/mnt/storagepool/apps_config/stirlingpdf/logs`
- `/mnt/storagepool/apps_config/stirlingpdf/pipeline`

### Deployment

```bash
cd stirling-pdf-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
