---
title: Supercharging My Workflow with Hermes Agent
date: 2026-07-15 09:20:00 -0300
categories: [documentation,ai]
tags: [hermes,agent,automation,ai]
---

# Enter the Agent Era

I've been experimenting with [Hermes Agent](https://github.com/NousResearch/hermes-agent) by Nous Research — an open-source AI agent framework that runs in the terminal, Discord, Telegram, and pretty much anywhere you want it. And honestly? It's been a game changer.

## What I've Built So Far

In just a few sessions, Hermes helped me:

- **Set up a Discord gateway** — so I can talk to my AI from anywhere, even on my phone while grabbing coffee. It's connected to my home server and responds in Portuguese (my native language).

- **Deploy local LLMs** — I've got a Qwen 2.5 3B running on an old GTX 1050 Ti via llama.cpp, and a smaller LFM 2.5 1.2B Thinking model for lightweight tasks. Both sit behind a local API, ready to serve.

- **Create a photography exhibition SPA** — a full dark-themed gallery site called *LUMEN* with AI-generated photos, complete with a lightbox, keyboard navigation, and nginx reverse proxy. Built and shipped in under an hour.

- **Revive my personal blog** — fixed broken drafts, swapped Twitter for Instagram, and generated a fresh avatar — all through the agent.

## Why Hermes Over Other Tools?

I've used ChatGPT, Claude, and Copilot. They're great. But Hermes is different in a few key ways:

| Feature | Hermes | Typical AI Chat |
|---------|--------|-----------------|
| **Persistent memory** | Remembers preferences, environment, past projects across sessions | Forgets everything when you close the tab |
| **Self-learning skills** | Saves reusable procedures as skills — gets better over time | Starts from scratch every conversation |
| **Multi-platform** | Same agent on Discord, Telegram, WhatsApp, CLI, desktop | Usually locked to one interface |
| **Full system access** | Reads files, runs commands, edits code, manages services | Sandboxed, no real access |
| **Provider-agnostic** | Swap between DeepSeek, Claude, local models mid-conversation | Locked to one provider |

## The Real Magic: Skills & Memory

The killer feature is that Hermes *learns*. After fixing a tricky issue — like figuring out nginx permissions or getting `gh` CLI to authenticate properly — it saves the approach as a skill. Next time I hit a similar problem, it already knows the drill.

It also remembers that I speak Portuguese, that my server runs on `192.168.0.11`, that I prefer nginx over Caddy, and that my GPU is a humble GTX 1050 Ti with 4GB of VRAM. I never have to repeat myself.

## What's Next

I'm planning to:

- Hook up Telegram as a second messaging channel
- Try the multi-agent kanban board for project management
- Set up cron jobs for automated daily summaries
- Experiment with voice mode via Discord

If you're curious, the project is fully open-source. Give it a spin:

```bash
curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash
hermes
```

The agent era is here — and it runs on a dusty home server in Fortaleza.
