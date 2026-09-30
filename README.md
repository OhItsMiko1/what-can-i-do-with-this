# What Can I Do With This?

A tiny mobile-first web app. Type an item (or snap a photo of it) and get simple ideas in four sections:

- **Keep**: useful ways to hold onto it
- **Repurpose**: creative or practical reuse
- **Sell**: whether it might reasonably be worth selling
- **Donate / Recycle**: practical disposal or donation options

It's one HTML file with no backend, no accounts, and no build step.

## What works out of the box

- A built-in list of about 30 common household items, loaded instantly
- Your own notes for each item
- Photos you attach to an item
- Notes and photos are saved on your device only (`localStorage`)

## Turn on AI (optional)

AI adds two things: it **identifies items from a photo**, and it writes ideas for items that aren't in the built-in list.

1. Get an API key at [console.anthropic.com](https://console.anthropic.com) and set a low monthly spend limit.
2. Open the app, expand **AI settings** at the bottom, paste the key, and tap **Save**.

The key is stored only in your browser and sent only to `api.anthropic.com`. Don't put a key in the code or in this repo. Don't use AI mode on a shared device. If you want to share the app publicly, put the API call behind a small server or serverless function instead of using personal keys.

## Host it free with GitHub Pages

1. In this repo, go to **Settings > Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
3. After a minute your app is live at `https://<your-username>.github.io/<repo-name>/`.

On a phone, open that link and use **Share > Add to Home Screen** to make it feel like an app.

## Files

- `index.html`: the whole app
- `README.md`: this file
