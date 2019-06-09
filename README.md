# docker-monitoring-sandbox
Monitor your server with the TICK Stack from Influx

## TICK Stack
Collectively, Telegraf, InfluxDB, Chronograf and Kapacitor are known as the TICK Stack.

> The TICK Stack is a loosely coupled yet tightly integrated set of open source projects designed to handle massive amounts of time-stamped information to support your metrics analysis needs.

### Telegraf
[Telegraf](https://influxdata.com/time-series-platform/telegraf/) is a plugin-driven server agent for collecting and reporting metrics.

### InfluxDB
[InfluxDB](https://www.influxdata.com/products/influxdb-overview/) is a time series database built from the ground up to handle high write and query loads. Is a custom high-performance datastore written specifically for time-stamped data, and especially helpful for use cases such as DevOps monitoring, IoT monitoring, and real-time analytics.

### Chronograf
[Chronograf](https://www.influxdata.com/time-series-platform/chronograf/) is the administrative user interface and visualization engine of the stack. Setup and maintain the monitoring and alerting for your infrastructure.

### Kapacitor
[Kapacitor]() is a native data processing engine. It can process both stream and batch data from InfluxDB. Kapacitor lets you plug in your own custom logic or user-defined functions to process alerts with dynamic thresholds, match metrics for patterns, compute statistical anomalies, and perform specific actions based on these alerts, like dynamic load rebalancing. 

## Setup

*Work in progress*
- Configure Docker Monitoring
- Configure NGINX Monitoring
- Configure Google OAuth Login

## Usage

Just `docker-compose up -d` and the full stack will be running in `YOUR_IP:8888`.

## Results

### Docker monitor
![Dashboard showing Docker information](docs/tick_docker.png)

### Nginx monitor
![Dashboard showing Nginx information](docs/tick_nginx.png)

### Logs monitor
![Dashboard showing logs information](docs/tick_logs.png)

## References
[InfluxData / TICK-docker](https://github.com/influxdata/TICK-docker)
