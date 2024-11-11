# SoWN-Starlink

![GitHub License](https://img.shields.io/github/license/sstrinic/SoWN-starlink)
![GitHub Repo Size](https://img.shields.io/github/repo-size/sstrinic/SoWN-starlink)
![GitHub Contributors](https://img.shields.io/github/contributors/sstrinic/SoWN-starlink)

This repository is part of the **Security of Wireless Networks** course and focuses on the **Starlink** satellite network.  
The project aims to analyze Starlink's performance and network behavior through comprehensive dashboards and data visualization tools, leveraging various monitoring and analysis tools.

## Project Overview

The goal of this project is to set up a robust analysis and monitoring environment for Starlink.  
By combining tools like Grafana, Prometheus, and custom Starlink exporters, the project provides insights into Starlink's network traffic, latency, stability, and security.

### Features

- **Real-time Starlink Data Dashboards**: Visualize key metrics of Starlink's network performance.
- **Automated Monitoring Setup**: Easily deploy Grafana, Prometheus and Portainer using Docker compose.
- **Network Traffic Analysis**: Capture and analyze packet data using Wireshark.
- **SpaceX API Integration**: Research and possibly integrate SpaceX's API (v4) for additional telemetry.

## Project Goals

- **Raspberry Pi Setup** ✅
- **Grafana and Prometheus Integration** ✅
- **Starlink Exporter Setup** ✅
- **Docker Compose Configuration**
- **SpaceX API (v4) integration**
- **Grafana dashboards**
- **Wireshark Packet Analysis**
- **Traceroute for Latency and Route Insights**

## Getting Started

To get started with this project, ensure that Docker and Docker Compose are installed on your system.  
This setup will initialize the required services, allowing you to monitor and analyze Starlink data.

### Prerequisites

- **Docker** and **Docker Compose**
- A **Raspberry Pi** (for certain parts of the project)
- Basic knowledge of networking tools like **Wireshark** and **Traceroute**

### Installation

Clone the repository:

```bash
git clone https://github.com/sstrinic/SoWN-starlink.git
cd SoWN-starlink
```

### Setup

1. **Start all services**: Run the following command to start Grafana, Prometheus, and other services.

   ```bash
   docker-compose up -d
   ```

2. **SELinux enabled distros like RHEL-based distros**: If you are using SELinux, use this command to ensure proper Docker permissions.

   ```bash
   sudo chcon -Rt svirt_sandbox_file_t <directory_name>
   ```

### Accessing the Dashboards

Once the services are up, you can access Grafana at `http://localhost:3000`.  
Here, you’ll be able to monitor Starlink data through various pre-configured dashboards.

## Usage

- **Grafana**: Visualize real-time network performance, latency, and other metrics for Starlink.
- **Wireshark**: Capture and analyze Starlink packet data to examine security and performance.
- **Traceroute**: Measure the latency and route of packets through the Starlink network.
- **Integration with SpaceX API**: Potential integration with SpaceX API for real-time satellite data.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
