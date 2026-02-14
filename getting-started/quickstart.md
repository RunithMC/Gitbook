---
description: Free library for Runith plugins.
icon: bolt
metaLinks:
  alternates:
    - https://app.gitbook.com/s/yE16Xb3IemPxJWydtPOj/getting-started/quickstart
---

# Quickstart

### RunithCore

All runith plugins depend on this core to function.

{% hint style="success" %}
Download it [here](https://github.com/RunithMC/maven/releases/tag/core)!
{% endhint %}

{% code title="Default Configuration" overflow="wrap" expandable="true" %}
```yml
# Available: mongodb, gson and none
# none database always return null and don't save data
type: "gson"
context-prefix: "" # Use: prison, lobby, survival-og for separate data in the same database

redis:
  enable: false # Independent from mongodb and Gson
  uri: "redis://user:test@localhost:6379/0"

mongodb:
  uri-enable: false
  uri: "mongodb+srv://test:test@test.rsojstp.mongodb.net/?retryWrites=true&w=majority&appName=Test"

  user: "admin"
  password: "password"
  host: "localhost"
  port: 27017

  connect-timeout-seconds: 3
  read-timeout-seconds: 2

gson:
  path: "plugins/RunithCore/Gson-Database"
```
{% endcode %}

We recommend using **MongoDB** for servers with a large number of users (+30), **GSON** for testing or few users, and **none** for testing (no data will be saved).
