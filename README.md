<div align="center">
<h1>Crownix Vault</h1>

<p>
    <strong>Secure. Private. Yours.</strong><br />
    A local-first password manager
</p>

<p>
    <a href="https://github.com/tsgamage/crownix-vault-releases/releases">Download</a> ·
    <a href="https://github.com/tsgamage/crownix-vault">Source Code</a> ·
    <a href="https://github.com/tsgamage/crownix-vault/issues">Report an Issue</a>
</p>

<a href="https://github.com/tsgamage/crownix-vault-releases/releases/tag/v1.1.0">
    <img src="https://img.shields.io/badge/version-1.1.0-blue" />
</a>
</div>

Crownix Vault is a modern, local-first password manager built for users who value privacy, transparency, and ownership of their data.
This repository contains **official release builds only**.
The source code is available separately for transparency and review.

---

## About

Crownix Vault is designed around a simple principle: **your secrets should never leave your device**.

Unlike cloud-based password managers, Crownix Vault stores all data locally in a single encrypted vault file. There is no account system, no server, no telemetry, and no background syncing. You decide where your data lives and how it is backed up.

The application is built with **Tauri (Rust backend)** and **React**, providing native performance with a minimal footprint.

---

## Platform Support

- **Windows**: Supported (current)
- **macOS**: In progress
- **Android**: Planned

At this time, Crownix Vault is officially supported **only on Windows**.

---

## Key Features

### Local-First by Design

- All data is stored locally in an encrypted vault file.
- No cloud storage, no remote servers, no tracking.
- Works fully offline (except update checks).

### Strong Cryptography

- **AES-256-GCM** encryption for all vault data.
- **PBKDF2 (SHA-256, 200,000 iterations)** for key derivation.
- Unique random salt per vault.
- Master password is never stored.

### Zero-Knowledge Architecture

- Only you can decrypt your vault.
- The application has no access to your master password or keys.
- No recovery servers and no backdoors.

### Advanced Password Generator & Analysis

- High-entropy password generation with granular controls.
- Detects weak, reused, common, and pattern-based passwords.
- Identifies keyboard walks, repeated characters, sequences, leet substitutions, and date patterns.

### Vault Health Dashboard

- Overall security score for your vault.
- Highlights weak, reused, and risky passwords.
- Designed to encourage measurable security improvements.

### Auto-Lock

- Automatically locks the vault after inactivity.

### Portable Vault File

- Your vault is a single encrypted file you fully own.
- You can back it up, move it, or store it wherever you want.

### Automatic Updates

- The app checks for updates on startup.
- Updates are delivered securely via official releases.

---

## Screenshots

Below are key screens from the application, shown in typical user flow order.

### Create a New Vault

Create a new encrypted vault by choosing a master password and storage location.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/create_new_vault.png" width="80%" />

---

### Unlock Vault

Unlock your vault using your master password. **The password is never stored.**

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/unlock_vault.png" width="80%" />

---

### All Passwords View

View and manage all stored credentials in a clean, searchable list.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/all_passwords_view.png" width="80%" />

---

### Categories View

Organize passwords into categories for better structure.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/categories_view.png" width="80%" />

---

### Security Dashboard

Analyze vault health, weak passwords, reuse, and patterns.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/security_dashboard.png" width="80%" />

---

### Tools Dashboard

Access password, passphrases, OTP, and recovery code generators and password analyzer tool.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/tools_dashboard.png" width="80%" />

---

### Trash

Deleted items are kept in trash and can be restored or permanently removed.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/trash.png" width="80%" />

---

### Vault Locked

The vault locks automatically when idle or manually by the user.

<img src="https://raw.githubusercontent.com/tsgamage/crownix-vault-releases/refs/heads/main/assets/screenshots/vault_locked.png" width="80%" />

---

## Downloads

All official builds are available on the **Releases** page:

[https://github.com/tsgamage/crownix-vault-releases/releases](https://github.com/tsgamage/crownix-vault-releases/releases)

### Windows

- Portable & Installer `.exe`

Checksums are provided with each release.

---

## Security Transparency

Crownix Vault is intentionally designed to be **auditable and transparent**.

- The source code is public for review.
- No network requests are made for vault data.
- No analytics, telemetry, or tracking.
- Encryption logic and password analysis are fully visible in the source code.

This allows users to **verify trust instead of assuming it**.

---

## Roadmap (High-Level)

- macOS support
- Android support
- Optional Google Drive–based vault storage for easy backup and sync (opt-in only)
- UI and accessibility improvements
- Ongoing security hardening

The roadmap may evolve based on feedback.

---

## License

Crownix Vault is released under the Crownix Source-Available License (SAL-1.0).
This means:

- The source code is publicly available for transparency and security review
- You may build and run the software for personal, non-commercial use
- You may not redistribute, modify, fork, or create derivative works
- Commercial use, resale, or rebranding is not permitted
- Third-party distribution of binaries is not allowed

The software is provided “as is”, without any warranty.
Crownix is not responsible for data loss, corruption, or misuse.

See the [`LICENSE`](./LICENSE) file for full terms.

---

## Feedback & Issues

If you encounter bugs or unexpected behavior, please report them here:

[https://github.com/tsgamage/crownix-vault-releases/issues](https://github.com/tsgamage/crownix-vault-releases/issues)

Responsible security reports are appreciated.

---

<div align="center">
  <sub>
    Crownix Vault · Official Release Repository
  </sub>
</div>
