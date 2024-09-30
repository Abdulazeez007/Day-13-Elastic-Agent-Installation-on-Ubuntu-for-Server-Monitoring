# Day-13-Elastic-Agent-Installation-on-Ubuntu-for-Server-Monitoring

Are you interested in monitoring your Linux server’s performance and security? In this guide, we’ll go through the steps to install an Elastic Agent on your Ubuntu Server. This will enable you to collect and manage logs effectively. Let’s get started!

## Why Elastic Agent?
Before we begin, you might wonder why you should bother with Elastic Agent. Here are a few compelling reasons:

- **Centralized Logging:** Collect and analyze logs from multiple sources in one place.
- **Real-time Monitoring:** Get instant visibility into your server’s health and performance.
- **Security Insights:** Detect and investigate potential security threats quickly.
- **Scalability:** Easily expand your monitoring as your infrastructure grows.

Now that we’re convinced, let’s get our hands dirty!

## Step 1: Preparing Your Elastic Environment
First, we’ll set up our Elastic environment:

1. Log into your Elastic web GUI.
2. Click the hamburger icon (☰) in the top-left corner.
3. Scroll down to the “Management” section and select “Fleet”.

## Step 2: Creating an Agent Policy
Now, let’s create a policy for our Ubuntu Server:

1. In Fleet, click on “Agent policies”.
2. Select “Create agent policy”.
3. Give your policy a name (e.g., “Ubuntu-Server-Policy”).
4. Click “Create agent policy”.

## Step 3: Generating the Installation Command
With our policy in place, we can generate the installation command:

1. Back in Fleet, click “Add agent”.
2. Scroll down to find the Linux installation code.
3. Copy this code to your clipboard.

## Step 4: Installing the Agent on Your Ubuntu Server
Time to put that code to work:

1. SSH into your Ubuntu Server.
2. Paste the installation command you copied earlier.
3. Press Enter and watch the magic happen!

The Elastic Agent will now install and configure itself based on your policy.

![Alt text](https://raw.githubusercontent.com/Virus192/Day-13-Elastic-Agent-Installation-on-Ubuntu-for-Server-Monitoring/refs/heads/main/images/photo_5989808863731369924_w.jpg)

## Step 5: Verifying the Installation
Let’s make sure everything is working as expected:

1. Return to your Elastic web GUI.
2. Click the hamburger icon (☰) and select “Discover”.
3. On the left side, look for “agent.name”.
4. You should see your newly created policy (e.g., “Ubuntu-Server-Policy”).
5. Click on it to view the incoming logs.

![Alt text](https://raw.githubusercontent.com/Virus192/Day-13-Elastic-Agent-Installation-on-Ubuntu-for-Server-Monitoring/refs/heads/main/images/photo_5989808863731369922_w.jpg)
![Alt text](https://raw.githubusercontent.com/Virus192/Day-13-Elastic-Agent-Installation-on-Ubuntu-for-Server-Monitoring/refs/heads/main/images/photo_5989808863731369926_w.jpg)

Congratulations! You’ve successfully installed an Elastic Agent on your Ubuntu Server! 🎉 You now have a powerful tool at your fingertips for monitoring your server’s performance, tracking system events, and keeping an eye on potential security issues.

## Conclusion
In our next blog, we will delve into creating alerts specifically for brute force activity. Additionally, we’ll develop a dashboard to visualize the origins of these attacks, enhancing your server’s security and monitoring capabilities. Stay tuned for more insights!
