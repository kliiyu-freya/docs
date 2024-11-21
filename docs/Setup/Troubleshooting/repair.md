# Troubleshooting Freya

This guide helps you resolve common issues when using Freya. Follow these steps to diagnose and fix problems.

---

## Table of Contents
1. [General Troubleshooting Steps](#general-troubleshooting-steps)
2. [Common Issues and Solutions](#common-issues-and-solutions)
3. [Viewing Logs for More Information](#viewing-logs-for-more-information)
4. [Getting Support](#getting-support)

---

## General Troubleshooting Steps

1. **Check if Freya is Running**
    Ensure Freya is active by running:

        freya status

    If it’s not running, start it using:

        freya run

2. **Restart Freya**
    Sometimes, a simple restart resolves issues:

        freya restart

3. **Verify Installation**
    If commands like `freya run` don't work, confirm Freya is installed correctly:

        freya -v

4. **Ensure Dependencies Are Installed**
    - Confirm that Docker is installed and running.
    - Check that the required version of python is installed

        python --version

--- 

## Common Issues and Solutions

1. **Cannot Access Dashboard**
    - **Problem**: The dashboard isn't accessible at http://localhost:6672.
    - **Solution**:
        - Verify that Freya is Runnin:

            freya run

        - Check if the dashboard was installed:

            freya --list packages

        If missing, install it:

            freya --install dashboard:latest

2. **Freya Commands Not Recognized**
    - **Problem**: CLI commands like `freya run` return an error.
    - **Solution**:
        - Try running with `python -m`:

            python -m freya run
        
        - Ensure Freya CLI is installed:

            pip install freya-cli

3. **Freya Fails to Start**
    - **Problem**: Freya crashes or doesn't start.
    - **Solution**:
        - Check the logs for detailed error messages (see the [Viewing Logs](#viewing-logs-for-more-information) section).
        - Try restrating Freya:

            freya restart

4. **Configuration Changes Not Taking Effect**
    - **Problem**: Updates made in the dashboard don’t seem to apply.
    - **Solution**:
        - Ensure you clicked **Save** or **Apply Changes**.
        - Restart Freya after making configuration updates:

            freya restart

5. **Network or Connection Issues**
    - **Problem**: Freya can't connect to external services or devices.
    - **Solution**:
        - Check your network settings in the dashboard or configuration files.
        - Verify your internet connection.

--- 

## Viewing Logs for More Information

Logs are essential for diagnosing issues. To view Freya’s logs:

1. **Using the Dashboard**: If installed, visit the log interface at:

        http://localhost:6672

2. **Using the Terminal** Run:

        freya logs

    Alternatively, check docker desktop for logs

---

## Getting Support
If the above steps don’t resolve your issue:

1. Search the Documentation Refer to the official documentation or FAQ for solutions.

2. Community Support Post your issue on Freya’s community forum or GitHub Discussions.

3. Report a Bug Open an issue on Freya’s GitHub repository. Include:
    - A clear description of the problem.
    - Steps to reproduce the issue.
    - Logs or screenshots if applicable.

---

Return to the main guide or revisit earlier sections:

- [Installation Guide](../Installation/installation.md)
- [Running Freya](../Installation/running.md)
- [Configuration Guide](../Configuration/configuration.md)

[Next: FAQ](faq.md)
