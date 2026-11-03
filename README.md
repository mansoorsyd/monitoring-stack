# Monitoring Stack

Prometheus + Node Exporter + Grafana, started with one command.

## Components
- **Prometheus:** collects and stores metrics
- **Node Exporter:** exposes server metrics (CPU, memory, disk)
- **Grafana:** dashboards and visualisation

## How to use
    docker compose up -d

- Grafana: http://localhost:3000
- Prometheus: http://localhost:9090

In Grafana: add Prometheus as a data source (URL `http://prometheus:9090`), then import dashboard ID **1860**.

Change the default Grafana password in `docker-compose.yml` before using this anywhere beyond your own computer.

## What I learned
- How metrics collection works
- Running multi-container setups with Docker Compose
