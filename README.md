# Home-Lab

Personal homelab running on TrueNAS SCALE with 60+ Docker containers, managed via Portainer.

## Hardware

- **TrueNAS SCALE** server on-premises
- Storage: ZFS pool with multiple datasets
- Network: your-network-subnet

## Architecture

All services run as Docker containers on TrueNAS SCALE, deployed and managed through **Portainer**. Most services use a shared `arrnet` Docker network for inter-container communication. Graylog collects centralized logs from all containers via GELF.

### Key Design Patterns

- **Media Stack**: Prowlarr, Radarr, Sonarr, Bazarr, LazyLibrarian for automated media acquisition and management
- **LLM Stack**: Ollama, Anything-LLM for local AI inference and chat
- **Monitoring**: Grafana + Prometheus for metrics, Graylog for logs, Scrutiny for HDD S.M.A.R.T., CrowdSec for threat detection
- **VPN**: Gluetun (WireGuard-based) for VPN connectivity for media containers

## Services

### Media
| Service | Description |
|---------|-------------|
| Jellyfin | Media server (video/movies/TV) |
| Jellyfin-Telegram | Telegram bot for Jellyfin notifications |
| Plex | Alternative media server |
| Radarr | Movie management for Sonarr/Radarr |
| Sonarr | TV show management |
| Prowlarr | Indexer manager |
| Bazarr | Subtitle management |
| LazyLibrarian | eBook download manager |
| SABnzbd | Usenet downloader |
| qBittorrent | BitTorrent client |
| Bitmagnet | Bittorrent indexer |
| MeTube | YouTube downloader |

### AI & LLM
| Service | Description |
|---------|-------------|
| Ollama | Local LLM inference engine |
| Anything-LLM | Chat interface for local LLMs |
| n8n | Workflow automation with AI integrations |

### Document Management
| Service | Description |
|---------|-------------|
| Paperless-NGX | Document scanning and归档 |
| Bookshelf | Personal book library |
| Calibre-Web | eBook management |
| Audiobookshelf | Audiobook server |

### Cloud & Sync
| Service | Description |
|---------|-------------|
| Nextcloud | Self-hosted cloud drive |
| Syncthing | File synchronization |
| Nebula-Sync | Sync between Nebula nodes |

### Home Automation
| Service | Description |
|---------|-------------|
| Home Assistant | Smart home hub |
| Matter-Server | Matter protocol server |

### Security
| Service | Description |
|---------|-------------|
| Vaultwarden | Self-hosted password manager |
| CrowdSec | Threat detection and banning |
| Cloudflared | Cloudflare tunnel for remote access |
| Tailscale | VPN for remote access |
| WireGuard | VPN server |

### Finance
| Service | Description |
|---------|-------------|
| Firefly III | Personal finance manager |
| Finboard | Financial dashboard |
| GnuCash | Accounting (via Docker) |

### Development
| Service | Description |
|---------|-------------|
| n8n | Workflow automation |
| Claude-Code | AI coding assistant |
| Ollama | Local LLM for dev |

### Home Lab Management
| Service | Description |
|---------|-------------|
| Portainer | Container management UI |
| Homarr | Dashboard/app launcher |
| Grafana | Metrics dashboards |
| Prometheus | Metrics collection |
| Graylog | Centralized logging |
| Scrutiny | HDD health monitoring |
| NodeExporter | System metrics for Prometheus |
| CrowdSec | Security log analysis |

### Automation & Utility
| Service | Description |
|---------|-------------|
| n8n | Workflow automation |
| Changedetection | Website change monitoring |
| Invoice Ninja | Self-hosted invoicing |
| Tandoor Recipes | Recipe manager |
| Mealie | Meal planning |
| Wizarr | Media library organizer |
| Stirling-PDF | PDF toolkit |
| It-Tools | Developer utilities |

## Quick Start

1. Clone this repo
2. Copy the `docker-compose.yaml` for the service you want
3. Update paths (`/path/to/your/data`) to match your storage layout
4. Update secrets (`changeme`) to strong passwords
5. Deploy with `docker compose up -d` or via Portainer

## Repository Structure

Each folder = one service or stack. Most are single `docker-compose.yaml` files. Some stacks (like `Arr-stack`) contain multiple related containers.

```
homelab/
├── Arr-stack/         # Prowlarr, Radarr, Sonarr, Bazarr, LazyLibrarian
├── Jellyfin/          # Media server
├── Nextcloud/         # Cloud drive
├── Home-Assistant/    # Smart home
├── Portainer/         # Container management
├── Grafana-Prometheus/ # Monitoring
├── Graylog/           # Centralized logging
└── ...                # 60+ more services
```

## Notes

- All compose files are sanitized — real paths, IPs, and secrets replaced with placeholders
- Volumes reference `/path/to/your/data` — adjust to your actual storage paths
- Most LinuxServer.io containers use `PUID=1000`, `PGID=1000` — adjust to match your user IDs
- Graylog GELF logging is enabled on most stacks for centralized log collection

## License

MIT — feel free to use and adapt for your own homelab.
