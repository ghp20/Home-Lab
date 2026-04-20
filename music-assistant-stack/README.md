# music-assistant-stack

Music streaming — Music Assistant

## Stack: music-assistant-stack

### Services

```
  • music-assistant-server
```

### Key Environment Variables

- `LOG_LEVEL`
- `MASS_DISABLE_ZEROCONF`

### Ports Exposed

- `8095`

### Deployment

```bash
cd music-assistant-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
