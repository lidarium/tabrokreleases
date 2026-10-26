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

By default, Tabrok does **not** transmit telemetry or crash reports to us or any third party. The following network connections happen during normal use:

- **Crash and error diagnostics (Sentry — strictly opt-in).** If you explicitly choose to enable crash telemetry in the first-run license dialog or in Settings → System, Tabrok reports unhandled errors and crashes to Sentry (hosted in the European Union) so stability problems can be diagnosed and resolved.
  - **What is sent:** Error messages, stack traces, application version, release channel, and session-health indicators (such as application start and clean shutdown signals).
  - **What is not sent:** Your API keys, prompts, instructions, uploaded files, task contents, visited URLs, web browsing sessions, or cookies.
  - **Incidental personal data:** We do not claim that no personal data is transferred. An error stack trace can incidentally include local file system paths (for example, containing your macOS username), which constitutes personal data under applicable data protection laws.
  - **Legal basis:** Processing is based solely on your explicit, freely given, and revocable consent under Section 6 of the Digital Personal Data Protection Act, 2023 (DPDP Act) and Article 6(1)(a) of the General Data Protection Regulation (GDPR).
  - **Retention period:** Telemetry data received by Sentry is retained for 90 days (standard retention cycle) and is automatically and permanently purged thereafter.
  - **Consent withdrawal:** Sentry reporting is **off by default**. You can enable or withdraw your consent at any time via Settings → System → Crash & Error Telemetry. Withdrawal takes effect immediately at runtime, halts the telemetry client, and clears pending transmissions. Local crash files remain saved on your Mac under `~/Library/Application Support/Tabrok/crashes` for your own troubleshooting regardless of consent status.
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

## 7. General Inquiries & Support

For general technical support, commercial inquiries, or licensing questions, contact `legal@lidarium.com` or visit https://lidarium.com.

## 8. Grievance Officer & Grievance Redressal Mechanism

In compliance with the Digital Personal Data Protection Act, 2023 (DPDP Act, 2023) and Rule 3(2) of the Information Technology (Intermediary Guidelines and Digital Media Ethics Code) Rules, 2021, this section sets forth the statutory grievance redressal mechanism for Data Principals.

### 8.1. Data Fiduciary & Grievance Handling Entity

Grievances are administered directly by the Data Fiduciary:

**M/s TERALIDARIUM WORKS (an Udyam-registered sole proprietorship firm existing under the laws of India)**  
As defined at `LICENSE` §1.1. In accordance with the firm's constitution, the statutory Udyam registration certificate and the natural-person identity of the sole proprietor are maintained privately and shall be disclosed upon written request for the purpose of legal notice, formal proceedings, or a dispute. No individual personal name is published herein; statutory notices and communications are received and acted upon through the designated institutional grievance address.

### 8.2. Contact Channel & Response Timelines

- **Designated Grievance Email:** `legal@lidarium.com`
- **Acknowledgement Commitment:** Every grievance or notice received will be acknowledged within **twenty-four (24) hours** of receipt.
- **Resolution Commitment:** Grievances will be investigated and resolved within **thirty (30) days** from the date of receipt.

### 8.3. Scope of Grievances Accepted

The Grievance Officer accepts communications and requests from Data Principals regarding:
1. **Right to Access:** Information regarding personal data processed or shared by the application.
2. **Right to Correction & Updating:** Correction, completion, or updating of inaccurate or misleading personal data.
3. **Right to Erasure:** Deletion of personal data maintained by the Data Fiduciary or third-party processors (such as Sentry).
4. **Consent Withdrawal:** Revocation of consent previously provided for crash or error reporting.
5. **Objection & Grievance Redressal:** Any complaint regarding non-compliance with data protection obligations or handling of personal data.

### 8.4. Escalation to the Data Protection Board of India

If a grievance is not redressed within thirty (30) days, or if you are dissatisfied with the resolution provided by the Data Fiduciary, you have the statutory right under the Digital Personal Data Protection Act, 2023 to file a complaint before the **Data Protection Board of India (DPBI)** in accordance with the rules and procedures prescribed under the Act.
