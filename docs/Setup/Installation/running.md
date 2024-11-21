# Running Freya

Once Freya is installed, you can start it using the Freya CLI. This guide provides instructions for running Freya and monitoring its status.

---

## Table of Contents
1. [Starting Freya](#starting-freya)
2. [Accessing the Dashboard](#accessing-the-dashboard)
3. [Viewing Logs](#viewing-logs)

---

## Starting Freya

To start Freya, use the following command in your terminal:

    freya run
This command will launch Freya in your terminal and begin executing the core processes.


## Troubleshooting the freya run Command
- If `freya run` doesn't work, try using:

        python -m freya run

- Ensure the installation step was completed successfully, and verify your Python environment.

---

## Accessing the Dashboard
> **Note:** The first time you access the dashboard, you will be prompted to create an account.

If you installed the optional Freya Dashboard, you can access it by navigating to the following URL in your browser:

    http://localhost:6672

The dashboard provides an interface to interact with Freya, monitor its performance, and manage configurations.

### If the Dashboard Is Not Installed
If you chose not to install the dashboard, you can still monitor Freya's logs to track its status

## Viewing Logs
To check Freya's logs, visit the same URL used for the dashboard:

    http://localhost:6672

Without the dashboard installed, this URL will serve a log interface that displays real-time updates and output from Freya.

Alternatively, you can view logs directly in your terminal where Freya is running.

--- 

Continue to the next section to learn how to configure Freya for your needs.

[Next: Configuring Freya](../Configuration/configuration.md)
