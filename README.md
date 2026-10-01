# Screen Squirrel releases

Downloads for **Screen Squirrel**, a small, friendly squirrel that lives on your Windows desktop. No account, no ads, no analytics. This repository holds only installers and release notes.

Get the latest installer from [Releases](https://github.com/TOFLeah/screen-squirrel-releases/releases/latest): download the `…_x64-setup.exe` file (for example `Screen.Squirrel.v2_0.2.1_x64-setup.exe`) and run it. It installs for your user only, with no admin prompt.

For the original **v1** build (offline only, no chat), use the [v1.0.1 release](https://github.com/TOFLeah/screen-squirrel-releases/releases/tag/v1.0.1) instead of Latest.

## "Windows protected your PC"

The app isn't code-signed yet, so Windows SmartScreen may say the publisher is unknown. Choose **More info**, then **Run anyway**. The app doesn't phone home, and it has no auto-updater.

## What it does

- Wanders along the bottom of your screen, sits, looks around, naps when left alone, and sometimes hops onto the top of the window you're using.
- Click it for a line, drag it anywhere, right-click it for a menu. The tray icon has Settings, Pause, and Quit.
- Reminders: the squirrel chirps and shows them in its speech bubble, with Done and Snooze.
- Optional chat, off by default: a model on your PC (Ollama or LM Studio), or your own key for OpenAI, Anthropic, Google Gemini, OpenRouter, Groq, Mistral, DeepSeek, xAI, Together AI, or any OpenAI-compatible server.

## What goes over the network

| Setting | What the app connects to |
|---|---|
| Chat off (default) | Nothing |
| Chat with Ollama or LM Studio | Only `localhost` on your PC |
| Chat with an online provider | Only that provider's API, with your key |
| "Check for a new version" (off by default) | `api.github.com`, to read the latest version number here |

Settings and chat history stay in `%APPDATA%\online.plaiground.screensquirrel.v2`. API keys are kept in Windows Credential Manager. Uninstalling with **Delete the application data** ticked removes all of it.
