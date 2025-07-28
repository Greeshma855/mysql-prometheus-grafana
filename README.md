# Monitor MySQL With Prometheus and Grafana


## Requirements
* Install Docker

## Not Essential 
* Install GNU Make (Not essential)

## Use the following command to run
* Run `docker compose up -d` (If you installed makefile you can use `make up`)


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


