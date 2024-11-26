---
layout: default
title: Practical AI :: Configure Python Virtual Environment
---

## Configure Python Virtual Environment

Creating a `virtual environment` for your Python project is a best practice. It allows you to manage project-specific dependencies without affecting other projects or the global Python installation. This ensures consistency across different development and production environments.

This guide will walk you through setting up a virtual environment using [venv](https://docs.python.org/3/library/venv.html), which is included in the Python Standard Library for Python 3.3 and newer.


## Prerequisites

- Python 3.3 or newer installed on your system.
- Command Prompt (Windows) or Terminal (macOS/Linux) access.
- Basic knowledge of navigating the command line.

## Windows Instructions

### Step 1: Create a Virtual Environment

1.	Open Command Prompt:
  
    - Press `Win + R`, type `cmd`, and press Enter.

2.	Navigate to Your Project Directory:
    - Use the `cd` command to change directories:

        ```bash
        cd path\to\your\project
        ```

3.	Create the Virtual Environment:
    - Run the following command:

        ```bash
        python -m venv .venv
        ```

    - This creates a directory named `.venv` in your project folder.
    - The `.venv` directory contains the Python executable and a local copy of the pip package manager.

### Step 2: Activate the Virtual Environment

1.	Activate:
    - Run the activation script:

        ```bash
        .venv\Scripts\activate
        ```

  	- You should see (.venv) at the beginning of your command prompt line, indicating that the virtual environment is active.

2.	[Optional] Verify Python Interpreter:
    - Check that you’re using the virtual environment’s Python interpreter:

        ```bash
        where python
        ```

	•	The path should point to your project’s .venv directory.

3.	Install Packages:
    - You can now install packages using pip:

        ```bash
        pip install package_name
        ```


### Step 3: Deactivate the Virtual Environment

1.	Deactivate:
    - To exit the virtual environment, simply run:

        ```bash
        deactivate
        ```

    - The (.venv) prefix should disappear from your command prompt.


## MacOS Instructions

### Step 1: Create a Virtual Environment

1.	Open Terminal:
    - Navigate to `Finder > Applications > Utilities > Terminal`
2.	Navigate to Your Project Directory:
    - Use the `cd` command to change directories:

        ```bash
        cd /path/to/your/project
        ```

3.	Create the Virtual Environment:
    - Run the following command:

        ```bash
        python3 -m venv .venv
        ```

  - This creates a directory named `.venv` in your project folder.
  - The `.venv` directory contains the Python executable and a local copy of the pip package manager.


### Step 2: Activate the Virtual Environment

1.	Activate:
    - Run the activation script:

        ```bash
        source venv/bin/activate
        ```

    - You should see (.venv) at the beginning of your terminal prompt, indicating that the virtual environment is active.

2.	[Optional] Verify Python Interpreter:
    - Check that you’re using the virtual environment’s Python interpreter:

        ```bash
        which python
        ```

    - The path should point to your project’s `.venv` directory.

3.	Install Packages:
    - You can now install packages using pip:

        ```bash
        pip install package_name
        ```


### Step 3: Deactivate the Virtual Environment

1.	Deactivate:
    - To exit the virtual environment, simply run:
        ```bash
        deactivate
        ```

    - The `(.venv)` prefix should disappear from your terminal prompt.


## Additional Notes

- Why Use a Virtual Environment?
  - Isolates project-specific dependencies.
  - Prevents conflicts between packages required for different projects.
  - Simplifies dependency management and deployment.
- Naming the Virtual Environment Directory
  - You can name the virtual environment directory anything you like. Common names include venv, env, or .venv.

- Using python vs. python3
  - On macOS and Linux, the python command might point to Python 2.x.
  - Use python3 to ensure you’re using Python 3.x.
	

- Upgrading pip
  - After activating your virtual environment, upgrade pip to the latest version:

    ```bash
    pip install --upgrade pip
    ```

- Creating a Requirements File
    - To export your project’s dependencies:

        ```bash
        pip freeze > requirements.txt
        ```
    - To install dependencies from a requirements.txt file:

        ```bash
        pip install -r requirements.txt
        ```
    - This is simple txt file with all the dependencies listed in it. It can be written manually or exported from the virtual environment.


- Virtual Environment in Version Control
  - Generally, you should exclude the `.venv` directory from version control systems like Git.
    - Add `.venv/` to your `.gitignore` file.
	
    

- Deleting a Virtual Environment
  - To remove a virtual environment, simply delete the `.venv` directory



- Alternative Virtual Environment Tools
  - `Virtualenv` - An older tool that provides similar functionality and supports
  - `Poetry` - A tool for dependency management and packaging in Python. 
  - `Pipenv` - Combines pip and virtualenv into a single tool for dependency management.
