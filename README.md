# Awesome NAS [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of NAS (Network-attached storage) resources and projects.

[![Stars](https://img.shields.io/github/stars/AwesomeDog/awesome-nas?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/stargazers) [![Forks](https://img.shields.io/github/forks/AwesomeDog/awesome-nas?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/network/members) [![Issues](https://img.shields.io/github/issues/AwesomeDog/awesome-nas?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/issues) [![Pull Requests](https://img.shields.io/github/issues-pr/AwesomeDog/awesome-nas?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/pulls) [![Contributors](https://img.shields.io/github/contributors/AwesomeDog/awesome-nas?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/graphs/contributors) [![Last commit](https://img.shields.io/github/last-commit/AwesomeDog/awesome-nas?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/commits/main) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/AwesomeDog/awesome-nas/pulls)

# Contents

- [What is NAS?](#what-is-nas)
- [Where to start?](#where-to-start)
- [Hardware](#hardware)
- [Operating Systems](#operating-systems)
- [Storage & Filesystem](#storage--filesystem)
- [Backup & Sync](#backup--sync)
- [File Access & Sharing](#file-access--sharing)
- [Media](#media)
- [Download](#download)
- [Productivity](#productivity)
- [Communication & Social](#communication--social)
- [Education](#education)
- [Entertainment](#entertainment)
- [Finance](#finance)
- [Home Automation & Life](#home-automation--life)
- [Network & Remote Access](#network--remote-access)
- [Monitoring & Health](#monitoring--health)
- [Dashboards & Containers](#dashboards--containers)
- [Security & Identity](#security--identity)
- [Automation](#automation)
- [AI](#ai)
- [Dev & Coding](#dev--coding)
- [Useful articles](#useful-articles)
- [Books](#books)
- [Videos](#videos)

# What is NAS?

> **Network-attached storage** (**NAS**) is a file-level (as opposed
> to [block-level storage](https://en.wikipedia.org/wiki/Block-level_storage "Block-level storage"))
> [computer data storage](https://en.wikipedia.org/wiki/Computer_data_storage "Computer data storage")
> server connected to a [computer network](https://en.wikipedia.org/wiki/Computer_network "Computer network")
> providing data access to a
> [heterogeneous](https://en.wikipedia.org/wiki/Heterogeneous_computing "Heterogeneous computing") group
> of clients. The term "NAS" can refer to both the technology and systems involved, or a specialized device
> built for such functionality (as unlike tangentially related technologies such
> as [local area networks](https://en.wikipedia.org/wiki/Local_area_network "Local area network"), a NAS
> device is often a singular unit).

_Source:_ [Network-attached storage](https://en.wikipedia.org/wiki/Network-attached_storage)

# Where to start?

- [Why I Built My Own Personal Cloud](https://medium.com/@T_Jen/why-i-built-my-own-personal-cloud-6fb426f61973) — why a NAS beats renting storage from the big cloud providers.
- [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) — the much larger sibling list; anything you can run on a NAS is in here.
- [r/selfhosted](https://www.reddit.com/r/selfhosted/) and [r/DataHoarder](https://www.reddit.com/r/DataHoarder/) — the two most active communities for this stuff.
- [ServeTheHome](https://www.servethehome.com/) — hardware reviews, NAS builds and homelab gear.

# Hardware

- [Synology](https://www.synology.com/) — the most widely used turnkey NAS brand; DiskStation Manager (DSM) is a polished, app-driven NAS OS.
- [QNAP](https://www.qnap.com/) — _QNAP_ designs and delivers high-quality network attached storage (NAS) and professional network video recorder (NVR) solutions.
- [TerraMaster](https://www.terra-master.com/) — budget-friendly multi-bay NAS enclosures, popular with DIY builders.
- [UGREEN NAS](https://www.ugreen.com/) — newer entrant in the consumer NAS space, strong hardware-per-price and an actively developed OS.

# Operating Systems

- [TrueNAS](https://www.truenas.com/) — World's most deployed storage OS with >1M deployments worldwide. Trusted by thousands of companies and organizations, including more than 40% of the Fortune 500.
- [Unraid](https://unraid.net/) — Commercial NAS OS with a flexible array (no RAID striping, mix drive sizes freely) and first-class Docker/VM support. Very popular with homelabbers.
- [Proxmox VE](https://www.proxmox.com/en/) — Hypervisor many people run _underneath_ a NAS; lets you virtualize TrueNAS/OMV and run containers on the same box.
  - [Proxmox VE Helper-Scripts (Community Edition)](https://github.com/community-scripts/ProxmoxVE) — one-command installers for hundreds of homelab apps on Proxmox.
- [openmediavault](https://www.openmediavault.org/) — The next generation NAS solution based on Debian Linux. Contains services like SSH, (S)FTP, SMB/CIFS, RSync and many more ready to use.
- [Rockstor](https://rockstor.com/) — Linux/BTRFS based NAS; Rockstor as a Cloud and Storage platform enables hackers, makers/re-distributors, and DIYers to build completely custom solutions.
- [CasaOS](https://github.com/IceWhaleTech/CasaOS) — A simple, easy-to-use, elegant open-source Personal Cloud system. Great starting point if you just want Docker apps on a spare machine.
- [ZimaOS](https://github.com/IceWhaleTech/ZimaOS) — A simplified, focused and open NAS OS from the CasaOS team, aimed at dedicated NAS hardware.
- [Runtipi](https://github.com/runtipi/runtipi) — A homeserver for everyone: one command setup, one click installs for your favorite self-hosted apps.
- [Umbrel](https://github.com/getumbrel/umbrel) — An elegant home server OS with a large curated app store.
- [Cosmos-Server](https://github.com/azukaar/Cosmos-Server) — Self-hosted home server platform with built-in reverse proxy, auth and container management.
- [YunoHost](https://github.com/YunoHost/yunohost) — An operating system aiming to simplify as much as possible the administration of a server; single sign-on across packaged apps.
- [arozos](https://github.com/tobychui/arozos) — Web Desktop Operating System for low power platforms, now written in Go!

# Storage & Filesystem

- [OpenZFS](https://openzfs.github.io/openzfs-docs/) — The filesystem behind TrueNAS/Proxmox. Copy-on-write, checksums, snapshots, send/receive replication and native RAID-Z.
- [mergerfs](https://github.com/trapexit/mergerfs) — FUSE union filesystem that pools drives of different sizes into one mount point without RAID; pairs naturally with SnapRAID.
- [SnapRAID](https://www.snapraid.it/) — Snapshot-based parity for disk arrays; unlike RAID it can be added to an existing pool of used disks and recovers from up to 6 disk failures.
- [OutletPicks RAID Calculator](https://www.outletpicks.com/raid-calculator) — Usable space and drives that can fail for RAID 0/1/5/6/10, Synology SHR/SHR-2 and ZFS RAID-Z1/2/3, mixed drive sizes included, with the TiB figure the NAS displays and the cost per usable TB at current NAS drive prices.

# Backup & Sync

- [restic](https://github.com/restic/restic) — Fast, secure, efficient backup program with deduplication and encryption; backs up to local disk, SFTP, S3, B2 and more.
- [BorgBackup](https://github.com/borgbackup/borg) — Deduplicating archiver with compression and authenticated encryption.
- [Kopia](https://github.com/kopia/kopia) — Cross-platform backup tool with fast incremental backups, client-side encryption and snapshot-style restore UI.
- [Duplicati](https://github.com/duplicati/duplicati) — Store securely encrypted backups in the cloud; friendly web UI, good fit for scheduled NAS-to-cloud jobs.
- [rclone](https://github.com/rclone/rclone) — "rsync for cloud storage"; sync, mount and migrate between 40+ cloud providers and your NAS.
- [Syncthing](https://github.com/syncthing/syncthing) — Open source continuous file synchronization between your devices, no central server required.
- [Nextcloud](https://github.com/nextcloud/server) — ☁️ A safe home for all your data: files, contacts, calendars and office documents with a huge app ecosystem.
- [Seafile](https://github.com/haiwen/seafile) — High-performance file syncing and sharing with per-file encryption and library versioning.

# File Access & Sharing

- [OpenList](https://github.com/OpenListTeam/OpenList) — A new AList fork: a file list program that supports multiple storages, powered by Gin and Solidjs.
- [File Browser Quantum](https://github.com/gtsteffaniak/filebrowser) — 📂 Web file browser for your NAS shares with multi-user access, sharing and search.
- [copyparty](https://github.com/9001/copyparty) — Portable file server with accelerated resumable uploads, dedup, WebDAV, SFTP, FTP, TFTP and zeroconf discovery.

# Media

## Media servers

- [Jellyfin](https://github.com/jellyfin/jellyfin) — The Free Software Media System. Volunteer-built, puts _you_ in control of your media; stream to any device from your own server, no strings attached.
- [Plex](https://github.com/plexinc/pms-docker) — The most polished commercial media server; rich client apps everywhere, remote streaming without any network setup.
_Note:_ Emby is intentionally not listed. Its GitHub repository has been dormant since March 2024 and the project is now closed-source; [Jellyfin](https://github.com/jellyfin/jellyfin) is its actively developed open-source fork and is listed above.

## Photos & videos

- [immich](https://github.com/immich-app/immich) — High performance self-hosted photo and video management solution; the current go-to Google Photos replacement.
- [PhotoPrism](https://github.com/photoprism/photoprism) — AI-powered self-hosted photo app with browsing, search, people recognition and maps.
- [Photoview](https://github.com/photoview/photoview) — Lightweight photo gallery for self-hosted personal servers.

## Music, books & comics

- [navidrome](https://github.com/navidrome/navidrome) — 🎧☁️ Your personal streaming service for your own music library; Subsonic-compatible.
- [audiobookshelf](https://github.com/advplyr/audiobookshelf) — Self-hosted audiobook and podcast server.
- [komga](https://github.com/gotson/komga) — Media server for comics/mangas/BDs/magazines/eBooks with API, OPDS, Kobo Sync and KOReader Sync support.
- [Kavita](https://github.com/Kareadita/Kavita) — Fast, feature-rich, cross-platform reading server; a popular alternative to Komga.
- [radishes](https://github.com/radishes-music/radishes) — Cross-platform copyright-free music platform (支持 windows / macos / linux / web).

## Media automation (\*arr stack)

- [MoviePilot](https://github.com/jxxghp/MoviePilot) — NAS 媒体库自动化管理工具. Automated media library search, rename and organise; the actively maintained successor to the now-removed `nas-tools` by the same author.
- [Sonarr](https://github.com/Sonarr/Sonarr) — Smart PVR for newsgroup and bittorrent users; automatic TV show search and management.
- [Radarr](https://github.com/Radarr/Radarr) — Movie organizer/manager for usenet and torrent users; the movie counterpart to Sonarr.
- [Lidarr](https://github.com/Lidarr/Lidarr) — Looks and smells like Sonarr, but made for music.
- [Bazarr](https://github.com/morpheus65535/bazarr) — Companion to Sonarr and Radarr that manages and downloads subtitles.
- [Seerr](https://github.com/seerr-team/seerr) — Open-source media request and discovery manager for Jellyfin, Plex and Emby.
- [Auto_Bangumi](https://github.com/EstrellaXD/Auto_Bangumi) — AutoBangumi: fully automated anime (追番) download and organisation tool.

# Download

- [qBittorrent](https://github.com/qbittorrent/qBittorrent) — The most popular open-source BitTorrent client for NAS use, with a full-featured built-in WebUI.
- [Transmission](https://transmissionbt.com/) — A fast, easy and free BitTorrent client for macOS, Windows and Linux.
- [aria2](https://github.com/aria2/aria2) — Lightweight multi-protocol command-line download utility (HTTP/HTTPS/FTP/BitTorrent/Metalink) with RPC control.
- [Prowlarr](https://github.com/Prowlarr/Prowlarr) — Indexer manager/proxy built on the popular \*arr .net/reactjs base stack, integrating seamlessly with Lidarr, Mylar3, Radarr, Readarr and Sonarr.
- [Jackett](https://github.com/Jackett/Jackett) — API support for your favorite torrent trackers; translates tracker queries into a common API for other apps.

# Productivity

- [Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF) — #1 locally hosted web application for performing various operations on PDF files.
- [SiYuan](https://github.com/siyuan-note/siyuan) — An open-source, privacy-first, self-hosted knowledge workspace; the easiest way to serve it is through Docker.
- [Joplin](https://github.com/laurent22/joplin) — The privacy-focused note taking app with sync capabilities for Windows, macOS, Linux, Android and iOS.
- [memos](https://github.com/usememos/memos) — A modern, open-source, self-hosted knowledge management and note-taking platform designed for privacy-conscious users.
- [logseq](https://github.com/logseq/logseq) — A privacy-first, open-source platform for knowledge management and collaboration.
- [AppFlowy](https://github.com/AppFlowy-IO/AppFlowy) — Bring projects, wikis, and teams together with AI. The leading open source Notion alternative.
- [personal-management-system](https://github.com/Volmarg/personal-management-system) — Your web application for managing personal data.
- [slash](https://github.com/yourselfhosted/slash) — An open source, self-hosted platform for sharing and managing your most frequently used links with human-readable shortcuts.
- [Apache Answer](https://github.com/apache/answer) — A Q&A platform software for teams at any scale: community forum, help center or knowledge management platform.
- [Outline](https://github.com/outline/outline) — The fastest knowledge base for growing teams; beautiful, realtime collaborative and feature packed.
- [Wiki.js](https://github.com/requarks/wiki) — Next generation open source wiki, backed by Git/PostgreSQL and rendered in Markdown or WYSIWYG.
- [Docmost](https://github.com/docmost/docmost) — Open-source collaborative wiki and documentation software, an open alternative to Confluence and Notion.
- [linkding](https://github.com/sissbruecker/linkding) — Self-hosted bookmark manager designed to be minimal, fast and easy to set up.
- [Linkwarden](https://github.com/linkwarden/linkwarden) — Self-hosted collaborative bookmark manager that collects, reads, annotates and fully preserves your links.
- [Karakeep](https://github.com/karakeep-app/karakeep) — A self-hostable bookmark-everything app (links, notes and images) with AI-based automatic tagging.

# Communication & Social

- [miniflux](https://github.com/miniflux/v2) — Minimalist and opinionated feed reader.
- [RSSHub](https://github.com/DIYgod/RSSHub) — 🧡 Everything is RSSible.
- [ntfy](https://github.com/binwiederhier/ntfy) — Send push notifications to your phone or desktop with a single HTTP PUT/POST; perfect for NAS job alerts.
- [Gotify](https://github.com/gotify/server) — A simple server for sending and receiving real-time messages over WebSocket.

# Education

- [calibre-web](https://github.com/janeczku/calibre-web) — 📚 Web app for browsing, reading and downloading eBooks stored in a Calibre database.
- [koodo-reader](https://github.com/koodo-reader/koodo-reader) — A modern ebook manager and reader with sync and backup capacities for Windows, macOS, Linux, Android, iOS and Web.
- [paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) — A community-supported supercharged document management system: scan, index and archive all your documents.
- [flat](https://github.com/netless-io/flat) — Project flat is the Web, Windows and macOS client of Agora Flat open source classroom.

# Entertainment

- [Sunshine](https://github.com/LizardByte/Sunshine) — Self-hosted game stream host for Moonlight; turn your NAS box / gaming PC into your own cloud gaming server.
- [Moonlight](https://github.com/moonlight-stream/moonlight-qt) — GameStream client for PCs (Windows, Mac, Linux, and Steam Link).
- [RomM](https://github.com/rommapp/romm) — A beautiful, powerful, self-hosted ROM manager and player for your game collection.

# Finance

- [Firefly III](https://github.com/firefly-iii/firefly-iii) — A personal finances manager with double-entry bookkeeping, budgeting and reporting.
- [Actual Budget](https://github.com/actualbudget/actual) — A local-first personal finance app built on an envelope budgeting method.
- [Ghostfolio](https://github.com/ghostfolio/ghostfolio) — Open source wealth management software for tracking portfolios and investments.

# Home Automation & Life

- [home-assistant](https://github.com/home-assistant/core) — 🏡 Open source home automation that puts local control and privacy first.
- [Frigate](https://github.com/blakeblackshear/frigate) — NVR with realtime local object detection for IP cameras; stores recordings on your NAS.
- [Mealie](https://github.com/mealie-recipes/mealie) — Self hosted recipe manager and meal planner with a REST API and reactive frontend.
- [grocy](https://github.com/grocy/grocy) — ERP beyond your fridge: web-based self-hosted groceries & household management solution.

# Network & Remote Access

- [Tailscale](https://github.com/tailscale/tailscale) — The easiest, most secure way to use WireGuard and 2FA; the standard way to reach your NAS from anywhere without opening ports.
- [Headscale](https://github.com/juanfont/headscale) — An open source, self-hosted implementation of the Tailscale control server.
- [NetBird](https://github.com/netbirdio/netbird) — Connect your devices, users and agents into a secure WireGuard-based overlay network with SSO.
- [frp](https://github.com/fatedier/frp) — A fast reverse proxy to help you expose a local server behind a NAT or firewall to the internet.
- [Caddy](https://github.com/caddyserver/caddy) — Fast and extensible multi-platform web server with automatic HTTPS; the simplest reverse proxy for self-hosted apps.
- [Traefik](https://github.com/traefik/traefik) — The cloud native application proxy with automatic service discovery from Docker labels.
- [Nginx Proxy Manager](https://github.com/NginxProxyManager/nginx-proxy-manager) — Docker container for managing Nginx proxy hosts with a simple, powerful interface and free SSL.
- [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) — Network-wide ads & trackers blocking DNS server.
- [Pi-hole](https://github.com/pi-hole/pi-hole) — A black hole for Internet advertisements: network-level DNS ad blocking.
- [Technitium DNS Server](https://github.com/TechnitiumSoftware/DnsServer) — Self-hosted DNS server with ad blocking, DNS-over-HTTPS/TLS and a web console.
- [rustdesk-server](https://github.com/rustdesk/rustdesk-server) — RustDesk Server Program: self-host the relay/signaling server for the open-source RustDesk remote desktop.

# Monitoring & Health

- [uptime-kuma](https://github.com/louislam/uptime-kuma) — A fancy self-hosted monitoring tool.
- [Checkmate](https://github.com/bluewave-labs/Checkmate) — An open-source, self-hosted tool that tracks and monitors server hardware, uptime, response times and incidents in real time.
- [Netdata](https://github.com/netdata/netdata) — The fastest path to full stack observability; per-second metrics with zero configuration.
- [Beszel](https://github.com/henrygd/beszel) — Lightweight server monitoring with historical data, docker stats and alerts.
- [Grafana](https://github.com/grafana/grafana) — The open and composable observability and data visualization platform.
- [Prometheus](https://github.com/prometheus/prometheus) — The Prometheus monitoring system and time series database.
- [scrutiny](https://github.com/AnalogJ/scrutiny) — Hard Drive S.M.A.R.T Monitoring, Historical Trends & Real World Failure Thresholds.
- [kener](https://github.com/rajnandan1/kener) — Stunning status pages, batteries included!

# Dashboards & Containers

- [homepage](https://github.com/gethomepage/homepage) — A highly customizable homepage (or startpage / application dashboard) with Docker and service API integrations.
- [Homarr](https://github.com/homarr-labs/homarr) — A modern and easy to use dashboard with 80+ integrations, 20K+ built-in icons and authentication out of the box.
- [Dashy](https://github.com/lissy93/dashy) — 🚀 A self-hostable personal dashboard built for you; includes status-checking, widgets and themes.
- [OliveTin](https://github.com/OliveTin/OliveTin) — Gives safe and simple access to predefined shell commands from a web interface.
- [portainer](https://github.com/portainer/portainer) — Making Docker and Kubernetes management easy.
- [Dockge](https://github.com/louislam/dockge) — A fancy, easy-to-use and reactive self-hosted docker compose.yaml stack manager.

# Security & Identity

- [vaultwarden](https://github.com/dani-garcia/vaultwarden) — Unofficial Bitwarden compatible server written in Rust, formerly known as bitwarden_rs.
- [authentik](https://github.com/goauthentik/authentik) — The authentication glue you need: self-hosted SSO and identity provider for all your apps.
- [Authelia](https://github.com/authelia/authelia) — The Single Sign-On Multi-Factor portal for web apps. OpenID Certified.
- [ZITADEL](https://github.com/zitadel/zitadel) — Identity infrastructure, simplified: self-hostable IAM with SSO, OIDC and SAML.

# Automation

- [n8n](https://github.com/n8n-io/n8n) — Fair-code workflow automation platform with native AI capabilities; combines visual building with code.
- [qinglong](https://github.com/whyour/qinglong) — Timed task management platform supporting Python3, JavaScript, Shell and TypeScript.

# AI

- [Ollama](https://github.com/ollama/ollama) — Get up and running with local LLMs on your own hardware.
- [Open WebUI](https://github.com/open-webui/open-webui) — User-friendly self-hosted AI interface (supports Ollama, OpenAI-compatible APIs and more).
- [LocalAI](https://github.com/mudler/LocalAI) — The open-source AI engine: run LLMs, vision, voice, image and video models on consumer hardware.
- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) — The most powerful and modular diffusion model GUI, API and backend with a graph/nodes interface.
- [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) — Full-stack local AI app: chat with your documents with RAG, agents and no data leaving your machine.
- [Soma](https://github.com/AwesomeDog/soma) — Local-first semantic search engine for your files: hybrid BM25 + vector + HyDE search over documents, PDFs, images, audio and video. Runs 100% offline as a single binary with CLI, web UI and HTTP API — a good fit for making a large NAS archive searchable in plain language.
- [faster-whisper](https://github.com/SYSTRAN/faster-whisper) — Faster Whisper speech-to-text transcription with CTranslate2; great for transcribing your media library.

# Dev & Coding

- [Gitea](https://github.com/go-gitea/gitea) — Git with a cup of tea! Painless self-hosted all-in-one software development service.
- [gogs](https://github.com/gogs/gogs) — Gogs is a painless self-hosted Git service; extremely lightweight.
- [code-server](https://github.com/coder/code-server) — VS Code in the browser; develop directly against your NAS from any device.
- [ToolJet](https://github.com/ToolJet/ToolJet) — Low-code platform for building business applications; connect to databases, cloud storages, GraphQL, API endpoints and more.
- [penpot](https://github.com/penpot/penpot) — Penpot: The open-source design tool for design and code collaboration.

# Useful articles

- [LinuxServer.io](https://www.linuxserver.io/) — Maintains a huge catalogue of well-built Docker images used by most NAS/homelab setups.
- [TRaSH Guides](https://trash-guides.info/) — Hard-mode guides for Sonarr, Radarr and the rest of the \*arr stack.
- [OpenZFS Documentation](https://openzfs.github.io/openzfs-docs/) — Admin and developer docs for OpenZFS on Linux and FreeBSD.
- [mergerfs docs](https://github.com/trapexit/mergerfs) — Full documentation for pooling drives of mixed sizes without RAID.

# Books

- [FreeBSD Mastery: ZFS](https://mwl.io/static/books/freebsd-mastery-zfs.html) — Michael W. Lucas. Data storage for the 21st century and beyond; the clearest ZFS book available.
- [FreeBSD Mastery: Advanced ZFS](https://mwl.io/static/books/freebsd-mastery-advanced-zfs.html) — Michael W. Lucas. Because your disks are plotting against you.
- [FreeBSD Mastery: Storage Essentials](https://mwl.io/static/books/freebsd-mastery-storage-essentials.html) — Michael W. Lucas. How to avoid making your host unusable at install time but not realize it for months.

# Videos

- [Techno Tim](https://www.youtube.com/@TechnoTim) — Homelab and self-hosted walkthroughs, including NAS and Docker setups.
- [Jeff Geerling](https://www.youtube.com/@JeffGeerling) — Raspberry Pi, NAS builds and storage/network benchmarking.
- [Level1Techs](https://www.youtube.com/@Level1Techs) — Deep dives on storage, ZFS, networking and server hardware.
- [ServeTheHome](https://www.youtube.com/@STH) — Hardware reviews and homelab/storage tutorials.
- [DB Tech](https://www.youtube.com/@DBTechYT) — Beginner-friendly Docker and self-hosted app tutorials.
- [Hardware Haven](https://www.youtube.com/@HardwareHaven) — Short, focused guides on self-hosting and homelab services.
