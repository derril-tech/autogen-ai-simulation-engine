# 🏙️ AI Simulation Engine
**Agent-Based City Modeling with Real-Time Visualizations**

🌐 **[View Live Application](https://autogen-ai-simulation-engine-web.vercel.app/)**

> **A sophisticated city simulation platform where autonomous agents drive emergent behavior. Model traffic patterns, economic dynamics, and urban growth through interactive, real-time visualizations.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.109+-009688.svg)](https://fastapi.tiangolo.com/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black.svg)](https://vercel.com/)

---

## ✨ What It Does

AI Simulation Engine demonstrates **agent-based modeling** and **systems thinking** through an interactive city simulation where:

1. **Autonomous Agents** — Citizens, companies, and vehicles make independent decisions
2. **Emergent Behavior** — Complex patterns arise from simple agent interactions
3. **Real-Time Visualization** — Performance-optimized React renders thousands of agents smoothly
4. **Policy Experimentation** — AI-powered policy advisor suggests parameter adjustments
5. **Historical Analysis** — Archive and compare simulation runs to understand system dynamics

All powered by deterministic tick-based systems with background job orchestration.

---

## 🎯 Core Features

### 🤖 **Agent-Based Modeling**
- **Three Agent Types** — Citizens (homes, jobs, happiness), Companies (employment, economy), Vehicles (traffic, congestion)
- **Autonomous Behavior** — Each agent makes decisions based on local state and environment
- **Emergent Patterns** — Traffic flows, economic cycles, and population dynamics emerge naturally
- **Deterministic Stepping** — Reproducible results with tick-based simulation

### 📊 **Performance-Aware Visualizations**
- **Real-Time Grid Rendering** — Optimized React components handle 1000+ agents smoothly
- **Interactive Agent Inspector** — Click any agent to view detailed state
- **Live Metrics Dashboard** — Employment, congestion, price index, and commute times update in real-time
- **Time-Series Charts** — Visualize system evolution over hundreds of ticks
- **Mobile-Optimized** — Responsive design with 44px+ touch targets

### 🎨 **Modern UI/UX**
- **State-Driven Architecture** — Smooth transitions without page reloads
- **Dark/Light Mode** — Beautiful theme with system preference support
- **Single-Page Experience** — Seamless navigation between simulation views
- **Real-Time Updates** — Polling architecture keeps data fresh without WebSockets overhead

### 🧠 **AI-Powered Policy Advisor**
- **OpenAI Integration** — GPT-4.1-mini provides intelligent policy recommendations
- **Bounded Parameter Control** — AI suggests tax rates, road budgets, and zoning policies
- **Context-Aware Suggestions** — Understands simulation mechanics and trade-offs
- **Streaming Chat Interface** — Interactive conversation with the Mayor AI advisor

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🎮 **Interactive Simulator** | Create, step, and control simulations in real-time |
| 📈 **Real-Time Metrics** | Live dashboard with employment, congestion, and economic indicators |
| 🗄️ **Simulation Archive** | Browse and replay historical simulation runs |
| 🔄 **Comparison Tool** | Side-by-side analysis of different simulation scenarios |
| 💾 **Export & Share** | Download simulation data or share via URL |
| 💬 **AI Chat Interface** | Conversational policy advisor with streaming responses |
| 🎛️ **Custom Presets** | Save and reuse custom simulation configurations |
| 📊 **Event Timeline** | Track simulation milestones and agent actions |
| 🎯 **Agent Inspector** | Deep dive into individual agent state and behavior |
| ⏸️ **Background Jobs** | Long-running simulations with pause/resume capability |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16.0.10** | React 19.2 with App Router and Server Components |
| **TypeScript** | Type-safe development with strict mode |
| **Tailwind CSS** | Utility-first styling with design tokens |
| **shadcn/ui** | Accessible component library |
| **React 19.2** | Latest React features with performance optimizations |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance async Python API |
| **Python 3.11+** | Modern Python with type hints |
| **Pydantic v2** | Data validation and serialization |
| **OpenAI GPT-4.1-mini** | Intelligent policy recommendations |

### **Data & Infrastructure** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL database with RPC functions |
| **Upstash Redis** | Job queue, caching, and live state storage |
| **Railway** | Backend API hosting |
| **Vercel** | Frontend hosting with edge functions |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INTERACTION                         │
│         Create Simulation → Step Ticks → Observe            │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│              AGENT-BASED SIMULATION ENGINE                  │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │   Citizens   │  │  Companies   │  │   Vehicles   │      │
│  │  (Agents)    │  │   (Agents)   │  │   (Agents)   │      │
│  │              │  │              │  │              │      │
│  │ • Home       │  │ • Jobs       │  │ • Routes     │      │
│  │ • Work       │  │ • Wages      │  │ • Speed      │      │
│  │ • Happiness  │  │ • Economy    │  │ • Congestion │      │
│  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘      │
│         │                 │                 │               │
│         └─────────────────┼─────────────────┘               │
│                           │                                  │
│                  ┌────────▼────────┐                        │
│                  │  Tick Engine    │                        │
│                  │  (Deterministic)│                        │
│                  └────────┬────────┘                        │
└───────────────────────────┼──────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────────┐
│              REAL-TIME VISUALIZATION                        │
│  • Grid Renderer (1000+ agents)                            │
│  • Metrics Dashboard (live updates)                        │
│  • Time-Series Charts (historical data)                     │
│  • Agent Inspector (detailed state)                        │
└─────────────────────────────────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────────┐
│              AI POLICY ADVISOR (Optional)                   │
│  ┌──────────────────────────────────────────────┐          │
│  │  User: "Reduce traffic congestion"            │          │
│  │  ↓                                            │          │
│  │  OpenAI GPT-4.1-mini Analysis                │          │
│  │  ↓                                            │          │
│  │  Policy Patch: {roadBudget: 75, ...}        │          │
│  │  ↓                                            │          │
│  │  Apply to Simulation                         │          │
│  └──────────────────────────────────────────────┘          │
└─────────────────────────────────────────────────────────────┘
```

---

## 📖 User Guide

### Getting Started

1. **Create a Simulation** — Navigate to `/simulator`, select a preset (Small Town, Gridlock City, or Boomtown), and click "Create"
2. **Step the Simulation** — Use "Step 1", "Step 10", or "Step 50" to advance time
3. **Observe Behavior** — Watch agents move, metrics update, and patterns emerge
4. **Inspect Agents** — Click any cell or agent in the grid to view detailed state
5. **Try AI Advisor** — Go to `/playground` and ask the Mayor AI for policy suggestions

### Understanding the Simulation

| Component | What It Represents |
|-----------|-------------------|
| **Grid** | City layout with residential, commercial, and road zones |
| **Citizens** | Population with homes, jobs, happiness, and commute times |
| **Companies** | Employers that provide jobs and affect local economy |
| **Vehicles** | Traffic that moves between homes and jobs |
| **Metrics** | System-level indicators (employment, congestion, price index) |
| **Events** | Simulation milestones and agent actions |

### Pro Tips

- **Start with Gridlock City** to see traffic dynamics in action
- **Step slowly** (1 tick at a time) to observe agent decision-making
- **Use the Inspector** to understand individual agent behavior
- **Try different presets** to see how initial conditions affect outcomes
- **Ask the AI** for policy suggestions when metrics need improvement
- **Compare simulations** to understand parameter impact

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Grid Rendering | 1000+ agents at 60fps |
| Tick Computation | <150ms for 32x32 grid |
| API Response Time | <500ms (p95) |
| Frontend Bundle | Optimized with code splitting |
| Mobile Performance | 90+ Lighthouse score |
| Real-Time Updates | Polling every 1.2s |

---

## 🛡️ Architecture Highlights

### Systems Thinking
- **Interconnected Systems** — Tax rates affect happiness, road budgets affect traffic, zoning affects employment
- **Feedback Loops** — Agent decisions create patterns that influence future decisions
- **Emergent Behavior** — Complex city dynamics arise from simple agent rules

### Agent-Based Modeling
- **Autonomous Agents** — Each citizen, company, and vehicle makes independent decisions
- **Local Interactions** — Agents respond to their immediate environment
- **Deterministic Rules** — Reproducible results enable experimentation

### Performance Optimization
- **React Memoization** — Grid cells memoized to prevent unnecessary re-renders
- **Efficient State Management** — Minimal state updates, batched operations
- **Background Jobs** — Long-running simulations don't block the UI
- **Redis Caching** — Fast state retrieval and job queue management

---

## 🎨 Customization

### Simulation Presets
- **Small Town** — Low congestion, balanced growth
- **Gridlock City** — High traffic, dense jobs
- **Boomtown** — Rapid expansion, economic growth

### Custom Presets
Create and save your own simulation configurations with custom parameters:
- Grid size (up to 128x128)
- Initial population
- Tax rates
- Road budgets
- Zoning policies

---

## 🛡️ Security

- ✅ API rate limiting (30-60 requests/minute per endpoint)
- ✅ CORS protection for API endpoints
- ✅ Environment variables for all secrets
- ✅ Input sanitization and validation
- ✅ Bounded parameter ranges (AI cannot suggest invalid values)
- ✅ Supabase RPC functions for secure database access

---

## 📈 What Makes This Impressive

This application demonstrates proficiency in:

- 🤖 **Agent-Based Modeling** — Autonomous agents with emergent behavior patterns
- 🧠 **Systems Thinking** — Understanding interconnected systems and feedback loops
- ⚛️ **Performance-Aware React** — Optimized rendering of 1000+ interactive agents
- 🎨 **Modern Full-Stack** — Next.js 16, React 19.2, FastAPI, TypeScript
- 🤖 **AI Integration** — OpenAI GPT-4.1-mini with streaming responses
- 💾 **Database Design** — Supabase PostgreSQL with RPC functions
- ⚡ **Real-Time Systems** — Background jobs, polling, and live state management
- 🎯 **State Management** — Efficient React state patterns and optimization
- ☁️ **Cloud Architecture** — Railway, Vercel, Upstash Redis deployment
- 🔧 **DevOps** — Environment management, CI/CD, monitoring

---

## 🙏 Acknowledgments

- **[OpenAI](https://openai.com/)** — GPT-4.1-mini API for intelligent policy recommendations
- **[Supabase](https://supabase.com/)** — PostgreSQL database and RPC functions
- **[Upstash](https://upstash.com/)** — Serverless Redis for caching and job queues
- **[Railway](https://railway.app/)** — Backend API hosting
- **[Vercel](https://vercel.com/)** — Frontend hosting and edge functions
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful, accessible components
- **[Next.js](https://nextjs.org/)** — React framework with App Router
- **[FastAPI](https://fastapi.tiangolo.com/)** — Modern Python web framework

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">


[Live Demo](https://autogen-ai-simulation-engine-web.vercel.app/) 

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
