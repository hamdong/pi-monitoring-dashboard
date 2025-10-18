# 🖥️ Raspberry Pi Monitoring Dashboard

A lightweight, local-only dashboard to monitor your Raspberry Pi and Docker containers. No accounts, no cloud — just Prometheus, Grafana, and a couple exporters.

## 🔧 What’s Included

| Tool          | Purpose                          |
| ------------- | -------------------------------- |
| Grafana       | Dashboard UI                     |
| Prometheus    | Metrics collection engine        |
| node_exporter | Pi system stats (CPU, RAM, temp) |
| cAdvisor      | Docker container stats           |

## 🚀 Quick Start

### 1. Clone this repo

```bash
git clone https://github.com/hamdong/pi-monitoring-dashboard.git
cd pi-monitoring-dashboard
```

### 2. Start everything

```bash
docker-compose up -d
```

### 3. Open the dashboard

1. Go to `http://<your-pi-ip>:3000`
1. Login: `admin` / `your-password-here` → change password
1. Dashboard is preloaded under **"Dashboards > Browse"**

## 📊 Metrics Covered

- Pi CPU, RAM, disk, and temp
- Docker container CPU %, memory, network
- System load average

## ⚙️ Ports

| Service       | Port |
| ------------- | ---- |
| Grafana       | 3000 |
| Prometheus    | 9090 |
| cAdvisor      | 8080 |
| node_exporter | 9100 |

## 🛑 Stop Everything

```bash
docker-compose down
```

## 💡 Notes

- No Grafana account required
- All data stays local
- Portable setup — just clone this repo on a new system

## 📄 License

MIT — free to use and modify.
