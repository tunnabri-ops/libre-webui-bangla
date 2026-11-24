# 💬 libre-webui-bangla

[![AI Chat](https://img.shields.io/badge/type-ai%20chat-blue)](https://github.com/tunnabri-ops/libre-webui-bangla)
[![Language](https://img.shields.io/badge/UI-Bangla%20%2B%20English-orange)](https://github.com/tunnabri-ops/libre-webui-bangla)

**Bangla AI chat on your own machine — local models with Ollama, plus Groq, OpenRouter, Gemini, Mistral and DeepSeek, with a free no-key fallback.**

> বাংলা সংস্করণ নিচে আছে। / Bangla version below.

## ✨ Features

- **One-command install** — `docker-compose.yml` runs Ollama (`:11434`) and the chat UI (`:3000`) together
- **Providers** (see `bangla-config.json`): Ollama (no key, local), Groq, OpenRouter, Gemini, Mistral, DeepSeek
- **Bangla UI** — Bangla interface flag in the config
- **Free no-key fallback** — `text.pollinations.ai`, used only when you explicitly select it in Settings

## 🚀 How to use

```bash
docker compose up -d
```

Then open http://localhost:3000 and pull a model:

```bash
docker exec -it <ollama-container> ollama pull qwen2.5:7b
```

## ⚠️ Honest limits

- Needs Docker and a server — it will **not** run as a static GitHub Pages site.
- The Docker-socket Work sandbox stays **disabled by default** — it is root-equivalent host control, so do not enable it casually.

## 🇧🇩 বাংলা

**লিব্রে ওয়েবইউআই বাংলা — নিজের কম্পিউটারে বাংলা AI চ্যাট।**

- `docker compose up -d` চালিয়ে http://localhost:3000 খুলুন
- লোকাল মডেল (Ollama) অথবা Groq / OpenRouter / Gemini — নিজের কী ব্যবহার করুন
- ফ্রি fallback শুধু আপনি নিজে সিলেক্ট করলেই চলবে

## 📄 License

MIT — use it however you like; credit is appreciated.
