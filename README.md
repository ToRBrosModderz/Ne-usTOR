# Ne-usTOR

Ne-usTOR is a free, safe, open-source, web-based, cross-platform, and full-featured RAT (Remote Administration Tool) that allows you to control all your devices via browser anywhere.

✅ No data collection: Spark does not collect any user information.
✅ No auto-updates: The server will not update itself.
✅ Direct communication: Clients communicate exclusively with your server.

GitHub repo size	GitHub issues	GitHub closed issues
GitHub downloads	GitHub release (latest by date)
⚠️ Disclaimer
THIS PROJECT, ITS SOURCE CODE, AND RELEASES SHOULD ONLY BE USED FOR EDUCATIONAL PURPOSES.

❌ Illegal usage is strictly prohibited.
❌ Authors and developers are not responsible for any misuse.
✅ Use it at your own risk.

If you find security vulnerabilities, do not open an issue. Contact me immediately via email.

🚀 Quick Start

Binary Execution
Download the executable from the releases page.
Follow the Configuration instructions.
Run the executable and access the web interface at http://IP:Port.
Generate a client and run it on the target device.
Start managing your devices!
⚙️ Configuration
The configuration file config.json should be in the same directory as the executable.

Example:

{
    "listen": ":8000",
    "salt": "123456abcdef123456", 
    "auth": {
        "username": "password"
    },
    "log": {
        "level": "info",
        "path": "./logs",
        "days": 7
    }
}
Main Parameters:
listen (required): Format IP:Port.
salt (required): Max length 24 characters. After modification, all clients need to be regenerated.
auth (optional): Authentication credentials (username:password).
Hashed passwords are recommended ($algorithm$hashed-password).
Supported algorithms: sha256, sha512, bcrypt.
log (optional): Logging configuration.
level: disable, fatal, error, warn, info, debug.
path: Log directory (default: ./logs).
days: Log retention days (default: 7).
🛠️ Features
Feature/OS	Windows	Linux	MacOS
Process Manager	✔	✔	✔
Kill Process	✔	✔	✔
Network Traffic	✔	✔	✔
File Explorer	✔	✔	✔
File Transfer	✔	✔	✔
File Editor	✔	✔	✔
Delete File	✔	✔	✔
Code Highlighting	✔	✔	✔
Desktop Monitor	✔	✔	✔
Screenshot	✔	✔	✔
OS Info	✔	✔	✔
Remote Terminal	✔	✔	✔
* Shutdown	✔	✔	✔
* Reboot	✔	✔	✔
* Log Off	✔	❌	✔
* Sleep	✔	❌	✔
* Hibernate	✔	❌	❌
* Lock Screen	✔	❌	❌
🚨 Functions marked with * may require administrator/root privileges.

