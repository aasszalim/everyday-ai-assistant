# Everyday AI Cyber Safety

A small, browser-based companion for defensive cybersecurity guidance. Get help with account recovery, suspicious messages, compromised accounts, device hardening, and everyday security questions.

## Try it

[Open the live app](https://aasszalim.github.io/everyday-ai-assistant/) or open `index.html` directly in a browser.

## Connect a provider

1. Open **API settings** and choose Google Gemini, Anthropic Claude, or OpenAI-compatible / other.
2. Enter the provider's API endpoint, model ID, and your own API key. The app suggests a default endpoint for each provider.
3. Save settings for this browser tab session, choose a cybersecurity topic, describe the situation without secrets, and select the action button.

Custom providers must use the OpenAI Chat Completions format. Requests go directly from your browser to the selected provider, so the endpoint must allow browser requests (CORS). The provider may charge for API use. API keys are kept in this tab's `sessionStorage`; use the **Forget** button to remove saved settings.

## Safety and privacy

Never paste passwords, one-time codes, recovery codes, private keys, session cookies, or payment details. For password/account recovery, the app gives guidance for official provider recovery flows; it does not retrieve passwords or bypass authentication. For suspicious messages, defang URLs and remove personal details before pasting. The app does not save your descriptions, but sends them to the AI provider you configured. Check that provider's data policy and verify recovery instructions on its official website.

## Development

This is a dependency-free static HTML app. Edit `index.html` and reload it in a browser. No build step is required.
