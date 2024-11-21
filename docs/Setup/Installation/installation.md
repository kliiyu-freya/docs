## Installation

### Prerequisites
Before installing Freya, ensure the following prerequisites are met:

1. **Docker**: Freya runs in a Docker container. Install Docker from the [official website](https://www.docker.com/get-started).
2. **Python**: Freya requires Python to be installed. Download and install Python from the [official Python website](https://www.python.org/downloads/).

### Steps to Install Freya

1. **Install the Freya CLI**
    Open your terminal and run the following command:
    
        pip install freya-cli

2. **Verify Installation**
    Run the following command to verify that the Freya CLI is installed:

        freya -v
    > If that doesnt work run: `python -m freya -v`

3. **Install the Freya Core**
    Run the following command to install Freya core:

        freya --install core:latest

4. **Optional**
    Install the Freya Dashboard:

        freya --install dashboard:latest

4. **Verify Installation**
    Run the following command to verify the installation:

        freya --list packages

---

Continue to the next section to learn how to run and interact with Freya.

[Next Running Freya](running.md).