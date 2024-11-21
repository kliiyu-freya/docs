# Configuring Freya

Configuring Freya allows you to tailor its behavior and settings to your specific needs. The easiest way to configure Freya is through the dashboard.

---

## Table of Contents

1. [Accessing the Dashboard](#accessing-the-dashboard)
2. [Using the Configuration Panel](#using-the-configuration-panel)
3. [Saving and Applying Changes](#saving-and-applying-changes)

---

## Accessing the Dashboard

To configure Freya, start by accessing the dashboard. Open your browser and navigate to the following URL:

    http://localhost:6672

Ensure that Freya is running before attempting to access the dashboard. If the page doesn't load:
- Verify that the Freya Dashboard is installed.
- Confirm Freya is running with the `freya run` command.

---

## Using the Configuration Panel

Once on the dashboard:

1. **Log In**: If required, log in using the credentials set during installation (or the default credentials if not configured yet).
   
2. **Navigate to Settings**: Locate and click on the **Settings** or **Configuration** tab in the dashboard menu.

3. **Adjust Settings**: Customize the available options, which may include:
   - **General Settings**: Modify Freya's name, response behavior, and operational preferences.
   - **Integration Settings**: Add or configure third-party integrations such as smart home devices or APIs.
   - **Network Settings**: Update connection settings, including ports and hostnames.

4. **Advanced Configuration**:
   - For more advanced users, use the **Advanced** or **Custom Scripts** sections to modify Freya's internal behavior or add custom modules.

---

## Saving and Applying Changes

After making your changes:

1. **Save Settings**: Click the **Save** or **Apply Changes** button on the dashboard.
2. **Restart Freya** (if prompted): Some changes require a restart to take effect. Use:

    freya run

---

Continue to the next section to learn how to troubleshoot Freya.

[Next: Troubleshooting Freya](../Troubleshooting/repair.md)