# Privacy Policy for Tabrok

**Last Updated:** October 2026

Tabrok is a local-first desktop application for running autonomous AI browser agents. This Privacy Policy explains what information the app processes, where it goes, and how you control it.

## 1. Local-First Architecture

Tabrok runs entirely on your Mac. The app consists of a desktop client and a backend service that communicate over a private local channel — a Unix socket with a random, per-launch authentication token. Nothing it does is shared with us by default, and the backend cannot be reached by other apps, devices, or the network.

## 2. Data Stored Locally on Your Device

The following data stays on your machine, under `~/Library/Application Support/Tabrok`:

- **API keys** (Google Gemini, OpenRouter, Mistral, NVIDIA NIM): encrypted at rest using macOS Keychain via Electron `safeStorage`. Keys are never written to disk in plain text, never included in exports, and never leave your machine except as authentication to the model provider you configured.
- **Uploaded files and images**: the files and images you attach to a task or conversation.
- **Browser profiles**: the agent works in its own Chrome profile, stored under `~/.tabrok/google_user_data` (owner-only permissions), so websites you sign into during agent runs stay logged in. This directory contains session cookies for sites you log into and is restricted to your user account.
- **Local logs and crash reports**: used for your own troubleshooting, viewable and clearable in Settings → System.
- **Usage metrics**: anonymous counters (app starts, agent runs, errors) kept in a local JSON file.

## 3. What Is Transmitted, and Where

By default Tabrok does **not** send telemetry to us. The following connections happen as part of normal use:

- **Crash and error reports (Sentry).** Tabrok reports crashes and unhandled errors to Sentry (hosted in the EU) so the developer can diagnose and fix stability problems. These reports contain error messages, stack traces, and app version. They do **not** contain your API keys, task content, or website data — but a stack trace may incidentally include a local file path. This feature is on by default.
- **Model providers you configure.** When you use the AI assistant or the browser agent, your prompts, instructions, and any file contents you attach are sent directly to the LLM provider you selected (OpenRouter, NVIDIA NIM, Mistral, or Google Gemini) using your own API key. The websites the agent visits see the same activity a person browsing them would.

Tabrok does not send your data to any other server. There is no analytics SDK, no advertising tracker, and no first-party telemetry server.

## 4. What Tabrok Never Does

- Your API keys are never written unencrypted, never logged, and never included in exported archives.
- Your logged-in website sessions are never transmitted to the developer.
- Your prompts, tasks, and files are never used to train models or shared with third parties beyond the providers listed above.

## 5. Your Control and Data Deletion

You can:

- **Export your user data** (Settings → System → Export). The export contains only your uploaded files — credentials, encrypted keys, browser sessions, and cookies are structurally excluded.
- **Delete all local data** (Settings → System → Delete Data). This removes the app's data folder, your API keys from encrypted storage, legacy data folders, and saved browser profiles, then restarts the app.
- **Fully uninstall** via the "Uninstall Tabrok" app included in the DMG (Touch ID protected), which removes the application bundle and all associated data.

## 6. Changes to This Policy

Material changes will be noted in release notes and reflected in this document's revision date.

## 7. Contact

For privacy questions, or to submit a crash report archive for support, contact the developer directly via the support channel listed on the project's website.
