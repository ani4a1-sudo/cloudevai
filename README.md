# CloudevAI — Cloud AI Assistant

> Your cloud problems, solved in seconds.

**CloudevAI** is a specialist AI tool built exclusively for cloud engineers and DevOps teams. Not a general AI — a dedicated cloud expert available 24/7 that speaks your language and gets straight to the answer.

---

## 🌐 Live Website
[cloudevai.com](https://cloudevai.com)

---

## ✨ Features

- ☁️ **Multi-cloud support** — AWS, Azure and GCP in one place
- 🏗️ **Architecture diagrams** — Generate, edit and download professional diagrams
- ⚙️ **Terraform & IaC** — Production-ready infrastructure code
- 💻 **Copy-ready commands** — Every CLI command has a one-click copy button
- 🔒 **Security first** — Credential exposure alerts built in
- 🌙 **Light & dark mode** — Clean minimal design
- 📋 **Chat history** — All conversations saved locally
- 🔄 **CI/CD diagrams** — Sequence diagrams for pipelines

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, JavaScript (ES6+) |
| Diagrams | Mermaid.js |
| Fonts | Geist, Geist Mono (Vercel) |
| AI Engine | Claude API (Anthropic) |
| Backend | Node.js Serverless Function |
| Hosting | Netlify / Vercel |

---

## 📁 Project Structure

```
cloudevai/
├── index.html                    # Main website (HTML + CSS + JS)
├── netlify.toml                  # Netlify configuration
├── netlify/
│   └── functions/
│       └── chat.js               # Serverless function (hides API key)
├── docs/
│   └── CloudHelper-AI-Troubleshooting-Docs.txt  # Knowledge base
└── README.md                     # This file
```

---

## 🚀 How It Works

```
User asks a question
        ↓
Website sends request to Netlify Function
        ↓
Function adds API key (from environment variable)
        ↓
Sends to Anthropic Claude API
        ↓
Answer returned to user
        ↓
API key never exposed in browser ✅
```

---

## ⚙️ Setup & Deployment

### Prerequisites
- Anthropic API key (from console.anthropic.com)
- Netlify or Vercel account (free)
- Namecheap or any domain registrar

### Deploy Steps

**Step 1 — Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/cloudevai.git
cd cloudevai
```

**Step 2 — Add your API key**

On Netlify:
```
Site Settings → Environment Variables
Key: ANTHROPIC_API_KEY
Value: your-api-key-here
```

**Step 3 — Deploy**
```
Drag and drop project folder to Netlify
OR connect GitHub repo to Vercel
```

**Step 4 — Connect your domain**
```
Add cloudevai.com in Vercel/Netlify
Update DNS on Namecheap
Wait 24 hours for propagation
```

---

## 🔒 Security

- API key stored in environment variable — never in code
- Netlify Serverless Function acts as proxy
- Credential exposure detection built into AI prompt
- No user data stored on any server
- Chat history stored only in user's browser (localStorage)

---

## 📋 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `ANTHROPIC_API_KEY` | Your Anthropic API key | ✅ Yes |

---

## 🗺️ Roadmap

### V1 (Current — Beta)
- [x] Multi-cloud troubleshooting
- [x] Architecture diagram generation
- [x] Terraform code generation
- [x] CLI commands with copy buttons
- [x] Dark/light mode
- [x] Chat history
- [x] About section

### V2 (Coming Soon)
- [ ] Custom domain (cloudevai.com)
- [ ] PDF export
- [ ] Feedback system
- [ ] Voice input
- [ ] Multi-language support
- [ ] User authentication

---

## ⚠️ Disclaimer

CloudevAI is an independent educational tool. Not affiliated with, endorsed by or officially connected to Amazon Web Services, Microsoft Azure or Google Cloud Platform. All guidance is for educational purposes only. Always verify with official documentation before implementing in production environments.

---

## 👨‍💻 Built By

**Anirudh Jagannadh**

Built CloudevAI from scratch with zero prior coding experience. From idea to live product in a few days — powered by determination and Claude AI.

---

## 📄 License

MIT License — feel free to learn from this code.
