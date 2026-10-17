# Everyday AI

A small writing studio for drafting, refining, translating, and summarizing text. Runs as a static page; no account or server required.

## Try it

Open [index.html](./index.html) in a browser, or enable GitHub Pages in **Settings → Pages** and publish from the `main` branch, `/ (root)`.

## Connect an AI provider

1. Select **API settings**.
2. Enter an OpenAI-compatible API endpoint, a model name, and your API key. For OpenAI, the endpoint is `https://api.openai.com/v1`.
3. Save for this session, write a brief or paste text, choose Draft, Refine, Translate, or Summarize, then select **Generate**.

The browser sends requests directly to the provider. The API key is stored in this tab's `sessionStorage` only and is cleared when the tab session ends. Your provider may charge for API usage. The endpoint must allow browser requests (CORS). Do not enter a private key on a shared device or share a browser session containing your key.

## Privacy

Text is not saved by this app or sent anywhere except the AI endpoint you configure. Review that provider's data policy before sending sensitive content. AI output can be inaccurate; check it before relying on it.

## Development

This is a dependency-free static HTML app. Edit `index.html` and reload it in a browser to test changes. No build step is required.
