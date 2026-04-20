# claude-code-stack

Claude Code CLI

## Stack: claude-code-stack

### Services

```
  • claude-code
```

### Key Environment Variables

- `ANTHROPIC_API_KEY`
- `CLAUDE_DISABLE_OAUTH`
- `PATH`

### Volumes

- `/mnt/storagepool/apps_config/claude-code`
- `/mnt/storagepool/master/claude-code`

### Deployment

```bash
cd claude-code-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
