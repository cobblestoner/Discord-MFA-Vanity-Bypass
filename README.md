# MFA Python Bypass

This repository contains a Python script designed to interact with the Discord API, specifically for automating MFA (Multi-Factor Authentication) processes and managing vanity URLs in Discord servers.

## Features ✨
- **Automates MFA Handling**: Efficiently generates MFA tickets and tokens using the Discord API.
- **Vanity URL Management**: Updates Discord server vanity URLs with ease.
- **Secure and Configurable**: Reads sensitive data like tokens and passwords from a `config.json` file to ensure user-specific configurations.

## Prerequisites 🛠️
1. **Python 3.7+**: Make sure Python is installed on your system. [Download Python](https://www.python.org/downloads/)
2. **Dependencies**: Install the required Python package:
   ```bash
   pip install tls-client typing-extensions
   ```
3. **Discord API Token**: Obtain your Discord bot or user token.
4. **Vanity Code**: The custom code you want to set for your Discord server's vanity URL.

## Setup 🚀
1. Clone this repository:
   ```bash
   git clone https://github.com/kneeling/Discord-MFA-Vanity-Bypass.git
   cd Discord-MFA-Vanity-Bypass
   ```
2. Create a `config.json` file with the following structure:
   ```json
   {
       "vanity-code": "your-vanity-code",
       "password": "your-mfa-password",
       "token": "your-discord-token"
   }
   ```
3. Run the script:
   ```bash
   python main.py
   ```

## How It Works 🧠
1. **Initialization**: 
   - The script initializes a session using `tls-client` to emulate a Chrome browser.
   - Reads configurations from `config.json`.

2. **MFA Ticket Generation**:
   - Uses the Discord API to request an MFA ticket tied to the provided vanity code.

3. **Vanity Token Retrieval**:
   - Completes the MFA process using the password and MFA ticket to retrieve an authentication token.

## Security Notes 🔒
- **Token Safety**: Your Discord token grants access to your account or bot. Never share it publicly.
- **Use Responsibly**: This script interacts with the Discord API. Ensure you're adhering to Discord's [Terms of Service](https://discord.com/terms) and [Developer Policy](https://discord.com/developers/docs/policy).

## Disclaimer ⚠️
This script is intended for educational and personal use only. Unauthorized use of this script, especially for purposes that violate Discord's terms, may result in account bans or legal consequences. Use it responsibly.

## License 📄
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

# MADE BY POLAR

```diff
- if you wish to contact me, here is my user-id: 1147157867472900106
```
