# Docker Monitor

[![Latest Version](https://img.shields.io/github/v/release/kiwfy/docker-monitor.svg?style=flat-square)](https://github.com/kiwfy/docker-monitor/releases)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

Project to monitor all running docker containers and all main resources from a machine using grafana and prometheus

### Run

Requires [Docker](https://www.docker.com/get-started) and [Docker Compose](https://docs.docker.com/compose/install/) tool.

```sh
docker-compose up -d
```

### Grafana

[Grafana](https://grafana.com/) is expose on port `3000` and you can access your dashboards [here](http://localhost:3000/)

The default user and password to login in Grafana are: User `admin` and Password `admin`

### Prometheus

[Prometheus](https://prometheus.io/) is expose on port `9090` and you can access all metrics [here](http://localhost:9090/)

### Agents

The agents used for this project are [Node Exporter](https://github.com/prometheus/node_exporter) and [cAdvisor](https://github.com/google/cadvisor). 

### Grafana Config

For config in Grafana like allow embedding graph or other config you can access and update [grafana.ini](https://github.com/kiwfy/docker-monitor/blob/master/grafana/grafana.ini).

You can change the default dashboard configurations in [docker.json](https://github.com/kiwfy/docker-monitor/blob/master/grafana/dashboards/docker.json).

For update or add another datasource type you can use [datasource.yaml](https://github.com/kiwfy/docker-monitor/blob/master/grafana/provisioning/datasources/datasource.yaml)

**For new dashboards you can just create another json in [dashboard](https://github.com/kiwfy/docker-monitor/tree/master/grafana/dashboards) folder**


### Development

Want to contribute? Great!

**Kiwfy - Open your code, open your mind!**