### Nodepay Automate
<hr>

Automate Nodepay Network farming using proxies. **Important:** Read the instructions below.

- Use `run.py` 
- Supports Windows without [WSL](https://learn.microsoft.com/en-us/windows/wsl/install).
- Supports multiple accounts and uses 3 proxies per account (both SOCKS and HTTP).

## Requirements
1. Nodepay Account - [Register here](https://app.nodepay.ai/register?ref=FywftYq1yFb66N7)
2. VPS (optional) and Python 3
3. Proxies

## Proxy Sources:
- **Free Residential Proxies:**
  - [WebShare](https://www.webshare.io/?referral_code=p7k7whpdu2jg)
  - [ProxyScrape](https://proxyscrape.com/?ref=odk1mmj)
  - [MonoSans](https://github.com/monosans/proxy-list)
- **Paid Premium Proxies:**
  - [922proxy](https://www.922proxy.com/register?inviter_code=d03d4fed)
  - [Proxy-Cheap](https://app.proxy-cheap.com/r/JysUiH)
  - [Infatica](https://dashboard.infatica.io/aff.php?aff=544)

## Setup Guide

1. **Get Nodepay Token:**
   - Log in to [Nodepay](https://app.nodepay.ai/register?ref=FywftYq1yFb66N7), open Developer Tools (F12 or `Ctrl+Shift+I`).
   - Go to the **Console**, type `allow pasting` and press Enter.
   - Type `localStorage.getItem('np_token')`, press Enter, and copy the token.

2. **Install Dependencies:**

   - **Windows:**
     - Install Python: [Download](https://www.python.org/downloads/)
     - Download the script: [Nodepay Automate](https://github.com/fachryotosaka/nodepay-automate/archive/refs/heads/main.zip)
     - Install requirements: `python -m pip install -r requirements.txt`

   - **Linux (Ubuntu/Debian/CentOS):**
     - Update and install dependencies:
       ```bash
       sudo apt update && sudo apt install git python3 python3-pip -y   # Ubuntu/Debian
       sudo yum install git python3 python3-pip -y  # CentOS
       ```
     - Download script: `git clone https://github.com/fachryotosaka/nodepay-automate`
     - Install requirements: `python3 -m pip install -r requirements.txt`

   - **Termux (Android):**
     - Install Termux: [Download Here](https://f-droid.org/repo/com.termux_1020.apk)
     - Install dependencies:
       ```bash
       pkg update && pkg install git python python-pip -y
       ```
     - Download script: `git clone https://github.com/im-hanzou/nodepay-automate`
     - Install requirements: `python -m pip install -r requirements.txt`

## Running the Script

1. **Configure Proxies:**
   - Replace example proxies in `local_proxies.txt` with your own (3 proxies per account).
   - For multiple accounts, add tokens to `tokens.txt`.

2. **Start Farming:**

   - **Windows/Termux:**
     ```bash
     python3 run.py
     ```
     Select 1, then insert your Nodepay token.

   - **Multi-Account (ensure tokens are in `tokens.txt`):**
     ```bash
     python run.py
     ```
     Select 2.

   - **Linux:**
     ```bash
     python3 run.py
     ```
     Select 1 and insert your Nodepay token

## Notes
- Each account requires 3 proxies. Ensure you have enough for multiple accounts.
- Free proxies may not always work; consider using paid proxies for better reliability.
- Run at your own risk; this script is for educational purposes only.

