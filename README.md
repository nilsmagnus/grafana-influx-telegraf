# Monitoring with grafana + influxdb + telegraf 

A starting point for using grafana, influxdb and telegraf for monitoring.

* preconfigured datasource(influxdb) for grafana
* preconfigured dashboard(id 1443) as a start

# Prerequesites

docker 
docker-compose

# Run

    docker-compose up
    
    
* go to [http://localhost:3000](http://localhost:3000) , log in with admin/admin

* the pre-configured dashboard is located at [http://localhost:3000/dashboard/file/telegraf-host-metrics.json](http://localhost:3000/dashboard/file/telegraf-host-metrics.json?refresh=1m&orgId=1)


# Configure it

* add new datasources with the template in grafana/grafana-datasource.yaml
* edit telegraf.conf with the targets you want to monitor
* add new dashboards(as json files) in grafana/dashboards