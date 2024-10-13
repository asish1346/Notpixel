
# NotPixel

**npixel** is a powerful tool designed to bypass tasks, paint, and perform various automated functions seamlessly across devices. This application enables users to effectively enjoy its features, making it an essential tool for Telegram users.

![npixel Showcase](https://raw.githubusercontent.com/asish1346/Notpixel/main/shot.png)


## Warning
This program uses third-party libraries to log into Telegram accounts.

According to Telegram's Terms of Service, all accounts that register or log in using unofficial Telegram API clients will automatically be monitored to prevent violations of the Terms of Service.

So be careful, and hopefully your account won't get blocked.

All risks are borne by the user!

## Features
- ⚡ **Multi-Threading**
- 🎮 **Multi-Session Support**
- 🚀 **Automatic Boosting** (New Update)
- 💰 **Claim Mining**
- 🎨 **Paint Pixels**
- ⏱️ **3X Painting Speed**
- ✏️ **Custom Drawing Coordinates (X, Y)**
- 🌍 **Proxy Support**
- 💸 **User Balance Display**
- 🤖 **Anti-Detection Mechanism**
- 🛠️ **Robust Error Handling**
- 📦 **Easy to Use as a Module**
- 😴 **Sleep Mode for Night Operations**

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
  - [Windows](#windows)
  - [Ubuntu](#ubuntu)
  - [Termux (Android)](#termux-android)
  - [Other Devices](#other-devices)
- [How to Use](#how-to-use)
  - [About config.json](#about-configjson)
  - [Command Line Options / Arguments](#command-line-options--arguments)
  - [About Proxy](#about-proxy)
- [After Execution](#after-execution)
- [Contributing](#contributing)

## Requirements

Before installing **npixel**, ensure you have the following on your device:

- Python 3.x (Recommended version is 3.10)
- pip (Python package installer)
- Git (for cloning the repository)

## Installation

### Windows

1. **Download Python**: 
   - Visit the [Python download page](https://python.org).
   - Download and run the latest installer for Windows. 
   - Make sure to check "Add Python to PATH" during installation.

2. **Download Git**:
   - Visit the [Git download page](https://git-scm.com).
   - Download and install Git, following the setup instructions.

3. Open Terminal/CMD and navigate to the desired directory.
4. Clone the repository using Git:
   ```bash
   git clone https://github.com/asish1346/Notpixel.git
   ```
5. Navigate to the cloned folder:
   ```bash
   cd Notpixel
   ```
6. Install the required packages:
   ```bash
   python -m pip install -r requirements.txt
   ```
7. Copy `config.json.example` to `config.json`:
   ```bash
   copy config.json.example config.json
   ```
8. Adjust the `config.json` according to your preferences (see [About config.json](#about-configjson) for more information).
9. Run the application:
   ```bash
   python bot.py
   ```
   When prompted, enter your authentication key. To obtain a license key, please contact [Asʜᴜ || ☠️ xᴅ](https://telegram.dog/thilubhaii) on Telegram.

### Ubuntu

1. **Download Python**: 
   - Install Python using the terminal:
   ```bash
   sudo apt update
   sudo apt install python3 python3-pip git -y
   ```

2. Open a terminal and navigate to the desired directory.
3. Clone the repository:
   ```bash
   git clone https://github.com/asish1346/Notpixel.git
   ```
4. Navigate to the cloned directory:
   ```bash
   cd Notpixel
   ```
5. Copy `config.json.example` to `config.json`:
   ```bash
   cp config.json.example config.json
   ```
6. Adjust the `config.json` according to your preferences (see [About config.json](#about-configjson) for more information).
7. Install the required packages:
   ```bash
   python3 -m pip install -r requirements.txt
   ```
8. Run the application:
   ```bash
   python3 bot.py
   ```
   When prompted, enter your authentication key. To obtain a license key, please contact [Asʜᴜ || ☠️ xᴅ](https://telegram.dog/thilubhaii) on Telegram.

### Termux (Android)

1. **Download Python**:
   - Install Python:
   ```bash
   pkg update -y && pkg upgrade -y && pkg install python git -y
   ```

2. Open Termux and clone the repository:
   ```bash
   git clone https://github.com/asish1346/Notpixel.git
   ```
3. Navigate to the NotPixel folder:
   ```bash
   cd Notpixel
   ```
4. Copy `config.json.example` to `config.json`:
   ```bash
   cp config.json.example config.json
   ```
5. Adjust the `config.json` according to your preferences (see [About config.json](#about-configjson) for more information).
6. Install the required packages:
   ```bash
   python -m pip install -r requirements.txt
   ```
7. Run the application:
   ```bash
   python bot.py
   ```

### Other Devices

For other platforms or devices, follow these steps:

1. Ensure Python 3.x, pip, and Git are installed.
2. Clone the repository or download it manually.
3. Navigate to the project directory.
4. Copy `config.json.example` to `config.json`:
   ```bash
   cp config.json.example config.json
   ```
5. Adjust the `config.json` according to your preferences (see [About config.json](#about-configjson) for more information).
6. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
7. Run the application:
   ```bash
   python bot.py
   ```

## How to Use

### About config.json

Here's an explanation of the `config.json` contents:

| Keyword          | Description |
|------------------|-------------|
| **api_id**       | To fill this key, you can register first at [my.telegram.org/apps](https://my.telegram.org/apps). This is not mandatory; you can use mine which is already stored in the `config.json.example` file. |
| **api_hash**     | To fill this key, you can register first at [my.telegram.org/apps](https://my.telegram.org/apps). This is not mandatory; you can use mine which is already stored in the `config.json.example` file. |
| **referral_code**| Fill this key with your main account's invitation code. |
| **colors**       | Fill this key with a list of colors you want to apply to the canvas. You can get the color codes (hexcode) inside the Telegram bot (follow the existing format).
| **auto_upgrade** | This key is to activate the auto-upgrade feature. Inside, there are several more keys; give value `true` to activate it and `false` to deactivate it. |
| **countdown**    | This key determines how long to wait for energy to fill up; fill this key with a positive value (in seconds). |
| **time_before_start** | This key is used to create random countdown times before starting the script. The key has 2 values that need to be filled [small, large], example as shown in the config itself (unit: seconds). |

### Command Line Options / Arguments

This script/program also supports several argument parameters that can be used. Here's an explanation of the arguments:

- `--proxy / -P`: Can be used when you have a different filename for storing the proxy list. The default filename used by this script/program to store proxy lists is `proxies.txt`. If you have a file named `prox.txt` as your proxy list file, you just need to add the `--proxy / -P` argument parameter to use your proxy file. Example: 
  ```bash
  python bot.py --proxy prox.txt
  ```

- `--worker / -W`: This argument is used to customize the number of threads/workers used when the bot script runs. By default, this script/software uses `(total CPU cores / 2)` workers. For example, if your CPU has 6 cores, then the number of workers used is 3. You can customize the number of workers using this argument. For example, if you want to set the number of workers to 100, run bot.py with the argument like this: 
  ```bash
  python bot.py --worker 100
  ```
  If you don't like using workers/threads/multiprocessing, you can customize the worker to 1:
  ```bash
  python bot.py --worker 1
  ```

- `--action / -A`: This argument is used to directly enter the desired menu. For example, if this bot script has 5 menus and you don't want to input manually, you can use this argument to directly enter the desired menu. Example: 
  ```bash
  python bot.py --action 5
  ```
  This argument is useful if you use Docker/PM2 to run

 the bot script in the background process.

### About Proxy

You can add proxy lists in the `proxies.txt` file. The proxy format is as follows:

- **If there is authentication**:
  - **Format**: `protocol://user:password@hostname:port`
  - **Example**: `http://admin:admin@69.69.69.69:6969`

- **If there is no authentication**:
  - **Format**: `protocol://hostname:port`
  - **Example**: `http://69.69.69.69:6969`

Please carefully note whether the proxy you are using requires authentication or not, as many people DM me asking about how to use proxies.

## After Execution

After executing the bot, monitor its performance and ensure that it runs smoothly. Keep an eye on any error messages or prompts that may require your attention.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please submit a pull request or raise an issue.
