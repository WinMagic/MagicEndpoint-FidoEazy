# MagicEndpoint FIDO Eazy

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

##  👋  Say Goodbye to SSH Key Headaches! 👋

Let's be honest, managing SSH keys the old-fashioned way is a pain.  You know the drill:

* **Generating Key Pairs:**  Wrestling with command lines...  ⌨️
* **Guarding Private Keys:**  Like they're buried treasure... 💰
* **Revoking Access:**  A nightmare when someone leaves the team... 😫
* **Key Sprawl:**  Lost in a sea of keys... 🤯

Traditional SSH keys *are* better than passwords, but they still come with a whole new set of headaches. Plus, if those keys live unprotected on your hard drive, they're still vulnerable.  And here's the kicker – with traditional keys, anyone with access to that key can try to log in, regardless of whether their **device** is authorized.

## ✨  Imagine a Better Way... ✨

Wouldn't it be awesome if there was a simpler, more secure way – one that not only blocked unauthorized *users* but also ensured that only *authorized devices* could connect?

**Good news – there is!** 🎉

We're talking:

* **Passwordless Login:**  No more remembering complex passwords! 🔑
* **Rock-Solid Security:** Thanks to FIDO2 and TPM. 🛡️
* **Streamlined Experience:** So easy, anyone can do it! 🤩
* **Ironclad Device Authorization:**  Only *your* devices get in. 💻📱

## That's what MagicEndpoint FIDO Eazy is all about!  🚀

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

Refer to the [documentation](https://github.com/WinMagic/MagicEndpoint-FidoEazy/blob/main/Documentation.md) for detailed instructions.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file.

## Contact

[Your Name/Team] - [Your Email/Contact Information]
