# Atlas desktop downloads

Atlas is a personal knowledge workspace with graph and hex-tile visualizations, an offline-first artifact library, research discussions, and revision-based Understanding documents.

**[Download Atlas 0.2.0 for Apple Silicon Macs](https://github.com/ethanyanjiali/frontier-atlas-downloads/releases/tag/v0.2.0)**

This public repository contains downloads and release notes. The application's development repository is private. No personal library, API keys, or account sessions are included.

## Install the preview

- Requires an Apple Silicon Mac (M1 or newer), macOS 13 or newer.
- Download `Atlas-0.2.0-mac-arm64.zip` from the release's **Assets**, unzip it, and move Atlas.app into Applications.
- Quit any older Atlas instance before opening the new app. The browser development server also uses port 4173; stop it before starting the desktop backend.
- This preview is **not Developer ID signed or notarized**. macOS may block its first launch. After checking the source of your download, use macOS System Settings → Privacy & Security → Open Anyway if offered. Managed computers may prevent this; a signed build is not available yet. Do not disable Gatekeeper globally.
- First launch is a single setup page. Open your existing Atlas Data directory containing `atlas.json`, or create a new library. Choose a model provider and enter your own credentials.
- Later, use the floating Settings gear in the visualizer or Cmd+, to change the library/provider. Settings have Library and LLM provider tabs.

## Models and private providers

Built-in options: Codex/ChatGPT sign-in, OpenAI API, OpenRouter, Muse (Meta Model API), Claude (Anthropic API), and Gemini (Google API). API subscriptions/billing and model availability belong to the selected provider; there is no automatic billing-provider fallback. Codex requires a separately installed, signed-in Codex CLI.

Choose a **Main model** for discussions and Understanding, and a **Background model** for titles, summaries and small tasks. Dropdowns load provider catalogs when possible, with suggested defaults and custom model IDs as a fallback. Listing a model does not guarantee support for every Atlas feature. API credentials remain OS-encrypted on this computer, outside the portable library.

Settings can export a readable provider developer kit with an agent guide, typed feature contracts, an executable adapter scaffold, and offline verification. Install only trusted plugins: they execute local code and receive their provider's prompts and credentials.

## Storage and limitations

Choose a local folder, or a folder managed by iCloud Drive/Google Drive. Use one writing device at a time and wait for synchronization before switching computers. Keep a backup of your library. Credentials are configured separately on each computer.

This is an early desktop preview. The browser capture extension's desktop authentication/wake integration is not implemented yet. Mobile, Windows/Intel binaries, automatic updates, signing/notarization, and simultaneous multi-device conflict resolution are not included.

The application is distributed as packaged software, not as an open-source project. Runtime JavaScript is minified, but a locally installed Electron application can still be inspected. Third-party components retain their respective licenses.
