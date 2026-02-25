# 📞 gonopbx - Easy Web Control for Your Phone System

[![Download gonopbx](https://img.shields.io/badge/Download-gonopbx-blue?style=for-the-badge)](https://github.com/omz-bot/gonopbx/releases)

---

## 📋 What is gonopbx?

gonopbx is a user-friendly web interface that helps you manage your Asterisk PBX system. A PBX (Private Branch Exchange) is a phone system used by businesses to handle calls, voicemail, and phone extensions. gonopbx lets you control extensions, SIP trunks, call records, voicemail, and see real-time system activity from your web browser.

The app uses modern tools and can run quickly using Docker, which means you can set it up without needing to install complicated software. It is open-source, so you can trust that the code is available for review and improvement by the community.

---

## 💻 System Requirements

Before you download gonopbx, make sure your computer or server meets these requirements:

- Operating System: Windows 10 or newer, macOS Catalina or newer, or Linux (Ubuntu/Debian recommended)
- Processor: 2 GHz or faster processor (Intel or AMD)
- Memory: At least 4 GB RAM
- Disk Space: Minimum 2 GB free space for installation and data storage
- Network: Internet connection for downloading files and SIP trunk setup
- Software: Docker (see the next section for installation help)

---

## 🛠️ Installing Docker

gonopbx uses Docker to simplify installation and deployment. Docker is software that packages applications with everything they need to run. It works on Windows, macOS, and Linux.

If you don’t have Docker installed, follow these steps:

### Windows and macOS

1. Visit the official Docker website: https://www.docker.com/get-started
2. Download the Docker Desktop installer for your operating system.
3. Run the installer and follow the on-screen instructions.
4. Restart your computer if prompted.
5. Open Docker Desktop to check that it is running.

### Linux

1. Open a terminal window.
2. Follow the Docker installation guide for your distribution:
   - Ubuntu/Debian:  
     ```
     sudo apt update
     sudo apt install apt-transport-https ca-certificates curl gnupg lsb-release
     curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
     echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
     sudo apt update
     sudo apt install docker-ce docker-ce-cli containerd.io
     ```
3. Verify Docker is installed by running:  
   ```
   docker --version
   ```

If Docker runs without error, you are ready for the next step.

---

## 🚀 Download & Install gonopbx

Visit the official gonopbx release page below to get the latest version:

[Download gonopbx](https://github.com/omz-bot/gonopbx/releases)

This page contains the install packages you need. Currently, gonopbx is designed to run inside a Docker container to make setup easy and reliable.

### Steps to install gonopbx

1. **Download the latest release:**
   - Go to the link above.
   - Find the latest release version.
   - Download the `.zip` or `.tar.gz` file containing the configuration and setup scripts.

2. **Extract the files:**
   - Once downloaded, locate the file in your downloads folder.
   - Right-click and choose “Extract All” or use your system's archive tool.

3. **Run the setup script with Docker:**
   - Open your terminal (Command Prompt on Windows, Terminal on macOS/Linux).
   - Navigate to the extracted folder, for example:  
     ```
     cd path/to/gonopbx-folder
     ```
   - Start gonopbx using Docker Compose with the following command:  
     ```
     docker compose up -d
     ```

4. **Wait a few moments:** Docker will download the necessary images and start gonopbx.

5. **Access the web interface:**
   - Open your web browser.
   - Go to: `http://localhost:3000`
   - You should see the gonopbx login screen.

---

## 🔐 First Time Setup

After you access the web interface, take these steps:

1. Create the administrator account with a strong password.
2. Configure your internal extensions (the phones used inside your company).
3. Set up your SIP trunks (connections to external phone lines).
4. Adjust voicemail options and call recording settings based on your needs.
5. Explore the dashboard to monitor real-time call activity and system health.

---

## 🧰 Features Overview

gonopbx simplifies managing your phone system with these features:

- **Extensions:** Add, edit, and remove internal phone extensions.
- **SIP Trunks:** Link your PBX to external phone service providers.
- **Call Detail Records (CDR):** View detailed logs of incoming and outgoing calls.
- **Voicemail:** Set up personalized voicemail boxes and notifications.
- **Real-Time Dashboard:** Watch live call statistics and system performance.
- **User Management:** Control who can use the interface and access PBX settings.
- **Docker Deployment:** Install and run gonopbx using a container in minutes.

---

## 👩‍💻 Using gonopbx

Once set up, use gonopbx daily to manage your PBX system easily:

- Monitor calls to handle peak times.
- Add new users with extensions for your growing team.
- Listen to voicemail messages directly from the browser.
- Check call logs to resolve disputes or review performance.
- Manage SIP trunks to control call cost and quality.

---

## 🌐 Networking and Security Tips

Running a phone system requires attention to network and security:

- Use strong passwords for all user accounts.
- Keep your gonopbx and Docker installations updated.
- Limit access to the web GUI by IP or VPN if possible.
- Enable encryption (TLS/SRTP) on your SIP trunks and devices.
- Regularly back up your configuration and call data.

---

## 🆘 Where to Get Help

If you need assistance, consider these resources:

- [gonopbx GitHub Issues](https://github.com/omz-bot/gonopbx/issues): Report bugs or ask questions.
- Asterisk PBX Forums: Helpful for broader PBX setup questions.
- Docker Documentation: For advanced Docker usage.
- Your VPS or server provider support if you host remotely.

---

## 🔄 Updating gonopbx

When new versions come out:

1. Stop the running Docker containers:  
   ```
   docker compose down
   ```
2. Download and extract the new release.
3. Start the updated version:  
   ```
   docker compose up -d
   ```
4. Your settings and data should persist if you use persistent volumes as recommended.

---

## 📥 Download gonopbx Now

Start managing your phone system today by visiting the release page below to download the latest version:

[Download gonopbx](https://github.com/omz-bot/gonopbx/releases)