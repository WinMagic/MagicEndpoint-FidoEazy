# MagicEndpoint FidoEazy Usage Documentation

This document provides step-by-step instructions on how to use MagicEndpoint FidoEazy for secure SSH access on Windows.

## Prerequisites

Before you begin, ensure you have the following:

* **Windows OS:** MagicEndpoint FidoEazy is currently compatible with Windows operating systems only.
* **TPM 2.0:** A Trusted Platform Module (TPM) version 2.0 is required for secure key storage and device binding.  Most modern systems have this, but you may need to enable it in your BIOS settings.
* **OpenSSH v8.5+:** OpenSSH is required for SSH connectivity.  You can download the latest version from the official Microsoft GitHub page: [OpenSSH-Win64-v9.8.1.0.msi](https://github.com/PowerShell/Win32-OpenSSH/releases/download/v9.8.1.0p1-Preview/OpenSSH-Win64-v9.8.1.0.msi).  For more information on installing OpenSSH, please refer to the Microsoft documentation: [Install-Win32-OpenSSH](https://github.com/PowerShell/Win32-OpenSSH/wiki/Install-Win32-OpenSSH).

## Installation

1. **Download MagicEndpoint FidoEazy:** Download the latest release of MagicEndpoint FidoEazy from the [GitHub releases page](link-to-github-releases).  *(Remember to replace `link-to-github-releases` with the actual link.)*
2. **Run the Installer:** The downloaded file will be an executable. Double-click it to begin the installation process.
3. **Complete the Wizard:** Follow the on-screen instructions in the installation wizard to complete the installation.
4. **System Tray Icon:** Once the installation is finished, the MagicEndpoint FidoEazy icon (sdpin) will appear in your system tray.  This indicates that the application is running.  *(Include a screenshot here showing the system tray icon.  Example: `![SD Running](path/to/sdpin_screenshot.png)`)*.

## Configuration and Usage

1. **Create a MagicEndpoint PIN:** Right-click the SDPin icon in the system tray and select "Create MagicEndpoint Pin".

2. **Set Your PIN:** A "Create PIN" window will appear. Enter your desired PIN and confirm it in the provided fields. Choose a PIN you can remember, but avoid easily guessable sequences.

3. **MagicEndpoint Login Confirmation:** A confirmation message will appear, indicating that you are logged into MagicEndpoint.

4. **Access SSH Management:** Right-click the SDPin icon again and select "SSH Management".

5. **SSH Management Options:** The SSH Management UI provides two key sections:

    a. **SSH Keys:** This section displays a list of device-bound user-generated keys. A default key, generated after you configured your PIN, will be present. You can use this default key or create a new one.

    b. **SSH Servers:** This is where you add the SSH servers you wish to access.

6. <span style="color:red; font-weight:bold;">CRITICAL STEP: Authorize Your Device on the SSH Server</span>  In order to enable login from your authorized device to the SSH server, you **must** copy the SSH public key from the "SSH Keys" section of MagicEndpoint Fido Eazy and add it to the `authorized_keys` file on your Linux SSH server.

    * **Copy the Public Key:** In the "SSH Keys" section, select the key you wish to use and copy the public key associated with it.

    * **Access the Server:** Connect to your Linux SSH server using a traditional method (e.g., password authentication, another SSH key).

    * **Edit `authorized_keys`:** Open the `~/.ssh/authorized_keys` file for the user you wish to log in as. If the file doesn't exist, create it.  **Important:** Ensure the permissions on this file are restrictive (e.g., `chmod 600 ~/.ssh/authorized_keys`).

    * **Paste the Public Key:** Paste the copied public key into the `authorized_keys` file, ensuring it's on a new line.  You can add a comment to the key for identification (e.g., `ssh-rsa AAAAB3Nza... your_public_key_here your_device_name`).

    * **Save the File:** Save the changes to the `authorized_keys` file.

    <span style="color:blue;">We are working on providing scripts and automation to simplify this process in the future.</span>

7. **Add SSH Server in MagicEndpoint:** Once you have configured the SSH public keys on the server, return to the "SSH Servers" tab in MagicEndpoint and add your SSH server details:

    a. **SSH Server Address:** Enter the hostname or IP address of your SSH server.
    b. **Username:** Enter the username you use to log in to the SSH server.

*(Optional: You can include screenshots of each step to make the instructions even clearer. For example: `![SSH Keys Section](path/to/ssh_keys_screenshot.png)`)*


## Contact

If you have any questions or encounter any problems, please feel free to open an issue on the [GitHub repository](https://github.com/WinMagic/MagicEndpoint-FidoEazy/issues).
