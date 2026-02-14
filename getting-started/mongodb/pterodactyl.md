---
description: >-
  This guide explains how to install MongoDB Community Edition on Pterodactyl
  panel
icon: butterfly
---

# Pterodactyl

***

### 1) Download MongoDB Egg

[https://eggs.pterodactyl.io/egg/applications-mongodb-8/](https://eggs.pterodactyl.io/egg/applications-mongodb-8/)

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

***

### 2) Go to Nests

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

### 3) Create a New Nest

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### 4) Back and click in "import Egg" button

**4.1)** In associated Nest select "Database"

**4.2)** Click on import

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### 5) Create the server using MongoDB Egg

Set the password and username. Do not change them after installation, otherwise the MongoDB server will not start.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

### 6) Recommended: Create a user called "runithCore" with admin perms

**6.1)** Switch to the `admin` database\
The user's authentication database is the database where the user is created. For an administrator with wide-ranging privileges, you should create them in the `admin` database.bash

```bash
use admin
```

**6.2)** Create the user\
Use the `db.createUser()` method. The `root` role, when defined in the `admin` database, grants superuser privileges across the entire MongoDB instance.javascript

```json
db.createUser(
  {
    user: "runithCore",
    pwd: "testPassword", // Use https://www.lastpass.com/es//features/password-generator
    roles: [
      { role: "root", db: "admin" }
    ]
  }
)
```

