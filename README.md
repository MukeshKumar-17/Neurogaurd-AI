# ⚡ NeuroGuard AI — Agentic AI Platform

A full-stack platform to **build, deploy, and manage custom AI agents** with LangGraph workflows, Groq LLMs, optional RAG over your documents, and per-agent API keys — everything you need for production-grade agent infrastructure.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen.svg)
![Frontend](https://img.shields.io/badge/frontend-HTML%20%2F%20CSS%20%2F%20JS-orange.svg)

---

## 🚀 Features

| Feature | Description |
|---|---|
| **AI Agent Creation** | Define models, prompts, memory, and RAG in a guided flow with instant provisioning |
| **API Key Generation** | Cryptographically strong keys with prefix display, rotation, and validation on every call |
| **LangGraph Workflows** | Planner → retrieval → reasoning pipelines with clean state management and observability hooks |
| **RAG Integration** | Upload PDFs, chunk, embed with MiniLM, and serve FAISS-backed context to your agents |
| **Multi-Agent System** | Architecture-ready for supervisor patterns, handoffs, and coordinated specialist agents |
| **Groq LLM Support** | Low-latency inference with dynamic model routing across Llama, Qwen, DeepSeek, and more |
| **Real-time Chat** | Session-based chat interface with typing indicators, agent memory, and JWT authentication |
| **Dashboard Analytics** | Interactive analytics cards, usage trends, and agent management in a polished console UI |

---

## 📁 Project Structure

```
Neurogaurd/
├── frontend/
│   ├── index.html          # Landing page — features, preview, CTA
│   ├── login.html          # User login
│   ├── register.html       # User registration
│   ├── dashboard.html      # Dashboard — stats, charts, agent overview
│   ├── chat.html           # Real-time chat with AI agents
│   ├── create-agent.html   # Agent creation wizard
│   ├── agents.html         # Agent management — edit, delete, rotate keys, RAG upload
│   └── static/
│       ├── css/
│       │   └── styles.css  # Design system — tokens, components, layouts
│       └── js/
│           ├── core.js     # Auth, API helpers, shared utilities
│           └── ui.js       # UI interactions — sidebar, ripple, toasts
├── README.md
└── LICENSE
```

---

## 🛠️ Tech Stack

### Frontend
- **HTML5** — Semantic markup with accessibility (ARIA) support
- **CSS3** — Custom design system with CSS variables, glassmorphism, responsive grid
- **Vanilla JavaScript** — Zero framework dependencies, async/await API layer
- **Chart.js** — Interactive usage trend charts
- **Google Fonts** — Inter + Poppins typography
- **Font Awesome 6** — Icon system

### Backend (API)
- **LangGraph** — Stateful agent workflow orchestration
- **Groq** — Low-latency LLM inference (Llama 3, Qwen, DeepSeek)
- **FAISS** — Vector similarity search for RAG
- **MiniLM** — Sentence embeddings for document chunking
- **MongoDB** — Data persistence
- **JWT** — Authentication & session management

---

## 🏁 Getting Started

### Prerequisites
- A modern web browser
- A backend server running the API endpoints (see API routes below)

### Running Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/MukeshKumar-17/Neurogaurd-AI.git
   cd Neurogaurd-AI
   ```

2. **Serve the frontend**
   You can use any static file server:
   ```bash
   # Using Python
   cd frontend
   python -m http.server 8000

   # Using Node.js (npx)
   npx serve frontend
   ```

3. **Open in browser**
   ```
   http://localhost:8000
   ```

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/register` | Register a new user |
| `POST` | `/api/auth/login` | Login and receive JWT |
| `GET` | `/api/auth/me` | Get current user info |
| `GET` | `/api/dashboard/stats` | Dashboard statistics |
| `GET` | `/api/agents` | List all agents |
| `POST` | `/api/agents` | Create a new agent |
| `PATCH` | `/api/agents/:id` | Update agent settings |
| `DELETE` | `/api/agents/:id` | Delete an agent |
| `POST` | `/api/agents/:id/regenerate-key` | Regenerate API key |
| `POST` | `/api/agents/:id/rag/upload` | Upload PDF for RAG indexing |
| `POST` | `/api/chat` | Send a message to an agent |

---

## 📸 Pages Overview

- **Landing Page** — Hero section, feature grid with search filtering, dashboard preview with live chart, CTA sections
- **Dashboard** — Total agents, API call stats, usage trend bar chart, recent chat history, agent cards
- **Chat** — Agent selector dropdown, real-time messaging with typing indicators, memory/RAG status display
- **Create Agent** — Guided form with model selection, system prompt, memory/RAG toggles
- **Manage Agents** — Data table with edit modal, API key rotation, PDF upload for RAG, delete with confirmation

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Mukesh Kumar**
- GitHub: [@MukeshKumar-17](https://github.com/MukeshKumar-17)

---

<p align="center">
  <strong>⚡ Built for real-world deployment</strong>
</p>
