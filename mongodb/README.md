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
```

# Dashboards

#### Basic Sytem Info

![image1](./images/image1.png)

#### CPU & Operations count

![image2](./images/image2.png)

#### READ  | WRITE | DELETE Queries

![image2](./images/image3.png)

# Purpose of Each Panel using in Dashboard
