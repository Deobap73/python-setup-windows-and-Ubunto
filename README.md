# <p align="center"> python-setup-windows-and-Ubuntu </p>

## Setting Up the Development Environment  

Before diving into Python programming, it's critical to prepare a proper development environment. A well-configured environment ensures that we can write, test, and run our code smoothly, as well as allow us to install libraries and frameworks without conflicts.
I noticed, as I did, that there are some difficulties for programmers who are starting out in Python, in configuring their environment correctly and smoothly, so I created and organized this setup so that Ubuntu is used most of the time, but migrating to Windows whenever necessary, especially for RPA and enterprise application automation.

For this, we will have two configurations:

1. **Configuration in Ubuntu** – Python installation, package manager (pip), VS Code, Jupyter Notebook, and virtual environments.
2. **Windows Setup** – Python installation, integration with PowerShell, VS Code, Jupyter Notebook, and RPA tools.

From there, each module will indicate which system to use, so that it is possible to learn in the way that is most aligned with professional practice.

---

## Setting up the Ubuntu Development Environment

Many developers prefer Ubuntu because it offers a more stable and flexible development environment, as well as being widely used on servers and cloud infrastructure. However, even if you already have Python installed on your system, it's important to make sure everything is up to date and configured correctly. 

We will also learn how to use virtual environments, which are essential to keep different projects organized without dependency conflicts.

In addition, we'll set up **VS Code**, one of the most popular code editors for Python, and install useful tools like **pip**, Python's package manager. By the end of the setup, you'll have an environment ready to start programming and developing projects in Python without difficulties.

---

## Checking if Python is already installed

Ubuntu comes with Python pre-installed. To check the version, open the terminal (`Ctrl + Alt + T`) and run:

```sh
python3 --version
```

If the return is something like `Python 3.x.x`, it means that you already have Python installed.

Otherwise, install it with:

```sh
sudo apt update
sudo apt install python3
```

Confirm the installation by rechecking the version.

---

## Installing pip (Python Package Manager)

`pip` (acronym for "Pip Installs Packages") is the default package manager for Python. It is an essential tool for anyone working with Python, as it makes it easy to install, update, remove, and manage third-party libraries and dependencies.

To ensure that it is installed:

```sh
sudo apt install python3-pip
```

Verify the installation with:

```sh
pip3 --version
```

---

## Installing and Configuring VS Code

**Visual Studio Code (VS Code)** is a powerful source code editor developed by Microsoft. It is known for its versatility, performance, and extensibility.

To install:

```sh
sudo apt update
sudo apt install code
```

After installation, open VS Code and install the **Python extension (Microsoft)** for autocomplete, debugging, and linting support.

---

## Creating and Using Virtual Environments

Virtual environments in Python allow you to isolate dependencies for different projects, avoiding conflicts between libraries.

### Creating a Virtual Environment

```sh
mkdir ~/python-projects
cd ~/python-projects
python3 -m venv myenv
```

### Activating the Virtual Environment

```sh
source myenv/bin/activate
```

The terminal will show `(myenv) user@ubuntu:~$`, indicating that you are inside the virtual environment.

### Deactivating the Virtual Environment

```sh
deactivate
```

---

## Installing Jupyter Notebook (Optional, for Data Science and Machine Learning)

Jupyter Notebook is widely used for interactive programming and data visualization.

To install it inside a virtual environment:

```sh
pip install jupyter
```

To run Jupyter Notebook:

```sh
jupyter notebook
```

This will open Jupyter in the browser.

---

## Summary of Ubuntu Setup

✔ Installed Python and checked the version  
✔ Installed pip  
✔ Installed VS Code  
✔ Created and activated a virtual environment  
✔ Installed Jupyter Notebook  

---

## Setting Up the Windows Development Environment

While Ubuntu is widely used by developers and data scientists, Windows is still the most popular operating system in the world and often the default choice in businesses and development teams.

By the end of this setup, you will have a completely configured environment on Windows, allowing you to program in Python without difficulty. 

---

## Downloading and Installing Python

1. Visit the official website:
   👉 [Download Python for Windows](https://www.python.org/downloads/windows/)
2. Download the latest version of Python 3.x.
3. **Important:** During installation, check the `Add Python to PATH` option.
4. Click on `Install Now` and wait for it to install.
5. To verify that the installation was successful, open the Command Prompt (cmd) and type:

```sh
python --version
```

If everything is correct, `Python 3.x.x` will appear.

---

## Installing pip (Python Package Manager)

pip is usually already installed with Python on Windows, but confirm by running:

```sh
pip --version
```

If the command is not recognized, update pip with:

```sh
python -m ensurepip --default-pip
python -m pip install --upgrade pip
```

---

## Installing VS Code and Configuring for Python

1. Download Visual Studio Code at:  
   👉 [Download VS Code](https://code.visualstudio.com/)
2. During installation, check the `Add to PATH` option.
3. After opening VS Code, install the **Python extension (Microsoft)**.

---

## Creating and Using Virtual Environments

To create a virtual environment on Windows, use the Command Prompt (cmd):

1. Create a folder for your projects:

```sh
mkdir C:\python-projects
cd C:\python-projects
```

2. Create a virtual environment:

```sh
python -m venv myenv
```

3. Activate the virtual environment:

```sh
myenv\Scripts\activate
```

The terminal will show `(myenv) C:\python-projects>`, indicating that the virtual environment is active.

To deactivate it, use:

```sh
deactivate
```

---

## Installing Jupyter Notebook (Optional, for Data Science and Machine Learning)

To install Jupyter Notebook inside the virtual environment:

```sh
pip install jupyter
```

To open Jupyter:

```sh
jupyter notebook
```

This will open Jupyter in the browser.

---

## Summary of Windows Setup

✔ Installed Python on Windows  
✔ Configured pip  
✔ Installed VS Code  
✔ Created and activated a virtual environment  
✔ Installed Jupyter Notebook  


