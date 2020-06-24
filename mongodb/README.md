# Mongodb Dashboard

Mongodb Dashboard Visualization uses  <img src="./images/logo_telegraf.png" width="60">  as an exporter

#### These Dashboards needs ```mongodb``` as Telegraf Input Plugins

### Configuration:

```toml
[[inputs.mongodb]]
  ## An array of URLs of the form:
  ##   "mongodb://" [user ":" pass "@"] host [ ":" port]
  ## For example:
  ##   mongodb://user:auth_key@10.10.3.30:27017,
  ##   mongodb://10.10.3.33:18832,
  servers = ["mongodb://127.0.0.1:27017"]

  ## When true, collect cluster status.
  ## Note that the query that counts jumbo chunks triggers a COLLSCAN, which
  ## may have an impact on performance.
  # gather_cluster_status = true

  ## When true, collect per database stats
  # gather_perdb_stats = false

  ## When true, collect per collection stats
  # gather_col_stats = false

  ## List of db where collections stats are collected
  ## If empty, all db are concerned
  # col_stats_dbs = ["local"]

  ## Optional TLS Config
  # tls_ca = "/etc/telegraf/ca.pem"
  # tls_cert = "/etc/telegraf/cert.pem"
  # tls_key = "/etc/telegraf/key.pem"
  ## Use TLS but skip chain & host verification
  # insecure_skip_verify = false
```

# Dashboards

#### Basic Sytem Info

![image1](./images/image1.png)

#### CPU & Operations count

![image2](./images/image2.png)

#### READ  | WRITE | DELETE Queries

![image2](./images/image3.png)

# Purpose of Each Panel using in Dashboard
