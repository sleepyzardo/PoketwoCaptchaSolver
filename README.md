# Pokétwo Captcha Solver

## Overview

The Pokétwo Captcha Solver is a high-performance tool designed to solve captchas for the Pokétwo Discord bot. It utilizes advanced techniques for captcha recognition and integrates with Discord's webhook system for notifications.

## Features

- **Captcha Solving:** Automated solving of captchas using various services.
- **Logging:** Detailed logs of captcha-solving attempts and errors.
- **Webhooks:** Sends notifications to Discord upon solving attempts.
- **License Management:** Validates license keys to ensure software authenticity.
- **Configuration:** Customizable settings for captcha service, webhook URLs, and more.
- **Discord Bot:** A Personalized Discord bot for reading and solving captchas.

## How It Works

1. **Initialization:** Upon startup, the software verifies the license and checks for updates. If everything is in order, it begins monitoring and solving CAPTCHAs.
2. **CAPTCHA Solving:** When a CAPTCHA request is received, the software utilizes the configured CAPTCHA service to solve it. The result is then processed and logged.
3. **Web Interface Access:** Uses the FastAPI web interface to trigger CAPTCHA solving requests and monitor progress.

## Requirements

- A functional license key, Bought from a reseller/admin.
- A functional captcha solving key obtained from your preferred source.

## Configuration

Update the `config.toml` file to configure the software according to your environment and preferences. Here is an example configuration:

```toml
[server]
port = 3000
save_logs = true

[captcha]
service = "Preferred service to solve reCaptchav2."
key = "Service Key"
license = "Software license"

[discord]
webhook = "Discord webhook"
bot_token = ""
whitelisted_guilds = []
message = "captcha <> off optional"
```
This example configuration demonstrates how to set up the server port, captcha service, and Discord webhook for the Pokétwo Captcha Solver. Adjust the values as needed for your setup.

## Setup

Follow these steps to set up the Pokétwo Captcha Solver on your system:

1. **Download and Extract the Software:**
   - If you haven't already, download the software package from the provided source.
   - Extract the files to a location on your computer where you want to run the software.

2. **Install Dependencies:**
   - By Default, The executable already comes pre-installed with all the dependencies. 
   - Open a terminal (Command Prompt on Windows, Terminal on macOS/Linux) and navigate to the folder where you extracted the software.

4. **Configure the Software:**
   - Locate the `config.toml` file in the software folder. This file contains settings that control how the software operates.
   - Open `config.toml` in a text editor (e.g., Notepad on Windows, TextEdit on macOS, or any code editor).
   - Update the settings in the file to match your environment. For example, set your server port, captcha service key, and Discord webhook URL. 
   - Save the changes to `config.toml`.

5. **Run the Software:**
   - In the terminal, make sure you're still in the software's directory.
   - Start the software by running the `start.bat` file
   - The software will start running, and you should see messages indicating its status in the terminal.

6. **Monitor Logs and Usage:**
   - The software logs its activities and any errors in the `bin/logs/` directory. Check these logs if you need to troubleshoot issues or monitor performance.

7. **Access the Web Interface:**
   - Open a client and send requests to `http://localhost:3000/solve/123x2384` (or the port specified in your `config.toml` file) to access the solve functionality.

If you encounter any issues or have questions, please refer to the documentation or contact support for assistance.

> [!NOTE]
> - **License and Keys:** Ensure your license key and any other required keys are correctly configured in the `config.toml` file. An incorrect or expired license key may prevent the software from functioning.
> - **Dependencies:** Make sure all dependencies listed in `requirements.txt` are installed. Run `pip install -r requirements.txt` to install them.
> - **Port Configuration:** By default, the software uses port 3000. If this port is occupied by another service, you need to change the port number in the `config.toml` file.
> - **Configuration Backup:** It’s wise to back up your `config.toml` file before making any modifications. This way, you can easily restore your previous settings if needed.

> [!CAUTION]
> - **Sensitive Information:** Do not share your license key, webhook URLs, or any other sensitive information publicly. Exposure of this information can lead to unauthorized access or misuse of the software.
> - **Error Handling:** Monitor the logs located in the `bin/logs/` directory for any errors or issues. Address any problems promptly to ensure smooth operation of the software.
> - **Security Risks:** Always ensure that the software is run in a secure environment. Regularly update your configuration and software to address any security vulnerabilities.
> - **System Resources:** Running the software may consume significant system resources. Ensure your system meets the minimum requirements and has sufficient resources to handle the workload.

## License

### Understanding the License

The software provided in this repository is protected by a license agreement. The license determines how you can use, modify, and distribute the software. Here's an overview of key points related to the license:

> [!IMPORTANT]
> - **License Key:** To use this software, you must have a valid license key. The license key is required to activate the software and access its features. Ensure that your license key is properly configured in the `config.toml` file under the `[captcha]` section. An invalid or expired key may prevent the software from functioning.
> - **License Validity:** The validity of your license is crucial for the continued operation of the software. Regularly check your license status and renew it if necessary to avoid interruptions. The software may include mechanisms to validate the license periodically.
> - **License Management:** Keep your license key secure and confidential. Avoid sharing it publicly or with unauthorized individuals. If you encounter any issues with your license, contact support for assistance.
> - **License Expiry:** Monitor the expiration date of your license. An expired license will result in the software becoming inactive or limited in functionality. Renew your license before it expires to ensure uninterrupted access to the software.

> [!WARNING]
> - **Unauthorized Use:** Using the software without a valid license is a violation of the license agreement and may lead to Revoking of the license. Ensure that you comply with the terms of the license to avoid any potential legal issues.

### Pricing

This software is currently available under a paid license. Pricing details and subscription options can be obtained by contacting our sales team directly. 

For information on pricing tiers, licenses, or custom solutions, please reach out to us at @sleepyzardo or @dependential on discord.

### Current Pricing Tiers

- **Basic Plan**: Includes a monthly license key and 24/7 support. 
- **Standard Plan**: Includes a lifetime license key and 24/7 support.
- **Premium Plan**: Includes a lifetime source code access with priority support and custom code requests.

Please note that pricing may vary based on specific requirements and usage. Contact us for a detailed quote and to discuss your needs.



### License Agreement

The full terms of the license agreement are provided with the software. Review the license agreement carefully to understand your rights and obligations. The agreement typically covers:

- **Permitted Uses:** How you are allowed to use the software, including any restrictions.
- **Modifications:** Whether you can modify or customize the software.
- **Distribution:** Rules regarding the distribution or sharing of the software.
- **Support and Updates:** Information about support and how updates are handled.

For any questions or issues related to the license, please contact our support team. Ensure that you comply with all terms and conditions to make the most of the software.

## Contact

For support or inquiries, please contact @sleepyzardo or @dependential on discord

## Contributing

As this is a private repository, contributions are limited to authorized personnel.
To contribute your ideas, Please contact me on discord @sleepyzardo.

## Disclaimer

Use of this software is subject to the terms outlined in the license agreement. Unauthorized use or distribution is prohibited.

## Updates
```diff
! Initial Release
