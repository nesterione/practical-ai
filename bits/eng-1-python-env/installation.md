# Installing Python: A Step-by-Step Guide

This guide will help you install Python on your system. Please follow the instructions specific to your operating system.

## Determine the Latest Stable Python Version

Before installing Python, check the [Python release cycle](https://devguide.python.org/versions/) to determine the current stable version.


## Windows Installation

### Step 1: Check if Python is Already Installed

1.	Open Command Prompt:
    - Press `Win + R`, type `cmd`, and press Enter.
2.	Check Python Version:

    ```bash
    python --version
    ```
    
    - If Python is installed, it will display a version number (e.g., Python 3.9.7).
    - If you receive an error or need a different version, proceed to Step 2.


### Step 2: Download Python

1.	Visit the Official Python Website:
    - Go to [python.org/downloads/windows](python.org/downloads/windows).
2.	Select the Latest Stable Release:
    - Choose the latest Python 3.x release that matches your system architecture (32-bit or 64-bit).
3.	Download the Installer:
    - Click on the executable installer link (e.g., Windows installer (64-bit)).

### Step 3: Install Python

1.	Run the Installer:
    - Locate the downloaded file (e.g., `python-3.x.x-amd64.exe`) in your Downloads folder.
    - Double-click the installer to launch it.
2.	Customize Installation Options:
    - Important: Check the box that says “Add Python 3.x to PATH” at the bottom of the setup window.
    - Click on “Install Now” for a default installation.
3.	Follow the Setup Wizard:
    - If prompted by User Account Control, click “Yes” to allow the installer to make changes.
    - Wait for the installation to complete.
4.	Complete Installation:
    - Click “Close” to exit the setup wizard.

### Step 4: Verify the Installation

1.	Open a New Command Prompt Window:
    - This ensures the PATH changes take effect.
2.	Check Python Version:
    ```
    python --version
    ```
  - You should see the Python version you installed (e.g., Python 3.9.7).

## MacOS Installation

### Step 1: Check if Python is Already Installed

1.	Open Terminal:
	•	Go to `Finder > Applications > Utilities > Terminal`.
2.	Check Python Version:
    ```python
    python3 --version
    ```
- If Python 3.x is installed, it will display the version number.
- If you need Python 3.x or a different version, proceed to Step 2.

### Step 2: Download Python

1.	Visit the Official Python Website:
  -   Go to https://python.org/downloads/macos.
2.	Download the Installer:
  - Click on the latest Python 3.x macOS 64-bit universal2 installer (e.g., `python-3.x.x-macos11.pkg`).

### Step 3: Install Python

1.	Run the Installer:
  - Locate the downloaded .pkg file in your Downloads folder.
  - Double-click the installer to launch it.
2.	Follow the Installation Steps:
    - Click “Continue” through the introduction and license agreement.
    - Click “Agree” to accept the license terms.
    - Click “Install” to begin the installation.
    - Enter your administrator password if prompted.
3.	Complete Installation:
    - Once the installation is successful, click “Close”.


#### Alternative Installation Using [Homebrew](https://brew.sh/

If you prefer using a package manager, you can install Python via Homebrew.

1.	Install [Homebrew](https://brew.sh/) (if not already installed):
2.	Update Homebrew:
    ```bash
    brew update
    ```
3.	Install Python 3:
    ```
    brew install python
    ```
4.	Verify the Installation:
    ```bash
    python3 --version
    ```

### Step 4: Verify the Installation

1.	Open a New Terminal Window.
2.	Check Python Version:
    ```bash
    python3 --version
    ```
  - You should see the Python version you installed.

## Additional Notes

- Environment Variables (Windows):
  - If you forgot to add Python to the PATH during installation, you can add it manually:
	1.	Go to Control Panel > System and Security > System.
	2.	Click on Advanced system settings.
	3.	Click Environment Variables.
	4.	Under System Variables, find and select Path, then click Edit.
	5.	Click New and add the path to your Python installation (e.g., C:\Python39\).
- Using python3 vs. python:
  - On MacOS and Linux, use python3 to ensure you’re using Python 3.x, since python may point to Python 2.x.
- Installing `pip`:
  - `pip` is the package installer for Python and is included by default in Python 3.4 and above.
  - Verify Pip installation:

    ```bash
    pip3 --version
    ```
  - If Pip is not installed, go to [https://pip.pypa.io/en/stable/installation/](https://pip.pypa.io/en/stable/installation/) for installation instructions.



### Next Steps
- [Virtual Environment](./virtual-environment.md): Learn how to create isolated Python environments for your projects.
	