# HOMELAB

## Informations:  
This contains some informations about my homelab, used technologies, hardware informations, apps used etc..
Hope it will help you to build or improve your own homelab

## Technologies

| Name | Version | Role |
|------------|--------------|---------|
| Proxmox VE | 7.2-3 | Hypersivor |
| Proxmox Backup Server | 2.3-1 | Backup Hypersor |
| OpenMediaVault | 6.3.3| Nas |
| Docker | 20.10.21 | Container Solution |
| PfSense | 2.6.0 | Friewall / Router |
| Porainer | 2.14.0 |Container Orchestrator |

## Hardware

| Name | Role | CPU | RAM | STORAGE | GPU |
|------------|--------------|---------|--------|---------|-------|
| ODIN | Hypersivor | Ryzen 5 5600x | 4 x 16GB DDR4 | 2x 256go SSD + 2 x 1To SSD| P400
| LOKI| Management | j5040 | 2 x 4GB DDR4 | 2x 128Go SSD | 
| NJORD | NAS | G6400 | 2x 4 GB DDR4 | 2 x 128 Go SSD + 4 x 4To HDD |
| FREYJA | NAS | G6400 | 2x 4GB DDR4 | 2 x 128 Go SSD + 8 x 4To HDD |
| FRIGG | NAS| G6400 | 2 x 8GB DDR4 | 2 x 2To SSD + 2 x 128 Go SSD + 6 x 2To HDD |
| TYR | Proxmox Backup Server | j5040 | 2 x 4GB DDR4 | 2 x 2To SSD + 2 x 128 Go SSD |
| SKADI | NAS + DNS/CACHE | G1610T | 2 x 4GB DDR4 | 3 x 2 To HDD+ 1 x 128Go SSD |
| BALDR | Firewall | j4125 | 2x 4GB DDR4 | 1 x 128Go SSD |

Rack: Startech 42U X 1 | Digitus 10'' 6U x 3
Server Case : UK 4129 x 3 | UK 2129 x 2 | UK 1029 x1 | Hp Micro Gen8
Switch(s):  HP 1920-48G X 1 | HP 1810-8G x 3
Inverter: v7 UPS1RM2U3000
AP-Wifi: Zyxel AX1800

## Virtualized Servers

| Name | Role | CPU | RAM | 
|------------|--------------|---------|--------|
| THOR | APPs | 4 | 16 GB
| FREY | Monitoring / Log APPs | 2 | 8 GB
| HEIMDALL | DMZ Apps | 1 | 2 GB
| HEL | Media APP | 4 | 8 GB

## Applications (Container)
| Name | Attach Server  | Roles |
|------------|-------|-------------|
| Cadvisor | all | Metrics exporter | 
| Prometheus | FREY | Metrics aggregator | 
| Grafana | FREY| Visualize Metrics | 
| Loki | FREY | log aggregation/ visualize| 
| rsyslog | FREY | log server | 
| promtail | FREY | log discovery | 
| Influxdb | FREY | metrics receiver(my usage) | 
| Node-exporter | all | Metrics exporter| 
| Pyload-ng | HEL | Download Manager | 
| Jellyfin | HEL | Videos media center| 
| JellySeer | HEL| request manager | 
| Sonarr | HEL | Tv shows automation | 
| Radarr | HEL | Movies automation | 
| Readarr | HEL | Books automation | 
| Prowlarr | HEL | Indexers | 
| Ubooquiti | HEL | comics store/lector | 
| Librephotos | HEL | photos store | 
| Deluge | HEL | bittorrent client | 
| Jackett | HEL | torrent proxy serevr | 
| Swag | HEIMDALL | http/https reverse proxy | 
| frp | HEIMDALL | tcp / udp reverse proxy | 
| Vaultwarden | THOR | password manager| 
| Pingvin-Share | THOR | sharing plateform| 
| Snipe-IT | THOR | asset management| 
| Librespeed | THOR | networkspeed tester | 
| Wikijs | THOR | wiki | 
| Heimdall | THOR | app dashboard | 
| Netbox | THOR | IPAM and DCIM | 
| Grocy | THOR | cooking erp | 
| Duplicati | THOR | backup container volumes  | 
| ntp | LOKI | time server | 
| postfix-relay | LOKI | relay smtp | 
| kms | LOKI | licence activation server | 
| nginx-proxy-manager | LOKI | http/https reverse proxy | 
| gitea | LOKI | git | 
| pihole | LOKI | Dns | 
| librenms | LOKI | Supervision | 
| ansible-semaphore | LOKI | ansible UI |
| lancache | SKADI | dns/cache server(games) |

