<div align='center'>

# 🏠 **Home-Lab**

_A self-hosted infrastructure powering media, automation, productivity, and more._

![Docker](https://img.shields.io/badge/Docker-27.5.0-blue?logo=docker) ![TrueNAS](https://img.shields.io/badge/TrueNAS-25.04-success?logo=truenas) ![Containers](https://img.shields.io/badge/Containers-137_running-green) ![Stacks](https://img.shields.io/badge/Stacks-65-informational)

</div>

## 📊 Quick Stats

| Metric | Value |
|--------|-------|
| 🟢 Active Stacks | **57** |
| 🔴 Inactive Stacks | **8** |
| 🐳 Running Containers | **137** / 140 |
| ✅ Healthy Containers | **68** |
| 📦 Docker Images | **557** |
| 💾 Volumes | **957** |

## 🖥️ Server Hardware

<details>
<summary><b>Click to expand hardware specifications</b></summary>

| Component | Specification |
|-----------|--------------|
| **CPU** | AMD Ryzen 5 2600 6-Core (12 threads) |
| **RAM** | 125.7 GB |
| **HDD Storage** | 32 TB (HDD pool: /mnt/storagepool) |
| **NVMe Storage** | 870 GB (NVMe pool: /mnt/nvmepool) |
| **Operating System** | TrueNAS CE 25.04.2.6 |
| **Kernel** | 6.12.15-production+truenas |
| **Architecture** | x86_64 |
| **Docker Version** | 27.5.0 |
| **Storage Driver** | overlay2 on ZFS |
| **Cgroup** | v2 |
| **Hostname** | truenas-us |

</details>

## 📁 Stack Categories

### 🎬 Media & Entertainment

| Stack | Status | Description |
|-------|--------|-------------|
| [`arr-stack`](./arr-stack/) | 🟢 | The *Arr stack is a suite of media management applications for automating the... |
| [`immich-stack`](./immich-stack/) | 🟢 | Immich is a self-hosted photo and video backup solution, an alternative to Go... |
| [`immichframe-stack`](./immichframe-stack/) | 🟢 | ImmichFrame is a digital photo frame application that displays your Immich ph... |
| [`jellyfin-stack`](./jellyfin-stack/) | 🟢 | Jellyfin is a free and open-source media system that lets you stream your med... |
| [`jellyfin-telegram-stack`](./jellyfin-telegram-stack/) | 🟢 | Telegram bot integration for Jellyfin, providing notifications and control vi... |
| [`jellystat-stack`](./jellystat-stack/) | 🟢 | JellyStat is a statistics and monitoring dashboard for Jellyfin, tracking pla... |
| [`metube-stack`](./metube-stack/) | 🟢 | MeTube is a web GUI for yt-dlp, allowing you to download videos from YouTube ... |
| [`music-assistant-stack`](./music-assistant-stack/) | 🟢 | Music Assistant is a music library manager and player that integrates with st... |
| [`seerr-stack`](./seerr-stack/) | 🟢 | Overseerr / Jellyseerr — a request management portal for your media server, a... |
| [`tdarr-stack`](./tdarr-stack/) | 🔴 | Tdarr is a distributed transcoding system for automating media library health... |

### 🌐 Networking & VPN

| Stack | Status | Description |
|-------|--------|-------------|
| [`crowdsec-stack`](./crowdsec-stack/) | 🟢 | CrowdSec is a collaborative intrusion prevention and detection system that sh... |
| [`npm-stack`](./npm-stack/) | 🟢 | Nginx Proxy Manager provides a web interface for managing Nginx reverse proxy... |
| [`npmplus-stack`](./npmplus-stack/) | 🔴 | NPM Plus — an enhanced version of Nginx Proxy Manager with additional feature... |
| [`pihole-stack`](./pihole-stack/) | 🟢 | Pi-hole is a network-level ad and internet tracker blocking application actin... |
| [`searxng-stack`](./searxng-stack/) | 🟢 | SearXNG is a privacy-respecting metasearch engine that aggregates results fro... |
| [`unbound-stack`](./unbound-stack/) | 🔴 | Unbound is a validating, recursive, caching DNS resolver that provides DNSSEC... |
| [`vpn-stack`](./vpn-stack/) | 🟢 | WireGuard VPN server for secure remote access to the homelab network, providi... |
| [`wireguard-us-server-stack`](./wireguard-us-server-stack/) | 🟢 | WireGuard VPN server configured for US exit, providing secure tunneling with ... |

### 🔧 Infrastructure & Monitoring

| Stack | Status | Description |
|-------|--------|-------------|
| [`autoheal-stack`](./autoheal-stack/) | 🟢 | Autoheal monitors Docker containers and automatically restarts unhealthy ones... |
| [`beszel-stack`](./beszel-stack/) | 🟢 | Beszel is a lightweight server monitoring tool with a clean web UI for tracki... |
| [`census-stack`](./census-stack/) | 🔴 | Census provides infrastructure asset inventory and configuration management t... |
| [`graylog-stack`](./graylog-stack/) | 🔴 | Graylog is a centralized log management platform that collects, indexes, and ... |
| [`monitoring-stack`](./monitoring-stack/) | 🟢 | Full monitoring stack with Prometheus, Grafana, Alertmanager, and exporters f... |
| [`portracker-stack`](./portracker-stack/) | 🟢 | PortRacker is a network port tracking and service inventory tool for monitori... |
| [`stirling-pdf-stack`](./stirling-pdf-stack/) | 🟢 | Stirling PDF is a self-hosted web application for PDF manipulation — merge, s... |
| [`tugtainer-stack`](./tugtainer-stack/) | 🟢 | Tugtainer provides container management utilities and tools for Docker enviro... |

### 📝 Productivity & Collaboration

| Stack | Status | Description |
|-------|--------|-------------|
| [`book-stack`](./book-stack/) | 🟢 | BookStack is a self-hosted platform for organizing and storing documentation ... |
| [`collabora-stack`](./collabora-stack/) | 🟢 | Collabora Online is a LibreOffice-based online office suite that integrates w... |
| [`homarr-stack`](./homarr-stack/) | 🟢 | Homarr is a sleek, customizable dashboard for managing and accessing all your... |
| [`home-assistant-stack`](./home-assistant-stack/) | 🟢 | Home Assistant is an open-source home automation platform that integrates wit... |
| [`lubelogger-stack`](./lubelogger-stack/) | 🟢 | LubeLogger is a web-based vehicle maintenance and service record tracker for ... |
| [`matter-server`](./matter-server/) | 🟢 | Matter Server stack |
| [`mealie-stack`](./mealie-stack/) | 🟢 | Mealie is a self-hosted recipe manager and meal planner with a clean web inte... |
| [`nextcloud-stack`](./nextcloud-stack/) | 🟢 | Nextcloud is a self-hosted productivity platform providing file sharing, coll... |
| [`onlyoffice-stack`](./onlyoffice-stack/) | 🟢 | ONLYOFFICE Docs is an online office suite for creating, editing, and collabor... |
| [`paperlesngx-stack`](./paperlesngx-stack/) | 🟢 | Paperless-ngx is a document management system that scans, indexes, and archiv... |
| [`syncthing-stack`](./syncthing-stack/) | 🟢 | Syncthing is a continuous file synchronization program that syncs files betwe... |
| [`vaultwarden-stack`](./vaultwarden-stack/) | 🟢 | Vaultwarden is a lightweight Bitwarden-compatible password manager server wri... |
| [`vikunja-stack`](./vikunja-stack/) | 🟢 | Vikunja is an open-source to-do and project management application with kanba... |

### 🤖 AI & Development

| Stack | Status | Description |
|-------|--------|-------------|
| [`anything_llm-stack`](./anything_llm-stack/) | 🟢 | AnythingLLM is an all-in-one AI document chatbot — connect LLMs to your docum... |
| [`claude-code-stack`](./claude-code-stack/) | 🟢 | Claude Code provides an AI-powered code assistant environment for software de... |
| [`n8n-portainer-stack`](./n8n-portainer-stack/) | 🟢 | n8n is a workflow automation platform with a visual node-based editor for con... |
| [`ollama-stack`](./ollama-stack/) | 🔴 | Ollama runs large language models locally with a simple API, supporting Llama... |
| [`qdrant-stack`](./qdrant-stack/) | 🟢 | Qdrant is a high-performance vector similarity search engine for AI/ML applic... |

### 💰 Finance

| Stack | Status | Description |
|-------|--------|-------------|
| [`finboard-stack`](./finboard-stack/) | 🟢 | FinBoard is a financial dashboard for tracking investments, portfolio perform... |
| [`trading-agent-ron-stack`](./trading-agent-ron-stack/) | 🟢 | Trading Agent Ron is an automated trading bot infrastructure for monitoring a... |
| [`trailing-stop-stack`](./trailing-stop-stack/) | 🟢 | Trailing Stop provides automated trailing stop-loss order management for cryp... |

### 🎛️ Dashboards & Utilities

| Stack | Status | Description |
|-------|--------|-------------|
| [`dashapp-stack`](./dashapp-stack/) | 🟢 | DashApp provides a custom dashboard application for homelab service access an... |
| [`it-tools-stack`](./it-tools-stack/) | 🟢 | IT-Tools is a collection of handy online tools for developers — encoders, dec... |
| [`nebula-sync-stack`](./nebula-sync-stack/) | 🟢 | Nebula Sync provides configuration synchronization across multiple Pi-hole in... |
| [`reactive-resume-stack`](./reactive-resume-stack/) | 🟢 | Reactive Resume is a free and open-source resume builder with real-time colla... |
| [`sample-plan-stack`](./sample-plan-stack/) | 🟢 | Sample Plan is a template and planning tool for homelab project management. |
| [`wizarr-stack`](./wizarr-stack/) | 🟢 | Wizarr is a tool for managing invitations and onboarding for Plex/Jellyfin me... |

### ⚙️ Custom Applications

| Stack | Status | Description |
|-------|--------|-------------|
| [`bichon-ai-digest-stack`](./bichon-ai-digest-stack/) | 🟢 | Bichon AI Digest generates AI-powered content digests and summaries from vari... |
| [`bichon-stack`](./bichon-stack/) | 🟢 | Bichon is a custom homelab application for automation and service management. |
| [`journiv-stack`](./journiv-stack/) | 🟢 | Journiv is a journaling and life-tracking application for personal reflection... |
| [`karakeep-stack`](./karakeep-stack/) | 🟢 | Karakeep is a bookmark and knowledge management system for saving and organiz... |
| [`spartans-logistics`](./spartans-logistics/) | 🟢 | Spartans Logistics extends the Spartans platform with supply chain and logist... |
| [`spartans-stack`](./spartans-stack/) | 🔴 | Spartans is a custom application for homelab task coordination and team manag... |
| [`tracktor-stack`](./tracktor-stack/) | 🔴 | Tracktor is a tracking and monitoring application for managing assets, packag... |

### 📦 Other Stacks

| Stack | Status | Description |
|-------|--------|-------------|
| [`seafile-stack`](./seafile-stack/) | 🟢 | Seafile Stack stack |
| [`spartans-dashboard-stack`](./spartans-dashboard-stack/) | 🟢 | Spartans Dashboard Stack stack |
| [`spartans-events-stack`](./spartans-events-stack/) | 🟢 | Spartans Events Stack stack |
| [`spartans-maintenance`](./spartans-maintenance/) | 🟢 | Spartans Maintenance stack |
| [`spartans-practice`](./spartans-practice/) | 🟢 | Spartans Practice stack |

---

<div align='center'>

_Last synced: 2026-05-25 17:01 UTC_  
_Maintained by [Alex](https://github.com/ghp20) • Powered by [Portainer](https://www.portainer.io/)_

</div>
