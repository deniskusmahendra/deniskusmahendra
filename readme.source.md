```aura width=860 height=300
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'space-between', width: '100%', height: '100%', overflow: 'hidden', borderRadius: 20, background: '#0B0F14', border: '1px solid #243447', fontFamily: 'Inter, sans-serif', padding: '34px 42px' }}>
  <style>{`
    @keyframes orbit { to { transform: rotate(360deg); } }
    @keyframes breathe { 0%, 100% { opacity: .5; } 50% { opacity: 1; } }
    #orbit { animation: orbit 24s linear infinite; transform-origin: 742px 151px; }
    #signal { animation: breathe 2.4s ease-in-out infinite; }
  `}</style>
  <svg width="860" height="300" style={{ position: 'absolute', top: -1, left: -1 }}>
    <defs>
      <pattern id="grid" width="42" height="42" patternUnits="userSpaceOnUse">
        <path d="M 42 0 L 0 0 0 42" fill="none" stroke="rgba(36,52,71,.42)" strokeWidth="1" />
      </pattern>
      <radialGradient id="cyanGlow" cx="88%" cy="48%" r="52%">
        <stop offset="0%" stopColor="rgba(34,211,238,.17)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
      <radialGradient id="amberGlow" cx="5%" cy="0%" r="72%">
        <stop offset="0%" stopColor="rgba(245,158,11,.13)" />
        <stop offset="100%" stopColor="rgba(245,158,11,0)" />
      </radialGradient>
    </defs>
    <rect width="860" height="300" fill="url(#grid)" />
    <rect width="860" height="300" fill="url(#cyanGlow)" />
    <rect width="860" height="300" fill="url(#amberGlow)" />
    <g id="orbit">
      <circle cx="742" cy="151" r="82" fill="none" stroke="rgba(34,211,238,.34)" strokeWidth="1" strokeDasharray="4 10" />
      <circle cx="742" cy="69" r="4" fill="#22D3EE" />
    </g>
    <circle cx="742" cy="151" r="53" fill="rgba(11,15,20,.64)" stroke="rgba(245,158,11,.34)" />
    <path d="M714 164 L731 147 L744 158 L772 130" fill="none" stroke="#22D3EE" strokeWidth="3" strokeLinecap="round" strokeLinejoin="round" />
    <circle cx="772" cy="130" r="4" fill="#F59E0B" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'space-between' }}>
    <span style={{ color: '#F59E0B', fontSize: 12, fontWeight: 800, fontFamily: 'monospace', letterSpacing: 2.2 }}>DENIS / PROFILE</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8, border: '1px solid rgba(34,211,238,.28)', borderRadius: 999, background: 'rgba(15,23,42,.58)', padding: '7px 12px' }}>
      <span id="signal" style={{ width: 7, height: 7, borderRadius: 999, background: '#22D3EE' }} />
      <span style={{ color: '#CBD5E1', fontSize: 11, fontFamily: 'monospace', letterSpacing: 1 }}>JAKARTA, INDONESIA</span>
    </div>
  </div>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: 610 }}>
    <span style={{ color: '#F8FAFC', fontSize: 40, fontWeight: 800, lineHeight: 1.04, letterSpacing: -1.4 }}>Denis Kusmahendra</span>
    <span style={{ color: '#22D3EE', fontSize: 20, fontWeight: 700, marginTop: 12 }}>AI Engineering</span>
    <span style={{ color: '#94A3B8', fontSize: 17, lineHeight: 1.55, marginTop: 12, maxWidth: 570 }}>Building LLM-powered apps on a foundation in statistics and data.</span>
  </div>

  <div style={{ position: 'relative', display: 'flex', alignItems: 'center', gap: 9 }}>
    {['Python • FastAPI', 'LLMs • LangChain', 'Pydantic', 'SQL • PostgreSQL'].map(function(item) {
      return <span key={item} style={{ color: '#CBD5E1', border: '1px solid rgba(148,163,184,.22)', borderRadius: 7, background: 'rgba(15,23,42,.72)', padding: '7px 10px', fontSize: 12, fontWeight: 700, fontFamily: 'monospace', letterSpacing: .7 }}>{item}</span>;
    })}
  </div>
</div>
```

<p align="center">
  <a href="https://deniskusmahendra.github.io/"><img src="https://img.shields.io/badge/Website-0F172A?style=for-the-badge&logo=website&logoColor=22D3EE" alt="Portfolio Website" /></a>
  <a href="https://www.youtube.com/@deniskusmahendra"><img src="https://img.shields.io/badge/YouTube-0F172A?style=for-the-badge&logo=youtube&logoColor=FF0000" alt="YouTube" /></a>
  <a href="https://www.linkedin.com/in/deniskusmahendra/"><img src="https://img.shields.io/badge/LinkedIn-0F172A?style=for-the-badge&logo=linkedin&logoColor=22D3EE" alt="LinkedIn" /></a>
  <a href="mailto:deniskusmahendra@gmail.com"><img src="https://img.shields.io/badge/Email-0F172A?style=for-the-badge&logo=gmail&logoColor=F59E0B" alt="Email" /></a>
  <a href="https://drive.google.com/file/d/1ji1PeWBmWnJwtZGsKh-BlzzDy1JIicd2/view?usp=drive_link"><img src="https://img.shields.io/badge/Resume-0F172A?style=for-the-badge&logo=readme&logoColor=F59E0B" alt="Resume" /></a>
</p>

## 👨‍💼 About Me

👋 Hello! I'm Denis Kusmahendra, a Statistics undergraduate at Jakarta State University focused on **AI Engineering**: building applications powered by large language models.

🤖 I'm currently building LLM apps with Python, FastAPI, Pydantic, and LangChain, such as an API that turns customer reviews into structured sentiment data. Before this, I built end-to-end data analytics projects with SQL, Python, and Power BI, and full-stack websites with Next.js. That background helps me work with data, evaluate model output, and ship working products.

🎥 I also make beginner-friendly SQL and data tutorials on YouTube.

## 🛠 Toolbox

**AI & Backend:** ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white) ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat&logo=pydantic&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white) ![Groq](https://img.shields.io/badge/Groq-F55036?style=flat) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat&logo=sqlalchemy&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

**Web:** ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat&logo=firebase&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)

**Data:** ![SQL](https://img.shields.io/badge/SQL-336791?style=flat&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white) ![Statsmodels](https://img.shields.io/badge/Statsmodels-003B57?style=flat) ![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat&logo=googlebigquery&logoColor=white) ![Power%20BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black) ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

## 🧭 Journey

Newest first.

### 🤖 AI Engineering

| Project | What it is | Stack |
|---------|------------|-------|
| **[Shopping Agent](https://github.com/deniskusmahendra/shopping-agent)** | AI shopping agent. *In progress.* | `Python` `LLMs` |
| **[Feedback Analyzer](https://github.com/deniskusmahendra/feedback-analyzer)** | API that uses an LLM to turn customer reviews into structured data: sentiment label, 1–5 score, and main theme, validated with Pydantic. | `FastAPI` `Groq` `Pydantic` `PostgreSQL` |
| **[Learning AI Engineering](https://github.com/deniskusmahendra/learning-ai-engineering)** | My coursework in Python for AI, async programming, Pydantic validation, and LangChain agents. | `Python` `LangChain` `Pydantic` |

### 🌐 Full-Stack Web

| Project | What it is | Stack |
|---------|------------|-------|
| **[Friend Group Website](https://github.com/deniskusmahendra/friend-group-website)** | [Live](https://friend-group-website.vercel.app) site for my friend group: photo albums, hangout plans, gaming sessions, and badges. | `Next.js` `TypeScript` `Firebase` |
| **[RawMeaters](https://github.com/deniskusmahendra/rawmeaters)** | [Live](https://www.rawmeaters.com) community website with recipes, a beginner guide, and email signup. | `Next.js` `TypeScript` |
| **[Learning Full-Stack Web Development](https://github.com/deniskusmahendra/learning-full-stack-web-development)** | My exercises and projects from Scrimba's full-stack course. | `JavaScript` `React` |

### 📊 Data Analysis

| Project | What it is | Stack |
|---------|------------|-------|
| **[Demand Forecasting & Inventory Optimization](https://github.com/deniskusmahendra/demand-forecasting-and-inventory-optimization)** | Holt-Winters forecasting and an ABC-XYZ inventory matrix for replenishment planning. | `SQL` `Python` `Power BI` |
| **[Marketing & Conversion Funnel](https://github.com/deniskusmahendra/marketing-and-conversion-funnel)** | GA4 event data in BigQuery to find checkout drop-offs and the best traffic sources. | `BigQuery` `SQL` `Power BI` |
| **[Customer Retention & Segmentation](https://github.com/deniskusmahendra/customer-retention-and-segmentation)** | RFM segmentation and cohort analysis to find high-value customers and track retention. | `Python` `SQL` `Power BI` |
| **[Sales Performance Analysis](https://github.com/deniskusmahendra/sales-performance-analysis)** | Power BI dashboard of sales KPIs, revenue trends, and regional performance. | `PostgreSQL` `Power BI` |
| **[Learning Data Analysis](https://github.com/deniskusmahendra/learning-data-analysis)** | My coursework in Excel, SQL, Python, and Power BI. | `Excel` `SQL` `Python` |

### 🎓 Foundations

| Project | What it is | Stack |
|---------|------------|-------|
| **[Portfolio Website](https://github.com/deniskusmahendra/deniskusmahendra.github.io)** | My [personal portfolio site](https://deniskusmahendra.github.io). | `HTML` `CSS` |
| **[College Assignments](https://github.com/deniskusmahendra/college-assignments)** | College coursework in databases and web development. | `SQL` `Web` |

## 🎯 Goals

**Now:** Building LLM-powered apps and AI agents, and learning LangChain, retrieval (RAG), and evaluation.

**Next:** Going deeper into the foundations of AI: machine learning, neural networks, deep learning, and natural language processing (NLP), so I understand how the models I build with work, not just how to call them.
