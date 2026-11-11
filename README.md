# FOCUS

A dark, distraction-friendly personal productivity dashboard.

## What's included

- Overview dashboard with task progress and personal stats
- Task list with priorities and completion tracking
- Projects workspace
- Calendar view
- Notes and brain-dump capture
- Habit and goal tracking
- Manual money and savings tracker (AUD)
- Focus timer
- FOCUS AI chat panel with basic local commands
- Floating Waves focus companion with animated visual waveform
- Responsive desktop, tablet and mobile layouts
- Local JSON export

## Run locally

Open `index.html` in a browser, or serve this directory with any static file server.

## Deploy with Cloudflare Pages

1. Open **Workers & Pages** in Cloudflare.
2. Choose **Create application** → **Pages** → **Connect to Git**.
3. Select `joelrobinson952-stack/FOCUS`.
4. Use the `main` branch and **None** as the framework preset.
5. Leave the build command empty and set the build output directory to `/`.
6. Deploy.

Cloudflare Pages will publish the static site and redeploy on new commits.

## Prototype limitations

Data currently lives in this browser's localStorage. This version does not yet provide real user accounts, cross-device sync, secure server-side storage, real LLM-powered AI, bank connections, push notifications or ambient audio playback. The assistant handles a small set of local commands and can update local task/project data.

Before public launch, add secure authentication, a Cloudflare Worker API, D1 database migrations and per-user data isolation. Connect an AI model through a server-side secret and expose only permissioned app actions. Require confirmation for destructive or financial actions. Never put API keys in browser code.
