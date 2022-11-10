# Grafana Dashboards
[![Opstree Solutions][opstree_avatar]][opstree_homepage]<br/>[Opstree Solutions][opstree_homepage] 

  [opstree_homepage]: https://opstree.github.io/
  [opstree_avatar]: https://img.cloudposse.com/150x150/https://github.com/opstree.png

This repostiorty contains Grafana Dashboards to visualize your metrics stored in Prometheus.

# Supported Agent
- Telegraf
- Promtheus Exporters

# Dashboards
Currently Following are the set of Grafana Dashboards we have uploaded to Grafana labs. you can find a detailed description of each dashboard on Grafana Page in below links. 

**Telegraf Agent Dashboards**
- [Node Dashboard](https://grafana.com/grafana/dashboards/12484-system-informationn/)
- [Apache2 Dashboard](https://grafana.com/grafana/dashboards/15389-apache2/)
- [Nginx Dashboard](https://grafana.com/grafana/dashboards/14900-nginx/)
- [Redis Dashboard](https://grafana.com/grafana/dashboards/12497-redis-server/)
- [Cassandra Dashboard](https://grafana.com/grafana/dashboards/12493-cassandra/)
- [Zookeeper Dashboard](./zookeeper)
- [Kafka Cluster Dashboard](https://grafana.com/grafana/dashboards/14505-kafka-cluster-metrics/)
- [Kafka Topic Metrics](https://grafana.com/grafana/dashboards/14506-kafka-topics-metrics/)
- [Mongodb Dashboard](https://grafana.com/grafana/dashboards/12556-mongo-db/)

**Prometheus Exporter Dashbaords**
- [Elasticsearch Dashboard](https://grafana.com/grafana/dashboards/16532-opstree-elasticsearch-dashboard/)
- [Mongodb Dashboard](https://grafana.com/grafana/dashboards/16490-opstree-mongodb-dashboard/)
- [Nginx Dashboard](https://grafana.com/grafana/dashboards/16813-nginx/)
- [Node Exporter Dashboard](https://grafana.com/grafana/dashboards/15780-opstree-node-exporter-a/)
- [Postgresql Dashboard](https://grafana.com/grafana/dashboards/16806-postgresql-dashboard/)
- [Rabbitmq Dashboard](https://grafana.com/grafana/dashboards/16063-opstree-rabbitmq-dashboard/)
- [Redis Dashboard](https://grafana.com/grafana/dashboards/16056-redis-dashboard-opstree/)

**Azure Dashboards**
- [Azure PostgreSQL Flexi](https://grafana.com/grafana/dashboards/16057-azure-postgresql-flexi-opstree/)

**Kubernetes Dashboards**
- [Kubernetes Ingress Controller Dashboard](https://grafana.com/grafana/dashboards/12575-kubernetes-ingress-controller-dashboard/)

# Setup Instructions of Grafana Dashboards
**Add datasource in Grafana**
- In Above Dashboards we are using Promehteus Datasource to visualize all the metrics, so we are going to select Promtheus Datasource in Grafana.
- Add Prometheus and fill out the url, authentication, scrape interval and name of the data source. Press save and test. It should show Data source is working if Grafana successfully connects to Prometheus.

# Create Dashboards
A Dashboard is a group of widgets but it also provides a lot more feature like folders, variables, time ranges and auto refresh. Follow below mention steps to import our Dashboards.
- Go to the plus icon on the left side of the homepage and click on import dashboards.
- Copy the json of above mentioned dashboards and past it in import via panel json box, then click on Load.