# gpu-monitoring-container

[Docker Compose](https://docs.docker.com/compose/) file to set up NVIDIA GPU monitoring on a single server using [DCGM-Exporter](https://github.com/NVIDIA/dcgm-exporter), [Prometheus](https://github.com/prometheus/prometheus), and [Grafana](https://github.com/grafana/grafana).

## Prerequisites

1. [NVIDIA Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html)
2. [Docker Compose](https://docs.docker.com/compose/install/). Please make sure your docker-compose supports Compose file format [version 3.x](https://docs.docker.com/compose/compose-file/compose-versioning/).

## Set Up

Run the following command to launch containers:

```bash
make docker-up
```

Then you can access http://localhost:19300 for Grafana Dashboard (default username: _admin_, password: _admin_).
