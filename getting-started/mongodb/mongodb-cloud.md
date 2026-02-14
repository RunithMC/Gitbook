---
icon: cloud
---

# MongoDB Cloud

## Step 1: Create an Account <a href="#step-1-create-an-account" id="step-1-create-an-account"></a>

**Visit MongoDB Cloud:**

1. **Open your web browser** and navigate to [MongoDB Cloud.](https://www.mongodb.com/products/platform/cloud)

**Sign Up:**

1. **Click on the Sign Up button**.
2. **Enter your email address and create a password**.
3. Alternatively, you can sign up using your **Google account**.

**Accept Privacy Policy & Terms:**

1. **Read through the Privacy Policy & Terms**.
2. **Check the box to accept them and proceed**.

**Answer "Getting to Know You" Questions:**

1. You will be presented with a few questions to help MongoDB understand your needs.
2. You can answer these questions randomly as they do not affect your setup.

***

## Step 2: Deploy Your Cluster <a href="#step-2-deploy-your-cluster" id="step-2-deploy-your-cluster"></a>

**Choose the Free Tier:**

1. After logging in, you will be directed to the **MongoDB Atlas dashboard**.
2. **Click on Build a Cluster**.
3. Select the **M0 (Free) tier option**.

**Cluster Configuration:**

**Name Your Cluster:**

1. You can leave the default name as **Cluster0** or choose a custom name.

**Cloud Provider & Region:**

1. Choose **AWS** as your cloud provider.
2. Select a region closest to you. (**Frankfurt** is recommended for European users).
3. Click **Create Cluster** to begin the deployment process.

***

## Step 3: Set Up a Database User <a href="#step-3-set-up-a-database-user" id="step-3-set-up-a-database-user"></a>

**Create a Database User:**

1. While your cluster is being created, you will need to set up a database user.
2. Go to the **Database Access tab**.
3. **Click on Add New Database User**.

**Set a Username & Password:**

1. Enter a username of your choice.
2. Create a strong password and make a note of it as you will need it later.
3. Click **Add User** to create the database user.

***

## Step 4: Choose a Connection Method <a href="#step-4-choose-a-connection-method" id="step-4-choose-a-connection-method"></a>

**Connect to Your Cluster:**

1. Once your cluster is created, go to the **Clusters view**.
2. **Click on the Connect button** for your cluster.

**Choose a Connection Method:**

1. Select **Connect Your Application**.

**Drivers:**

1. Select Drivers
2. Copy the connection string provided.

**Note:** Ensure the connection string starts with `mongodb+srv://`.

**Update Your Configuration File:**

1. Open your **core.yml** file
2. Paste the connection string into the file.
3. Replace `<password>` in the connection string with the password you noted down earlier.

I**mportant:** Make sure to remove **`< >`**

***

## Step 5: Configure Network Access <a href="#step-5-configure-network-access" id="step-5-configure-network-access"></a>

**Add IP Address:**

1. Navigate to the **Network Access tab**.
2. **Click on Add IP Address**.
3. Enter the IP address of the server where you will be hosting your bot or application.
4. If you want to allow access from anywhere, you can add `0.0.0.0/0`, but this is not recommended for security reasons.
5. Click **Confirm** to add the IP address.

***

## Common Issues and Troubleshooting <a href="#common-issues-and-troubleshooting" id="common-issues-and-troubleshooting"></a>

**Buffer Timeout**

**Whitelist IP Address:**

1. Ensure your server's IP is whitelisted under the **Network Access tab**.

**Correct Password:**

1. Verify that the password you are using in the connection string is correct.
2. If you have forgotten your password, you can reset it in the **Database Access tab**:
   * Go to **Database Access**.
   * Click **Edit** next to the user.
   * Enter a new password and save the changes.
