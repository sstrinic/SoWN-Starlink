# SoWN-starlink

Security of Wireless Networks course repository

## Current Goals

- Setup Raspberry pi :white_check_mark:
- Finish Docker-compose
- Setup Grafana
- Setup Prometheus
- Setup Starlink exporter
- Research SpaceX API v4
- Wireshark packet analysis
- Traceroute

## Setup

```bash
# Start all services:
docker-compose up -d

# In case of RHEL based linux distro you can use command:
sudo chcon -Rt svirt_sandbox_file_t dirname
```
