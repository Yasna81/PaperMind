# PaperMind 📄✦

A mobile-friendly AI-powered academic paper reader. Search PubMed for recent publications, get instant AI insights, and chat with any paper, all from your phone browser.

**[→ Open PaperMind](https://yasna81.github.io/PaperMind/)**
---



<img width="556" height="483" alt="image" src="https://github.com/user-attachments/assets/1e564379-b2e5-4357-bae5-fa8a217c6548" />







## Features

- **PubMed Search** — search by keywords and filter by relevance or date (2022+), up to 30 results
- **Abstracts loaded automatically** for all results in one batch
- **Clickable titles** — each paper links directly to its PubMed page
- **✦ Novelty · Key Findings · Open Doors** — one tap generates a single AI paragraph covering what's new, what was found, and what research it opens up
- **💬 Chat** — open any paper into a full chat interface and ask anything
- **PDF / text upload** — upload your own papers or paste text
- **Quick actions** — Summary, Methods, ELI5, Critique, Citation with one tap
- **Multiple AI models** via OpenRouter — DeepSeek, Gemini, Claude, GPT-4o, and free-tier options

---

## Getting Started

### 1. Get an OpenRouter API key
Sign up at [openrouter.ai](https://openrouter.ai) and grab your key from [openrouter.ai/keys](https://openrouter.ai/keys).

### 2. Use it
Option A — **GitHub Pages (recommended for mobile):**
1. Fork or clone this repo
2. Enable GitHub Pages in Settings → Pages → source: `main` branch, `/ (root)`
3. Visit `https://YOUR-USERNAME.github.io/papermind/` on your phone
4. Tap ⚙ Settings, paste your OpenRouter key, choose a model, save

Option B — **Local use:**
Just open `index.html` directly in any browser. No server needed.


Note : make sure to save api setting and test your keys before searching.


<img width="353" height="248" alt="image" src="https://github.com/user-attachments/assets/da2b3574-7ace-4ef5-bc9c-e6a7b2d24b7c" />


---

## Privacy

- Your API key is stored **only in your browser's localStorage** — it never touches any server except OpenRouter's API directly
- Paper text is sent to OpenRouter (and the model you choose) only when you trigger an AI action
- PubMed searches go directly to NCBI's public API — no intermediary

---

## Stack

Pure HTML + CSS + JavaScript. No frameworks, no build step, no dependencies to install. One file.

- **[PubMed E-utilities API](https://www.ncbi.nlm.nih.gov/books/NBK25499/)** — free, no key required
- **[OpenRouter API](https://openrouter.ai/docs)** — unified API for 100+ LLMs
- **[PDF.js](https://mozilla.github.io/pdf.js/)** — loaded from CDN on demand for PDF parsing

---

## Deploying to GitHub Pages

```bash
git clone https://github.com/YOUR-USERNAME/papermind.git
cd papermind
# 
mv paper-reader.html index.html
git add .
git commit -m "Initial commit"
git push
```

Then go to your repo → **Settings → Pages → Branch: main → Save**.
Your app will be live at `https://YOUR-USERNAME.github.io/papermind/` in ~1 minute.

---

## License

MIT
