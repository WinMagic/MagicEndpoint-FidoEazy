# MagicEndpoint FIDO Eazy

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Ditch the clunky old way of managing SSH keys! You know the drill: generating key pairs, wrestling with command lines, and then nervously guarding those precious private keys like they're buried treasure. And let's be honest, who hasn't accidentally shared a key or struggled to revoke access when someone leaves the team? Traditional SSH keys are a security upgrade from passwords, sure, but they come with a whole new set of headaches. Plus, if those keys live unprotected on your hard drive, they're still vulnerable.  And here's the kicker – with traditional keys, anyone with access to that key can try to log in, regardless of whether their *device* is authorized. Wouldn't it be awesome if there was a simpler, more secure way – one that not only blocked unauthorized *users* but also ensured that only *authorized devices* could connect? Good news – there is! We're talking passwordless login, rock-solid security thanks to FIDO2 and TPM, and a streamlined experience that even your grandma could handle. No more key sprawl, no more security worries, and best of all, ironclad device authorization. That's what MagicEndpoint FIDO Eazy is all about!

## Situation and Complications

Many Windows users still rely on insecure username/password authentication for SSH. While public/private key pairs are more secure, they introduce management complexities and risks, such as key theft. Securing private keys with TPM adds further complexity. Existing solutions like virtual smart cards (soon to be deprecated) and TPM-TLS certificates (limited client compatibility) are not ideal. FIDO SSH keys offer a more secure and user-friendly alternative, but integrating them seamlessly with Windows can be challenging.  Traditional SSH keys also lack a critical component: device authorization.  Anyone with the key can attempt a login, regardless of the device's legitimacy.

## The Solution: MagicEndpoint FIDO Eazy

MagicEndpoint FIDO Eazy simplifies secure SSH key management on Windows by leveraging FIDO keys, SSH certificates, and optional TPM integration. This approach offers:

* **Passwordless Authentication:** Eliminate password-related risks.
* **Device Binding:** Restrict access to authorized devices only.
* **Centralized Management:** Simplify key management with SSH certificates.
* **Scalability:** Easily manage SSH access for many users and devices.
* **FIDO2 Compliance:** Leverage the security of FIDO2 authenticators.
* **TPM Integration (Optional):** Enhance device binding with TPM.
* **User-Friendly Interface:** Streamlined key generation, management, and backup.
* **Broad Compatibility:** Supports PuTTY-CAC and Microsoft's OpenSSH.

## Key Features and Benefits

* **Automatic FIDO SSH Key Creation:** Easily generate TPM-backed FIDO keys.
* **One-Click Key Creation:** Add more keys as needed.
* **Intuitive Key Management UI:** A user-friendly interface for key management.
* **Seamless Key Backup:** Securely back up your keys.
* **Enhanced Security with ME Client:** Keys are unusable when the user logs out of MagicEndpoint.

## Getting Started

This repository provides:

* **Certificate Generation Tools:** Tools for creating SSH certificates.
* **Key Management Examples:** Scripts and examples for managing keys.
* **FIDO2 Integration Demonstrations:** Examples of using FIDO2 for SSH.

Refer to the [documentation](link-to-documentation) for detailed instructions.

## Contributing

Contributions are welcome! See the [contributing guidelines](CONTRIBUTING.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file.

## Contact

[Your Name/Team] - [Your Email/Contact Information]
