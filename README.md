# Tabrok Releases

Official distribution repository for **Tabrok** — the local-first Autonomous AI Browser Agent for macOS.

Describe any web task in plain language, and a real browser on your machine carries it out, step by step, while you watch.

---

## 📥 Download

| Release | Version | macOS Compatibility | Package | Release Notes |
| :--- | :--- | :--- | :--- | :--- |
| **Latest Beta** | `26.299.719-beta` | macOS 12+ (Intel x86_64 — runs on Apple Silicon via Rosetta 2) | [**Download Tabrok-26.299.719-beta.dmg** (202 MB)](https://github.com/lidarium/tabrokreleases/releases/download/v26.299.719-beta/Tabrok-26.299.719-beta.dmg) | [v26.299.719-beta](https://github.com/lidarium/tabrokreleases/releases/tag/v26.299.719-beta) |

**SHA-256 Checksum:**
```text
ed4f1b55b022c190e706d2f20637f8e8d92297a68e00055f8e131c447dce9d4c  Tabrok-26.299.719-beta.dmg
```

You can view all past and future releases on the [**GitHub Releases Page**](https://github.com/lidarium/tabrokreleases/releases).

---

> [!IMPORTANT]
> ### 🚨 macOS Beta Installation & Gatekeeper Workaround
> Because Tabrok is in public beta and signed ad-hoc (without Apple Developer ID notarization), macOS Gatekeeper will block the application on first launch with a warning such as:
> - *"Tabrok is damaged and cannot be opened. You should move it to the Trash."*
> - *"macOS cannot verify that this app is free from malware."*
>
> Follow either method below to launch the app:
>
> #### 🔹 Method 1: One-Line Terminal Command (Fastest & Recommended)
> 1. Drag **Tabrok.app** from the `.dmg` into your **/Applications** folder.
> 2. Open your Mac's **Terminal** (`Cmd + Space`, type `Terminal`, hit `Enter`).
> 3. Paste and run this command:
>    ```bash
>    xattr -cr /Applications/Tabrok.app
>    ```
> 4. Double-click **Tabrok** in `/Applications`. It will now launch immediately without warnings.
>
> ---
>
> #### 🔹 Method 2: macOS System Settings
> 1. In Finder, open your **/Applications** folder.
> 2. **Right-click** (or `Control + click`) on **Tabrok.app** and click **Open**.
> 3. If macOS blocks it, open **System Settings** -> **Privacy & Security**.
> 4. Scroll down to the **Security** section where you will see:
>    > *"Tabrok was blocked from use because it is not from an identified developer."*
> 5. Click **Open Anyway** and authenticate with Touch ID or your Mac password.

---

## Security & Privacy Highlights

* **Zero Secret Bundling**: No API keys, credentials, or private tokens are baked into the distributed app.
* **Encrypted Local Storage**: User API keys (Google Gemini, Mistral, NVIDIA NIM, OpenRouter) are encrypted at rest using Apple Keychain / Electron `safeStorage`. Keys never leave your machine and are never written in plain text.
* **Locked-Down Backend**: The backend binds only to a Unix domain socket (`/tmp/tabrok.sock`) protected by a per-launch authentication token.
* **Process Isolation**: The browser automation engine runs in an isolated user data directory (`~/.tabrok/google_user_data`).

For full details, please review our [Privacy Policy](./PRIVACY_POLICY.md).

---

## Legal & Licensing

* **License**: Tabrok is proprietary software licensed under the [Tabrok Proprietary Software License](./LICENSE). Free for personal use.
* **Privacy Policy**: [PRIVACY_POLICY.md](./PRIVACY_POLICY.md)
* **Third-Party Notices**: Tabrok includes components from open-source software. Full notices and licenses are documented in [THIRD-PARTY-NOTICES.md](./THIRD-PARTY-NOTICES.md) and [THIRD-PARTY-LICENSES/](./THIRD-PARTY-LICENSES/).
