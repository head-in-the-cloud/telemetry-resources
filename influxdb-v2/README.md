Written by: D. Zwart

## InfluxDB v2

A timeseries database nice for pushing time based data points of any type or shape.
With the limited time retention, you are in full control of automatic data purging to keep your storage limited in size.

The end-goal of Influx looks similar to Prometheus, but it is inherently different in it's setup.
Where Prometheus binds an incoming/outgoing port (therefore affecting your network deployment setup), influx is a only client with outgoing port. The data is barely aggregated.
Prometheus is more robust against internet connectivity issues, but I hope that's not a scenario we find eachother in often. 

### Setting it up

Start it with:
> `docker-compose up -d`

And then access it at:
> http://localhost:8086

### Nice to know

1) The user interface of InfluxDB is mighty and capable. It comes with data exploration and data loading plugins from all existing languages, frameworks etc.
2) InfluxDb v1 is not compatible to InfluxDb v2 due to the query language Flux being completely incompatible.