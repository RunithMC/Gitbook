---
description: >-
  This guide explains how to install MongoDB Community Edition on Ubuntu using
  the official MongoDB repository.
icon: server
---

# Own Machine

{% hint style="warning" %}
These steps work for Ubuntu 20.04, 22.04, and 24.04.
{% endhint %}

***

### Update Your System

```bash
sudo apt update && sudo apt upgrade -y
```

***

### Install Required Dependencies

```bash
sudo apt install -y gnupg curl
```

***

### Import MongoDB Public GPG Key

```bash
curl -fsSL https://pgp.mongodb.com/server-7.0.asc | sudo gpg -o /usr/share/keyrings/mongodb-server-7.0.gpg --dearmor
```

***

### Add the MongoDB Repository

#### Ubuntu 24.04 (Noble)

```bash
echo "deb [ arch=amd64 signed-by=/usr/share/keyrings/mongodb-server-7.0.gpg ] https://repo.mongodb.org/apt/ubuntu noble/mongodb-org/7.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
```

#### Ubuntu 22.04 (Jammy)

```bash
echo "deb [ arch=amd64 signed-by=/usr/share/keyrings/mongodb-server-7.0.gpg ] https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/7.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
```

#### Ubuntu 20.04 (Focal)

```bash
echo "deb [ arch=amd64 signed-by=/usr/share/keyrings/mongodb-server-7.0.gpg ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/7.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
```

***

### Update Package List

```bash
sudo apt update
```

***

### Install MongoDB

```bash
sudo apt install -y mongodb-org
```

This installs: - `mongod` (MongoDB server) - `mongosh` (MongoDB shell) - MongoDB tools

***

### Start MongoDB Service

```bash
sudo systemctl start mongod
sudo systemctl enable mongod
```

***

### Check Service Status

```bash
sudo systemctl status mongod
```

You should see:

```
Active: active (running)
```

***

### Test MongoDB

```bash
mongosh
```

Inside the shell:

```javascript
db.version()
```

Exit:

```javascript
exit
```

***

## Optional: Enable Authentication (Recommended for Production)

1. Edit the config file:

```bash
sudo nano /etc/mongod.conf
```

2. Add:

```yaml
security:
  authorization: enabled
```

3. Restart MongoDB:

```bash
sudo systemctl restart mongod
```

4. Create an admin user:

```javascript
use admin

db.createUser({
  user: "admin",
  pwd: "StrongPasswordHere",
  roles: [ { role: "root", db: "admin" } ]
})
```

***

## Optional: Allow Remote Connections

1. Edit config file:

```bash
sudo nano /etc/mongod.conf
```

2. Change:

```yaml
bindIp: 127.0.0.1
```

To:

```yaml
bindIp: 0.0.0.0
```

3. Restart MongoDB:

```bash
sudo systemctl restart mongod
```

4. Open firewall (if using UFW):

```bash
sudo ufw allow 27017
```

{% hint style="warning" %}
Only do this if your server is properly secured.
{% endhint %}

***

MongoDB should now be installed and running successfully on your Ubuntu server.
