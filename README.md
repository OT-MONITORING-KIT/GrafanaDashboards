# Grafana Dashboards
[![Opstree Solutions][opstree_avatar]][opstree_homepage]<br/>[Opstree Solutions][opstree_homepage] 

  [opstree_homepage]: https://opstree.github.io/
  [opstree_avatar]: https://img.cloudposse.com/150x150/https://github.com/opstree.png

This repostiorty contains Grafana Dashboards to visualize your metrics stored in Prometheus datasource.

# Supported Agent
- Telegraf

# Prerequisite
- Telegraf Agent on Each Node.
- Promtheus as Data Source to Store metrics.

# Dashboards
Currently Following are the set of Grafana Dashboards.
- Node Dashboard
- Redis Dashboard
- Cassandra Dashboard
- Zookeeper Dashboard
- Kafka Dashboard
- Mongodb Dashboard

# Setup Instructions of Grafana Dashboards
**Add datasource in Grafana**
- In Above Dashboards we are using Promehteus Datasource to visualize all the metrics, so we are going to select Promtheus Datasource in Grafana.\
- Add Prometheus and fill out the url, authentication, scrape interval and name of the data source. Press save and test. It should show Data source is working if Grafana successfully connects to Prometheus.

# Create Dashboards
A Dashboard is a group of widgets but it also provides a lot more feature like folders, variables, time ranges and auto refresh. Follow below mention steps to import our Dashboards.
- Go to the plus icon on the left side of the homepage and create click on import dashboards.
- Copy the json of above mentioned dashboards and past it in import via panel json box, then click on Load.