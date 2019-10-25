# TiDB docker-compose

## Requirements

* Docker >= 17.03
* Docker Compose >= 1.6.0

> **Note:** [Legacy Docker Toolbox](https://docs.docker.com/toolbox/toolbox_install_mac/) users must migrate to [Docker for Mac](https://store.docker.com/editions/community/docker-ce-desktop-mac), since it is tested that tidb-docker-compose cannot be started on Docker Toolbox and Docker Machine.

## Quick start

```bash
$ git clone https://github.com/pingcap/tidb-docker-compose.git
$ cd tidb-docker-compose && docker-compose pull # Get the latest Docker images
$ docker-compose up -d
$ mysql -h 127.0.0.1 -P 4000 -u root
```

* Access monitor at http://localhost:3000 (login with admin/admin if you want to modify grafana)

* Access [tidb-vision](https://github.com/pingcap/tidb-vision) at http://localhost:8010

* Access Spark Web UI at http://localhost:8080
  and access [TiSpark](https://github.com/pingcap/tispark) through spark://127.0.0.1:7077
