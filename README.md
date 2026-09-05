# Polybot Cloud 🌐

**The 24/7 Web & Mobile Control Plane for Polybot AI Agents.**

Polybot Cloud is the responsive companion web application for [Polybot](https://github.com/tejasundeep/polybot). Monitor your AI bot fleet, track 24/7 background routines, review action approvals on your phone, and chat with your agents from anywhere.

---

## 🚀 1-Click Deploy to Cloud

Deploy the web control plane in seconds with zero terminal setup:

### Deploy with Vercel (Recommended)
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Ftejasundeep%2Fpolybot-cloud&env=POLYBOT_RUNNER_URL,POLYBOT_AUTH_TOKEN)

### Deploy with Netlify
[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/tejasundeep/polybot-cloud)

### Deploy with Railway
[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/template?template=https%3A%2F%2Fgithub.com%2Ftejasundeep%2Fpolybot-cloud)

### Deploy with Render
[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/tejasundeep/polybot-cloud)

---

## ⚙️ Environment Variables

When deploying, configure the following environment variables (or configure them directly in the UI via the **Runner Config** button):

| Variable | Description | Default |
| :--- | :--- | :--- |
| `POLYBOT_RUNNER_URL` | The HTTP/HTTPS endpoint of your Polybot Harness Runner (e.g. `http://localhost:8799` or your VPS/Fly.io URL) | `http://localhost:8799` |
| `POLYBOT_AUTH_TOKEN` | Bearer token secret matching `PSB_AUTH_TOKEN` on your runner (optional for local testing) | *(empty)* |

---

## ✨ Features

* 📱 **Mobile & Desktop First** — Access your agent team from any phone browser (iOS Safari, Android Chrome) or desktop.
* ⚡ **24/7 Autonomous Routines 2.0** — Monitor recurring schedules, view deliverables, check countdown timers, and trigger runs on demand.
* 🛡️ **Remote Governance Approvals** — Review and approve sensitive commands or tool calls with 1 click from your phone.
* 🤖 **Bot Fleet Overview** — View all registered bots (Claude, Grok, Codex, Antigravity), assigned models, and live telemetry.
* 💬 **Live Chat** — Send prompts and converse with any bot in real time.
* 🔒 **Zero-CORS Proxy Gateway** — Built-in Next.js Route Handlers transparently relay requests to remote runners securely.

---

## 💻 Local Development

```bash
# Clone the repository
git clone https://github.com/tejasundeep/polybot-cloud.git
cd polybot-cloud

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

By default, Polybot Cloud connects to `http://localhost:8799`. Ensure your Polybot harness runner is running (`pnpm dev:server` in the `polybot` repo).
