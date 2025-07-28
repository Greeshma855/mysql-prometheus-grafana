# Monitor MySQL With Prometheus and Grafana


## Requirements
* Install Docker

## Not Essential 
* Install GNU Make (Not essential)

## Use the following command to run
* Run `docker compose up -d` (If you installed makefile you can use `make up`)
* PROMETHEUS -- Check http://localhost:9090/targets (1/1 up -green signal must be there)
* Grafana -- Home -> Connections -> Data sources -> Add datasource (http://prometheus:9090) -> save+test (Shall get a successful message)
* Grafana -- dashboards -> import -> 7362+load -> select Prometheus data source that we set -> can see all metrics.
* Run ` docker exec -it mysql mysql -u root -p` to get mysql environment & type your password
* Run your queries
* Run `exit` to exit Mysql
* Run `docker-compose down` to close Docker


## You'll be able to monitor  
* CRUD operations on database
* Locks & Dead Locks
* Connections
* CPU Usage
* Load Average
* Memory Usage
* Shared Buffers
* Current Fetched Data
* Database Cache
* Parallel Workers
* Transactions
* Sessions
* and so much more...
  

## Ports
The containers and their exposed ports are:

-   **MySQL** - `:3306`
-   **prometheus** - `:9090`
-   **grafana** - `:3000`
-   **mysql-exporter** - `:9104`


