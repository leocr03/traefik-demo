# traefik-demo

Demo of stack for monitoring composed by:

* traefik
* prometheus
* grafana

## Requirements

* [docker-compose](https://docs.docker.com/compose/install/)

## How to run

### To load

```bash
docker-compose up
```

### To complete reload

```bash
docker-compose stop && docker-compose rm && docker-compose up -d --build
```

### To access Traefik

[http://localhost:8080](http://localhost:8080)

### To access Prometheus

[http://localhost:9090](http://localhost:9090)

### To access Grafana

[http://localhost:3000](http://localhost:3000)

|user|password|
|---|---|
|admin|admin|

### To access the sample application

* via traefik:

[http://localhost](http://localhost)

* directly (without traefik):

[http://localhost:5000](http://localhost:5000)

* force some 404 error:

[http://localhost/foo](http://localhost/foo)

## Grafana Configuration

### DataSource Config

![alt text](https://i.imgur.com/j4Vdseb.png)

### Dashboard Import

![alt text](https://i.imgur.com/xHxBLgx.png)