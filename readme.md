# SyntaxVPN

<p align="center">
  <strong>A modern VPN client for Windows.</strong>
  <br>
  Simple interface. Convenient server management. Powered by Xray Core.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows-blue?logo=windows" alt="Windows">
  <img src="https://img.shields.io/badge/Java-21-orange?logo=openjdk" alt="Java 21">
  <img src="https://img.shields.io/badge/Version-1.1.0-green" alt="Version 1.1.0">
  <img src="https://img.shields.io/badge/Architecture-x64-lightgrey" alt="x64">
</p>

---

## About

**SyntaxVPN** is a desktop VPN client for Windows designed to make managing VPN connections simple and convenient.

Built with JavaFX and powered by Xray Core, SyntaxVPN provides an intuitive interface for managing server profiles and connecting to supported VPN protocols.

The application focuses on simplicity, functionality, and a clean user experience.

## Features

- **VLESS Support** — connect using VLESS server configurations.
- **Shadowsocks Support** — import and manage Shadowsocks servers.
- **Subscription Import** — import server configurations using HTTPS subscription links.
- **Base64 Decoding** — automatically decode Base64-encoded subscriptions.
- **Server Management** — add and manage server profiles.
- **Connection Management** — connect to and disconnect from servers.
- **Modern Interface** — clean and intuitive JavaFX interface.
- **Dark and Light Themes** — choose your preferred appearance.
- **Multilingual Interface** — English and Russian languages.
- **Automatic Profile Saving** — server profiles are saved locally.
- **Windows Installer** — convenient installation using a standalone setup executable.

## Screenshots

<!-- Add application screenshots here -->

| Main Window | Server Management |
|:---:|:---:|
| Coming soon | Coming soon |

| Dark Theme | Light Theme |
|:---:|:---:|
| Coming soon | Coming soon |

## Download

The latest version of SyntaxVPN is available in the GitHub Releases section.

**[Download SyntaxVPN] (https://github.com/alphawex090/syntaxvpn-vpnclient-x64/releases/tag/v1.1.0))**

### Installation

1. Download `SyntaxVPN-Setup.exe` from the Releases page.
2. Run the installer.
3. Follow the installation wizard.
4. Launch SyntaxVPN from the Start Menu or Desktop shortcut.
5. Add a server or import a subscription.
6. Connect and enjoy!

## System Requirements

- Windows 10 or Windows 11.
- 64-bit operating system (x64).
- Internet connection.
- Administrator privileges for installation.

## How to Use

### 1. Launch SyntaxVPN

Open SyntaxVPN after installation.

### 2. Add a Server

Navigate to the **Servers** tab.

You can add servers in two ways:

- Paste an individual server configuration link.
- Paste an HTTPS subscription URL.

Currently supported protocols:

- VLESS
- Shadowsocks

### 3. Select a Server

Choose a server from your server list.

### 4. Connect

Click the connection button and wait for the connection status to update.

### 5. Disconnect

Use the disconnect button to terminate the VPN connection.

## Technology Stack

SyntaxVPN is built using the following technologies:

| Technology | Purpose |
|---|---|
| Java 21 | Main programming language |
| JavaFX | Graphical user interface |
| Xray Core | VPN engine |
| Gradle | Build automation |
| Gson | JSON processing |
| Inno Setup | Windows installer |

## Project Structure

```text
SyntaxVPNDesktop/
│
├── installer/
│   ├── SyntaxVPN.ico
│   └── SyntaxVPN.iss
│
├── runtime/
│   ├── xray.exe
│   ├── geoip.dat
│   ├── geosite.dat
│   └── ...
│
├── src/
│   └── main/
│       └── java/
│           └── com/
│               └── syntaxvpn/
│
├── build.gradle
├── settings.gradle
└── README.md
```

## Building from Source

### Requirements

- JDK 21
- Git
- Gradle Wrapper (included in the repository)
- Inno Setup (for building the installer)

### Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Navigate to the Project Directory

```bash
cd SyntaxVPNDesktop
```

### Build the Project

```powershell
.\gradlew.bat clean build
```

### Create the Application Package

```powershell
.\gradlew.bat packageApp
```

The packaged application will be available in:

```text
build/package/SyntaxVPN/
```

### Build the Windows Installer

Open the following file using Inno Setup Compiler:

```text
installer/SyntaxVPN.iss
```

Compile the script to generate the Windows installer.

The installer will be created in:

```text
build/installer/SyntaxVPN-Setup.exe
```

## Privacy and Security

- Use subscription links and server configurations only from trusted providers.
- Do not share private subscription URLs or server credentials.
- Server profiles are stored locally on your computer.
- HTTPS certificate verification is enabled when downloading subscriptions.

## Community and Support

Follow the project on Telegram to receive updates, announcements, and information about new releases.

**Telegram:** https://t.me/syntaxvpns

For bug reports and feature requests, use the GitHub Issues section.

## License

SyntaxVPN uses third-party software and components, including Xray Core.

Each third-party component remains subject to its respective license.

Please review the applicable licenses before redistributing the application.

---

<p align="center">
  <strong>SyntaxVPN</strong>
  <br>
  Simple. Modern. Connected.
  <br><br>
  Made by SyntaxVPN Team.
</p>
