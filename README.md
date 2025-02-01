# MagicEndpoint FIDO Eazy

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

This repository provides standalone freeware and instructions for securing SSH access on Windows using FIDO keys and SSH certificates, leveraging device-bound keys and optional TPM integration.  It simplifies secure SSH access while enhancing device control.

## Situation and Complications

Many Windows users rely on insecure username/password authentication for SSH. While public/private key pairs are more secure, they introduce management complexities and risks, such as key theft.  Securing private keys with TPM adds further complexity. Existing solutions like virtual smart cards (soon to be deprecated) and TPM-TLS certificates (limited client compatibility) are not ideal. FIDO SSH keys offer a more secure and user-friendly alternative, but integrating them seamlessly with Windows can be challenging.

## The Solution: MagicEndpoint FIDO Eazy

MagicEndpoint FIDO Eazy simplifies secure SSH key management on Windows by leveraging FIDO keys, SSH certificates, and optional TPM integration.  This approach offers:

* **Passwordless Authentication:** Eliminate password-related risks like guessing, reuse, and phishing.
* **Device Binding:** Restrict access to authorized devices, preventing unauthorized use even if credentials are compromised.
* **Centralized Management:** Simplify key management with SSH certificates, enabling easy issuance and revocation.
* **Scalability:** Easily manage SSH access for numerous users and devices.
* **FIDO2 Compliance:** Leverage the security and interoperability of FIDO2 authenticators.
* **TPM Integration (Optional):** Enhance device binding and key protection with Trusted Platform Modules.
* **User-Friendly Interface:** Streamlined key generation, management, and backup.
* **Broad Compatibility:** Supports popular SSH clients like PuTTY-CAC and Microsoft's native OpenSSH command-line tools (ssh, scp, sftp, and SSH tunnels).

## Key Features and Benefits

* **Automatic FIDO SSH Key Creation:**  Effortlessly generate TPM-backed FIDO SSH keys.
* **One-Click Key Creation:** Easily add additional keys as needed.
* **Intuitive Key Management UI:**  Manage keys with a simple, user-friendly interface.
* **Seamless Key Backup:** Securely back up your keys for recovery.
* **Enhanced Security with ME Client:**  Keys become unusable when the user logs out of MagicEndpoint, adding an extra layer of protection.

## Getting Started

This repository provides:

* **Certificate Generation Tools:** Tools for creating SSH certificates signed by your own Certificate Authority (CA).
* **Key Management Examples:** Scripts and examples for managing SSH keys and certificates.
* **FIDO2 Integration Demonstrations:**  Examples of utilizing FIDO2 authenticators for SSH authentication.

Refer to the [documentation](link-to-documentation) for detailed instructions on how to set up and use MagicEndpoint FIDO Eazy.

## Contributing

Contributions are welcome! Please see the [contributing guidelines](CONTRIBUTING.md) for more information.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

[Your Name/Team] - [Your Email/Contact Information]
