# 🏠 Home Lab — Docker Compose Infrastructure

> **Gaurav's self-hosted homelab** — 71 Docker stacks running 100+ containers on TrueNAS Scale.
> Everything from media management to AI, finance tracking to smart home automation.

**🟢 54 Active** | **🔴 17 Inactive** | **📦 71 Total Stacks** | **🔄 Last Sync: 2026-05-01 19:02 UTC**

---

## 🖥 Server Hardware

| Component | Specification |
|-----------|---------------|
| **CPU** | AMD Ryzen 5 2600 — 6 Cores / 12 Threads @ 3.40 GHz |
| **RAM** | 128 GB DDR4 |
| **Storage Pool** | 32 TB ZFS (storagepool) |
| **NVMe Pool** | 870 GB NVMe (nvmepool) |
| **OS** | TrueNAS SCALE 25.04.2.6 (Debian 12 Bookworm) |
| **Kernel** | 6.12.15-production+truenas |
| **Docker** | 27.5.0 (overlay2) |
| **Network** | 1 GbE — LAN: 192.168.1.0/24 |
| **VPN** | Tailscale + WireGuard (Gluetun for container VPN) |
| **Reverse Proxy** | Nginx Proxy Manager + Let's Encrypt SSL |
| **DNS / Ad Block** | Pi-hole + Unbound recursive resolver |

## 🏗 Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    INTERNET                              │
│  ┌──────────┐  ┌──────────┐  ┌──────────────────────┐  │
│  │ Tailscale│  │ WireGuard│  │ Cloudflare (CrowdSec) │  │
│  └────┬─────┘  └────┬─────┘  └──────────┬───────────┘  │
└───────┼──────────────┼──────────────────┼───────────────┘
        │              │                  │
┌───────┴──────────────┴──────────────────┴───────────────┐
│              Nginx Proxy Manager (:80/:443)              │
│              ┌──────────────────────┐                    │
│              │   Let's Encrypt SSL  │                    │
│              └──────────────────────┘                    │
│  ┌──────────────────────────────────────────────────┐   │
│  │               Docker Services                     │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌───────┐  │   │
│  │  │  Media  │ │  *Arr   │ │ Finance │ │  AI   │  │   │
│  │  │ Stack   │ │  Stack  │ │ Stacks  │ │ Stack │  │   │
│  │  └─────────┘ └─────────┘ └─────────┘ └───────┘  │   │
│  └──────────────────────────────────────────────────┘   │
│  ┌──────────────────────────────────────────────────┐   │
│  │            Monitoring & Infrastructure            │   │
│  │  ┌─────────┐ ┌──────────┐ ┌──────────────────┐   │   │
│  │  │Prometheus│ │ Grafana  │ │  Beszel + Auto-  │   │   │
│  │  │          │ │          │ │  heal monitoring  │   │   │
│  │  └─────────┘ └──────────┘ └──────────────────┘   │   │
│  └──────────────────────────────────────────────────┘   │
│         TrueNAS SCALE — AMD Ryzen 5 2600                │
│              128 GB RAM | 32 TB Storage                 │
└─────────────────────────────────────────────────────────┘
```

---

## 📂 Stack Index

### ⚡ Media & Entertainment

| Stack | Status | Description |
|-------|--------|-------------|
| [arr-stack](./arr-stack/) | 🟢 | Complete *Arr stack — Prowlarr, Radarr, Sonarr, Bazarr, LazyLibrarian, Cleanuparr |
| | | Services: `options` · `arrnet` · `prowlarr` · `radarr` · `sonarr` +3 more |
| [immich-stack](./immich-stack/) | 🟢 | Self-hosted Google Photos alternative — photo/video backup with AI face recognition |
| | | Services: `immich-server` · `immich-machine-learning` · `redis` · `database` · `immich-ml-cache` |
| [jellyfin-stack](./jellyfin-stack/) | 🟢 | Open-source media server — stream movies, TV, music to any device |
| | | Services: `jellyfin` |
| [jellyfin-telegram-stack](./jellyfin-telegram-stack/) | 🟢 | Telegram bot integration for Jellyfin — notifications and remote control |
| | | Services: `jellyfin-telegram` |
| [jellystat-stack](./jellystat-stack/) | 🟢 | Jellyfin analytics dashboard — track media consumption stats |
| | | Services: `jellystat-db` · `jellystat` |
| [seerr-stack](./seerr-stack/) | 🟢 | Media request & discovery platform — Overseerr/Jellyseerr for your users |
| | | Services: `seerr-db` · `seerr` |
| [music-assistant-stack](./music-assistant-stack/) | 🟢 | Multi-room audio streaming — connect Spotify, local files, streaming services |
| | | Services: `music-assistant-server` |
| [immichframe-stack](./immichframe-stack/) | 🟢 | Digital photo frame powered by Immich — slideshow display |
| | | Services: `immichframe` |
| [metube-stack](./metube-stack/) | 🟢 | YouTube video downloader with web UI — grab videos locally |
| | | Services: `metube` |
| [plex-stack](./plex-stack/) | 🔴 | Plex Media Server — alternative media streaming (currently inactive) |
| | | Services: `plex` |
| [tdarr-stack](./tdarr-stack/) | 🔴 | Distributed media transcoding — automate codec/quality optimization |
| | | Services: `tdarr` · `tdarr-node` |

### 🔒 Networking & VPN

| Stack | Status | Description |
|-------|--------|-------------|
| [vpn-stack](./vpn-stack/) | 🟢 | VPN-protected download stack — Gluetun + qBittorrent + SABnzbd + Bitmagnet |
| | | Services: `arrnet` · `options` · `gluetun` · `qbittorrent` · `sabnzbd` +3 more |
| [wireguard-us-server-stack](./wireguard-us-server-stack/) | 🟢 | WireGuard VPN server — secure remote access to homelab |
| | | Services: `options` · `wireguard-us-server` |
| [npm-stack](./npm-stack/) | 🟢 | Nginx Proxy Manager — reverse proxy with Let's Encrypt SSL automation |
| | | Services: `npm` |
| [npmplus-stack](./npmplus-stack/) | 🔴 | Enhanced NPM with CrowdSec integration — advanced reverse proxy |
| | | Services: `npmplus` · `default` · `crowdsec_net` |
| [pihole-stack](./pihole-stack/) | 🟢 | Network-wide ad blocking via DNS — block ads on every device |
| | | Services: `pihole` |
| [unbound-stack](./unbound-stack/) | 🔴 | Recursive DNS resolver — privacy-first DNS resolution |
| | | Services: `unbound` |
| [crowdsec-stack](./crowdsec-stack/) | 🟢 | Collaborative security engine + Cloudflare bouncer — DDoS/brute-force protection |
| | | Services: `crowdsec` · `crowdsec-cloudflare-bouncer` · `crowdsec-net` |
| [searxng-stack](./searxng-stack/) | 🟢 | Privacy-respecting metasearch engine — search without tracking |
| | | Services: `redis` · `searxng` |
| [changedetection-stack](./changedetection-stack/) | 🟢 | Website change monitor — get alerted when pages update |
| | | Services: `changedetection` · `browser-sockpuppet-chrome` · `changedetection_net` |
| [dispatcharr-stack](./dispatcharr-stack/) | 🔴 | Arr dispatch with VPN routing — media automation behind VPN |
| | | Services: `dispatcharr` · `gluetun-iptv` |

### 🖥 Infrastructure & Monitoring

| Stack | Status | Description |
|-------|--------|-------------|
| [monitoring-stack](./monitoring-stack/) | 🟢 | Prometheus + Grafana — full system and container monitoring |
| | | Services: `prometheus` · `grafana` · `monitoring-net` |
| [beszel-stack](./beszel-stack/) | 🟢 | Lightweight server monitoring hub — agent-based multi-server tracking |
| | | Services: `beszel` · `beszel-agent` |
| [autoheal-stack](./autoheal-stack/) | 🟢 | Container auto-healer — automatically restart unhealthy containers |
| | | Services: `autoheal` |
| [portracker-stack](./portracker-stack/) | 🟢 | Port tracker — monitor which services are running on which ports |
| | | Services: `portracker` |
| [tugtainer-stack](./tugtainer-stack/) | 🟢 | Container management utilities — networking and Docker helpers |
| | | Services: `app` |
| [stirling-pdf-stack](./stirling-pdf-stack/) | 🟢 | Web-based PDF toolkit — merge, split, convert, OCR, sign PDFs |
| | | Services: `stirling-pdf` |
| [graylog-stack](./graylog-stack/) | 🔴 | Centralized log management — aggregate and analyze all server logs |
| | | Services: `graylog_net` · `mongodb` · `datanode` · `graylog` |
| [census-stack](./census-stack/) | 🔴 | Container census — inventory of deployed containers |
| | | Services: `options` · `census-server` |

### 📦 Productivity & Collaboration

| Stack | Status | Description |
|-------|--------|-------------|
| [nextcloud-stack](./nextcloud-stack/) | 🟢 | Self-hosted cloud — file sync, calendar, contacts, talk, and apps |
| | | Services: `nextcloud` · `postgres` · `redis` · `imaginary` · `cron` |
| [onlyoffice-stack](./onlyoffice-stack/) | 🟢 | Office document server — collaborative doc editing for Nextcloud |
| | | Services: `onlyoffice-document-server` |
| [collabora-stack](./collabora-stack/) | 🟢 | LibreOffice Online — browser-based document collaboration |
| | | Services: `options` · `collabora` |
| [vaultwarden-stack](./vaultwarden-stack/) | 🟢 | Self-hosted Bitwarden — secure password manager for all devices |
| | | Services: `db` · `vaultwarden` · `vaultwarden-net` |
| [vikunja-stack](./vikunja-stack/) | 🟢 | Task & project management — to-do lists, kanban, gantt charts |
| | | Services: `vikunja` · `db` · `vikunja_net` |
| [book-stack](./book-stack/) | 🟢 | Complete book stack — Calibre, Audiobookshelf, Calibre-Web for ebooks & audiobooks |
| | | Services: `books_net` · `bookshelf` · `calibre` · `calibre-web` · `audiobookshelf` +1 more |
| [paperlesngx-stack](./paperlesngx-stack/) | 🟢 | Document management — scan, OCR, tag, and search all your paperwork |
| | | Services: `postgres` · `redis` · `tika` · `gotenberg` · `paperless` |
| [mealie-stack](./mealie-stack/) | 🟢 | Recipe manager & meal planner — import from any website, plan meals |
| | | Services: `postgres` · `mealie` · `default` |
| [lubelogger-stack](./lubelogger-stack/) | 🟢 | Vehicle maintenance log — track services, fuel, expenses for your cars |
| | | Services: `lubelogger` |
| [homarr-stack](./homarr-stack/) | 🟢 | Service dashboard — beautiful homepage for all your self-hosted apps |
| | | Services: `homarr` · `homarr-network` |
| [home-assistant-stack](./home-assistant-stack/) | 🟢 | Smart home platform — control lights, sensors, automations |
| | | Services: `postgres` · `homeassistant` |
| [matter-server](./matter-server/) | 🟢 | Matter/Thread device server — connect smart home devices to Home Assistant |
| | | Services: `matter-server` |
| [syncthing-stack](./syncthing-stack/) | 🟢 | P2P file sync — continuous, private file synchronization across devices |
| | | Services: `syncthing` |
| [tandoor-recipes-stack](./tandoor-recipes-stack/) | 🔴 | Recipe management — collect, organize, and share recipes |
| | | Services: `postgres` · `tandoor` |

### 🤖 AI & Development

| Stack | Status | Description |
|-------|--------|-------------|
| [anything_llm-stack](./anything_llm-stack/) | 🟢 | Multi-LLM chat interface — unified frontend for OpenAI, Ollama, Anthropic |
| | | Services: `options` · `anything-llm` |
| [ollama-stack](./ollama-stack/) | 🔴 | Run LLMs locally — Llama, Mistral, Gemma and more on your own hardware |
| | | Services: `ollama` |
| [claude-code-stack](./claude-code-stack/) | 🟢 | Claude Code dev environment — AI-assisted coding in containers |
| | | Services: `claude-code` |
| [qdrant-stack](./qdrant-stack/) | 🟢 | Vector database — semantic search and RAG for AI applications |
| | | Services: `qdrant` |
| [n8n-portainer-stack](./n8n-portainer-stack/) | 🟢 | Workflow automation — connect APIs, services, and trigger automations |
| | | Services: `n8n` · `n8n-postgres` · `default` · `trading-net-ron` |

### 💰 Finance

| Stack | Status | Description |
|-------|--------|-------------|
| [trailing-stop-stack](./trailing-stop-stack/) | 🟢 | Trailing stop trading system — automated stock/crypto stop-loss |
| | | Services: `trading_net` · `db` · `agent` |
| [firefly3-stack](./firefly3-stack/) | 🔴 | Personal finance manager — track expenses, budgets, and bank transactions |
| | | Services: `firefly-db` · `firefly-iii` · `firefly-importer` |
| [finboard-stack](./finboard-stack/) | 🟢 | Investment dashboard — portfolio tracking with charts and analytics |
| | | Services: `backend` · `frontend` |
| [cashlytics-stack](./cashlytics-stack/) | 🔴 | AI expense analytics — smart categorization of spending |
| | | Services: `postgres` · `cashlytics` · `cashlytics-cron` |
| [monetr-stack](./monetr-stack/) | 🔴 | Budgeting & financial planning — envelope-based budgeting |
| | | Services: `monetr` · `monetr-postgres` · `monetr-valkey` |
| [split-pro-stack](./split-pro-stack/) | 🔴 | Expense splitting — track and settle shared costs |
| | | Services: `postgres` · `splitpro` |
| [trading-agent-ron-stack](./trading-agent-ron-stack/) | 🟢 | AI trading agent — automated stock/crypto trading strategies |
| | | Services: `trading-agent-ron` · `trading-postgres-ron` · `trading-redis-ron` |

### 📊 Dashboards & Utilities

| Stack | Status | Description |
|-------|--------|-------------|
| [dashapp-stack](./dashapp-stack/) | 🟢 | Custom Python dashboard — Plotly Dash application |
| | | Services: `dashapp` |
| [it-tools-stack](./it-tools-stack/) | 🟢 | Developer toolbox — base64, JSON, UUID, jwt, hash generators |
| | | Services: `it-tools` |
| [reactive-resume-stack](./reactive-resume-stack/) | 🟢 | Resume builder — free, modern, ATS-friendly resume templates |
| | | Services: `postgres` · `printer` · `app` |
| [wizarr-stack](./wizarr-stack/) | 🟢 | Media invitation system — onboard users to your media servers |
| | | Services: `wizarr` · `wizarr_postgres` · `wizarr_redis` · `wizarr_memcached` |
| [nebula-sync-stack](./nebula-sync-stack/) | 🟢 | Pi-hole sync — keep multiple Pi-hole instances in sync |
| | | Services: `orbital-sync` |
| [sample-plan-stack](./sample-plan-stack/) | 🟢 | Sample planning app — manage and organize samples/templates |
| | | Services: `backend` · `frontend` |

### 🚀 Custom Applications

| Stack | Status | Description |
|-------|--------|-------------|
| [bichon-stack](./bichon-stack/) | 🟢 | Bichon mail service — custom email delivery platform |
| | | Services: `bichon` |
| [bichon-ai-digest-stack](./bichon-ai-digest-stack/) | 🟢 | AI-powered email digests — summarize newsletters and updates |
| | | Services: `bichon-ai-digest` |
| [spartans-stack](./spartans-stack/) | 🟢 | Spartans blog platform — React-based content site |
| | | Services: `react-app` |
| [spartans-logistics](./spartans-logistics/) | 🟢 | Spartans logistics — inventory and order tracking system |
| | | Services: `db` · `backend` · `frontend` |
| [journiv-stack](./journiv-stack/) | 🟢 | Journiv travel logger — document and share your travels |
| | | Services: `options` · `postgres` · `redis` · `celery-worker` · `app` +2 more |
| [adventurlog-stack](./adventurlog-stack/) | 🔴 | Adventure log — track outdoor adventures and trips |
| | | Services: `options` · `db` · `backend` · `frontend` |
| [timelinize-stack](./timelinize-stack/) | 🔴 | Personal timeline — visualize your life events on a timeline |
| | | Services: `timelinize` |
| [tracktor-stack](./tracktor-stack/) | 🔴 | Equipment tracker — log and monitor equipment usage |
| | | Services: `app` |
| [wygiwyh-stack](./wygiwyh-stack/) | 🔴 | Expense tracker — WYGIWYH personal finance |
| | | Services: `db` · `wygiwyh` |
| [karakeep-stack](./karakeep-stack/) | 🟢 | Bookmark & content hoarder — AI-tagged bookmarking platform |
| | | Services: `options` · `web` · `chrome` · `meilisearch` |

---

## 🚀 Quick Start

To deploy any stack from this repository:

1. **Clone** the stack directory
2. **Update** `changeme` values in the docker-compose.yaml
3. **Adjust** volume paths to your environment
4. **Deploy** with `docker compose up -d`

> ⚠️ All secrets and passwords in this repository have been **sanitized**. Replace `changeme` values with real credentials before deploying.

## 🔒 Security Note

This repository is a **sanitized export** from Portainer. All passwords, API keys, domain names, and internal IPs have been replaced with placeholders. No real credentials are stored here.

---

*📝 Auto-synced from Portainer via the GitHub Portainer Sync job (Alex). Maintained manually for detailed documentation.*
