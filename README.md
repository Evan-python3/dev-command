# Dev Command For Windows

![Version](https://img.shields.io/badge/version-1.0.0-blue)

**Dev Command For Windows** is a command-line tool designed to simplify development tasks on Windows.

It provides useful commands for developers to create, analyze, run, and manage projects from a single CLI application.

---

# ✨ Features

* 🔍 Project code analysis
* 📦 Software installation using Winget
* 🏗️ Automatic project creation
* 🔄 Project file conversion
* 🖥️ Open projects directly in Visual Studio Code
* ▶️ Run projects automatically
* 🌳 Display project structure
* 🔄 Automatic update system

---

# 📥 Installation

## Using the installer

Download and run:

```
DevCommandSetup.exe
```

The installer will:

* Install Dev Command on your computer
* Add `dev` to your Windows PATH automatically
* Create shortcuts

After installation, open a new terminal and run:

```cmd
dev help
```

---

# 🚀 Usage

General command format:

```cmd
dev <command>
```

Display help:

```cmd
dev help
```

---

# 📌 Available Commands

## Version

Display the current installed version:

```cmd
dev --version
```

Example:

```
Version : 1.0.0
```

---

# 🔄 Update

Check for updates:

```cmd
dev --update
```

or:

```cmd
dev --upd
```

The update system will:

1. Check the latest available version
2. Download the new version
3. Replace the old executable
4. Update the local configuration

---

# 🔍 Analyze Project

Analyze the current project:

```cmd
dev analyze
```

The analyzer uses:

* pylint
* mypy
* pytest

It helps detect:

* Code errors
* Type problems
* Test failures
* Potential improvements

---

# 📦 Install Software

Install development tools using Windows Package Manager:

```cmd
dev install <software>
```

List available software:

```cmd
dev install --list
```

Available software:

| Command | Software           |
| ------- | ------------------ |
| python  | Python             |
| git     | Git                |
| vscode  | Visual Studio Code |
| node    | Node.js            |
| docker  | Docker Desktop     |

Example:

```cmd
dev install vscode
```

---

# 🏗️ Create Projects

Create a new project:

```cmd
dev setup <type> <name>
```

---

## Website Project

Example:

```cmd
dev setup website MyWebsite
```

Creates:

```
MyWebsite/
│
├── app.py
├── static/
├── templates/
└── README.md
```

---

## Python Application

Example:

```cmd
dev setup app MyApplication
```

Creates:

```
MyApplication/
│
├── src/
│   └── main.py
│
├── requirements.txt
└── README.md
```

---

## Script Project

Example:

```cmd
dev setup script MyScript
```

Creates:

```
MyScript/
│
├── script.bat
└── README.md
```

---

# 🔄 Convert Projects

Convert project files:

```cmd
dev convert
```

This command moves:

```
templates/
static/
```

into:

```
Converted/
```

---

# 🖥️ Open in Visual Studio Code

Open the current folder in VS Code:

```cmd
dev open
```

Requirements:

* Visual Studio Code installed
* `code` command available in PATH

---

# ▶️ Run Projects

Automatically run the project:

```cmd
dev run
```

Supported files:

```
app.py
src/main.py
script.bat
```

---

# 🌳 Display Project Tree

Show the project structure:

```cmd
dev tree
```

Example:

```
Project/
│
├── app.py
├── templates/
└── static/
```

---

# 🔄 Update System

Dev Command uses a remote update file:

```
update.json
```

Example:

```json
{
    "version": "1.0.1",
    "file_id": "GOOGLE_DRIVE_FILE_ID"
}
```

The program compares:

```
Installed version
        |
        v
Latest online version
```

If a newer version exists, it downloads and installs it automatically.

---

# 🛠️ Development

Clone the repository:

```cmd
git clone <repository-url>
```

Install dependencies:

```cmd
pip install requests gdown
```

Run the project:

```cmd
python dev.py
```

---

# 📁 Project Structure

Example:

```
Dev-Command/
│
├── dev.py
├── updater.py
├── config.json
├── README.md
└── requirements.txt
```

---

# 📋 Requirements

* Windows 10 / Windows 11
* Python 3.10+
* Winget
* Git (optional)
* Visual Studio Code (optional)

---

# 👨‍💻 Author

Created by **Xyltraz**

---

# 📄 License

This project is distributed for personal and educational use.

