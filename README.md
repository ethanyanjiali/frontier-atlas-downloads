# Atlas desktop downloads

Atlas is a personal knowledge workspace with graph and hex-tile visualizations, saved sources, research discussions, and revision-based Understanding documents.

**[Download Atlas 0.5.2 for Apple Silicon Macs](https://github.com/ethanyanjiali/frontier-atlas-downloads/releases/tag/v0.5.2)**

This repository contains downloads and release notes only. Development source remains private. No personal library, API keys or account sessions are included.

## Install or update

- Apple Silicon Mac (M1 or newer), macOS 13 or newer.
- Download `Atlas-0.5.2-mac-arm64.zip` from release Assets and unzip it. Install Atlas.app in Applications, or replace your existing Atlas.app at its current location after quitting it.
- Existing data stays in your chosen library folder. Settings, credentials and provider plugins stay in the installation profile. Do not delete your library or uninstall the profile when replacing the app.
- This build is **not Developer ID signed or notarized**. macOS may block first launch. After verifying your download, use System Settings → Privacy & Security → Open Anyway if offered. Managed computers may prevent launch. Do not disable Gatekeeper globally.
- First launch: open the Data folder containing `atlas.json`, or create a library. Choose a model provider and enter your own credentials. On another computer, configure credentials again and import a library archive from Settings → Library if needed.
- Later: use the Settings gear or Cmd+, for Library, LLM provider and App settings. File → New window opens another window; each can select a different graph.

Atlas 0.5.0 checks public releases once on launch outside developer mode. Settings → App offers checks, release notes, progress/cancellation and verified downloads. The unsigned build requires manual app replacement; a restart alone does not install an update. Older versions need a manual download of 0.5.0 first. Desktop backends use dynamic ports, so a browser development server need not be stopped unless it is writing the same graph.

## Providers and integration

Built-in choices: Codex/ChatGPT sign-in, OpenAI, OpenRouter, Muse (Meta Model API), Claude and Gemini. Billing and model availability belong to the chosen provider; there is no automatic billing-provider fallback. Codex needs a separately installed, signed-in Codex CLI. Main/background model selectors use available catalogs with custom IDs as a fallback. Credentials remain OS-encrypted on this computer.

Settings → App exports an integration developer kit: provider contracts/scaffold/tests plus an independent Inbox URL producer for iCloud, Google Drive or local managed folders. Install only trusted model plugins: they execute local code and receive their configured prompts/credentials.

## Phone and Chrome sharing

Settings → Library contains the one-time iPhone Shortcut guide. It writes a URL into a fixed per-graph Inbox folder without asking for a path on every share. Desktop Atlas must be running to collect. Review pending captures in Workspace → Inbox, then Keep or Discard. Reading does not publish the artifact.

The optional [Chrome Capture 0.5.1 ZIP](https://github.com/ethanyanjiali/frontier-atlas-downloads/releases/tag/chrome-v0.5.1) is available separately. Open Atlas once and Load unpacked from the extracted atlas-chrome-capture-0.5.1 folder. The extension identity is unchanged from 0.3.0. It saves into the desktop app and wakes it when closed. No localhost browser tab is required. Windows native-host integration and Chrome Web Store updates are not included.

## Storage and limits

Use a local library or a folder managed by iCloud Drive/Google Drive. Use one writing computer at a time, wait for synchronization before switching, and keep backups. Export/import transfers selected graphs and their content; it does not transfer credentials or plugins. Inbox v1 accepts URL envelopes, not arbitrary local files. Raw audio transcription and a mobile Atlas app remain outside this release.

Windows/Intel builds, signed automatic installation and simultaneous multi-device conflict resolution are not included. Runtime JavaScript is minified but Electron applications can be inspected. This packaged distribution is not an open-source license grant; third-party components retain their licenses.
