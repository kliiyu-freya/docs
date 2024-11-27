# Frequently Asked Questions (FAQ)

This document addresses common questions about Freya. If your question isn't answered here, refer to the [Troubleshooting Guide](repair.md) or reach out for support.

---

## General Questions

### 1. **What is Freya?**
Freya is an AI assistant/home assistant that helps automate tasks, manage smart devices, and provide AI-powered assistance in your daily life.

### 2. **What platforms does Freya support?**
Freya runs on systems that support Docker and Python, including Windows, macOS, and Linux.

### 3. **Do I need coding skills to use Freya?**
No, Freya is designed for ease of use with a dashboard for configuration. However, advanced users can customize Freya by modifying its scripts.

---

## Installation Questions

### 4. **What are the prerequisites for installing Freya?**
You need:

- **Docker** for containerized operation.
- **Python** for CLI functionality.
- Optional: **Git** if cloning the source code.

### 5. **How do I verify that Freya is installed correctly?**
Run the following command:

    freya -v

---

## Usage Questions

### 6. **How do I start Freya?**

Use the command:

    freya run

If that doesn't work, try:

    python -m freya run


### 7. **How do I access the Freya dashboard?**

Navigate to:

    http://localhost:6672

Make sure Freya is running and the dashboard is installed.


### 8. **Can Freya integrate with smart home devices?**

Yes, Freya supports integration with various smart devices. You can configure these integrations through the dashboard.

---

## Configuration Questions

### 9. **How do I configure Freya?**

Use the dashboard at:

    http://localhost:6672

Navigate to the **Settings** section to update configurations.


### 10. **What should I do if configuration changes don’t apply?**¨

Ensure you click **Save** or **Apply Changes** in the dashboard and restart Freya:

    freya restart

---

## Troubleshooting Questions

### 11. **Why is the dashboard not accessible?**

- Verify Freya is running:

        freya run

-  Ensure the dashboard and core is installed:

        freya install core:latest
        freya install dashboard:latest


### 12. **What should I do if Freya stops working?**

- Restart Freya:

        freya restart

- Check the logs for errors:

        freya logs


### 13. **How do I view Freya's logs?**

You can view logs via:

- **Dashboard**: At `http://localhost:6672`
- **CLI**:

        freya logs

---

## Advanced Questions

### 14. **Can I customize Freya's behavior?**

Yes, advanced users can modify Freya by:

- Editing configuration files.
- Adding custom scripts in the **Advanced** section of the dashboard.


### 15. **Is Freya open-source?**

Yes, Freya is licensed under the MIT license
Check the licensing and repository information on Freya's [GitHub page](https://github.com/kliiyu-freya).

---

## Support

If your question isn't answered here:

- Visit the [Troubleshooting Guide](repair.md).
- Check Freya's GitHub Discussions.
- Report issues on Freya's GitHub repository with detailed logs and error descriptions.

---

Return to the main guide:

- [Installation Guide](../Installation/installation.md)
- [Running Freya](../Installation/running.md)
- [Configuration Guide](../Configuration/configuration.md)
- [Troubleshooting Guide](../Troubleshooting/repair.md)
