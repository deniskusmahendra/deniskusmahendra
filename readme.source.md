```aura width=860 height=300
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'space-between', width: '100%', height: '100%', overflow: 'hidden', borderRadius: 18, background: '#0F1E3D', border: '1px solid rgba(91,100,120,.45)', fontFamily: 'Inter, sans-serif', padding: '32px 40px' }}>
  <style>{`
    @keyframes flow { from { stroke-dashoffset: 140; } to { stroke-dashoffset: 0; } }
    @keyframes glow { 0%, 100% { opacity: .35; } 50% { opacity: 1; } }
    #p1, #p2, #p3, #p4, #p5, #p6 { stroke-dasharray: 10 130; animation: flow 3.2s linear infinite; }
    #p2 { animation-delay: .5s; } #p3 { animation-delay: 1.1s; } #p4 { animation-delay: 1.6s; } #p5 { animation-delay: 2.1s; } #p6 { animation-delay: 2.6s; }
    #o1 { animation: glow 3.2s ease-in-out infinite; } #o2 { animation: glow 3.2s ease-in-out 1.6s infinite; }
    #live { animation: glow 2s ease-in-out infinite; }
  `}</style>
  <svg width="860" height="300" style={{ position: 'absolute', top: -1, left: -1 }}>
    <defs>
      <pattern id="dots" width="22" height="22" patternUnits="userSpaceOnUse">
        <circle cx="2" cy="2" r="1" fill="rgba(47,107,255,.16)" />
      </pattern>
      <radialGradient id="violetGlow" cx="82%" cy="50%" r="45%">
        <stop offset="0%" stopColor="rgba(47,107,255,.22)" />
        <stop offset="100%" stopColor="rgba(47,107,255,0)" />
      </radialGradient>
      <radialGradient id="mintGlow" cx="0%" cy="100%" r="60%">
        <stop offset="0%" stopColor="rgba(47,107,255,.12)" />
        <stop offset="100%" stopColor="rgba(47,107,255,0)" />
      </radialGradient>
    </defs>
    <rect width="860" height="300" fill="url(#dots)" />
    <rect width="860" height="300" fill="url(#violetGlow)" />
    <rect width="860" height="300" fill="url(#mintGlow)" />

    {[90, 150, 210].map(function(a) {
      return [64, 118, 172, 226].map(function(b) {
        return <line key={'a' + a + b} x1="600" y1={a} x2="690" y2={b} stroke="rgba(47,107,255,.18)" strokeWidth="1" />;
      });
    })}
    {[64, 118, 172, 226].map(function(b) {
      return [118, 182].map(function(c) {
        return <line key={'b' + b + c} x1="690" y1={b} x2="780" y2={c} stroke="rgba(47,107,255,.18)" strokeWidth="1" />;
      });
    })}

    <line id="p1" x1="600" y1="90" x2="690" y2="118" stroke="#2F6BFF" strokeWidth="2.5" strokeLinecap="round" />
    <line id="p2" x1="600" y1="210" x2="690" y2="172" stroke="#2F6BFF" strokeWidth="2.5" strokeLinecap="round" />
    <line id="p3" x1="690" y1="118" x2="780" y2="118" stroke="#F5F3EE" strokeWidth="2.5" strokeLinecap="round" />
    <line id="p4" x1="600" y1="150" x2="690" y2="64" stroke="#2F6BFF" strokeWidth="2.5" strokeLinecap="round" />
    <line id="p5" x1="690" y1="172" x2="780" y2="182" stroke="#F5F3EE" strokeWidth="2.5" strokeLinecap="round" />
    <line id="p6" x1="690" y1="226" x2="780" y2="182" stroke="#F5F3EE" strokeWidth="2.5" strokeLinecap="round" />

    {[90, 150, 210].map(function(y) {
      return <circle key={'i' + y} cx="600" cy={y} r="7" fill="#0F1E3D" stroke="#2F6BFF" strokeWidth="2" />;
    })}
    {[64, 118, 172, 226].map(function(y) {
      return <circle key={'h' + y} cx="690" cy={y} r="7" fill="#0F1E3D" stroke="#2F6BFF" strokeWidth="2" />;
    })}
    <circle id="o1" cx="780" cy="118" r="15" fill="rgba(47,107,255,.25)" />
    <circle id="o2" cx="780" cy="182" r="15" fill="rgba(47,107,255,.25)" />
    <circle cx="780" cy="118" r="8" fill="#2F6BFF" />
    <circle cx="780" cy="182" r="8" fill="#2F6BFF" />

    <circle id="live" cx="47" cy="41" r="4" fill="#2F6BFF" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', alignItems: 'center', paddingLeft: 16 }}>
    <span style={{ color: 'rgba(245,243,238,.7)', fontSize: 12, fontWeight: 700, letterSpacing: 2.4 }}>JAKARTA, INDONESIA  ·  LEARNING IN PUBLIC</span>
  </div>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: 520 }}>
    <span style={{ color: '#F5F3EE', fontSize: 42, fontWeight: 800, lineHeight: 1.04, letterSpacing: -1.5 }}>Denis Kusmahendra</span>
    <span style={{ color: '#2F6BFF', fontSize: 20, fontWeight: 700, marginTop: 10 }}>AI Engineering</span>
    <span style={{ color: 'rgba(245,243,238,.7)', fontSize: 16, lineHeight: 1.5, marginTop: 10 }}>Statistics student building with LLMs, one layer at a time.</span>
  </div>

  <div style={{ position: 'relative', display: 'flex', alignItems: 'center' }}>
    {['Statistics', 'Data', 'Web', 'AI'].map(function(step, i) {
      var now = step === 'AI';
      return <div key={step} style={{ display: 'flex', alignItems: 'center' }}>
        {i > 0 ? <div style={{ width: 22, height: 1, background: now ? '#F5A524' : 'rgba(91,100,120,.35)' }} /> : null}
        <span style={{ color: now ? '#0F1E3D' : 'rgba(245,243,238,.7)', background: now ? '#F5A524' : 'rgba(15,30,61,.8)', border: now ? '1px solid #F5A524' : '1px solid rgba(91,100,120,.25)', borderRadius: 999, padding: '6px 13px', fontSize: 12, fontWeight: 700, letterSpacing: .6 }}>{step}</span>
      </div>;
    })}
  </div>
</div>
```

<p align="center">
  <a href="https://deniskusmahendra.github.io/"><img src="https://img.shields.io/badge/Website-0F1E3D?style=for-the-badge&logo=website&logoColor=2F6BFF" alt="Portfolio Website" /></a>
  <a href="https://www.youtube.com/@deniskusmahendra"><img src="https://img.shields.io/badge/YouTube-0F1E3D?style=for-the-badge&logo=youtube&logoColor=FF0000" alt="YouTube" /></a>
  <a href="https://www.linkedin.com/in/deniskusmahendra/"><img src="https://img.shields.io/badge/LinkedIn-0F1E3D?style=for-the-badge&logo=linkedin&logoColor=2F6BFF" alt="LinkedIn" /></a>
  <a href="mailto:deniskusmahendra@gmail.com"><img src="https://img.shields.io/badge/Email-0F1E3D?style=for-the-badge&logo=gmail&logoColor=2F6BFF" alt="Email" /></a>
  <a href="https://drive.google.com/file/d/1ji1PeWBmWnJwtZGsKh-BlzzDy1JIicd2/view?usp=drive_link"><img src="https://img.shields.io/badge/Resume-0F1E3D?style=for-the-badge&logo=readme&logoColor=2F6BFF" alt="Resume" /></a>
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

### 🌐 Full-Stack Web

| Project | What it is | Stack |
|---------|------------|-------|
| **[Friend Group Website](https://github.com/deniskusmahendra/friend-group-website)** | [Live](https://friend-group-website.vercel.app) site for my friend group: photo albums, hangout plans, gaming sessions, and badges. | `Next.js` `TypeScript` `Firebase` |
| **[Portfolio Website](https://github.com/deniskusmahendra/deniskusmahendra.github.io)** | My [personal portfolio site](https://deniskusmahendra.github.io). | `HTML` `CSS` |

### 📊 Data Analysis

| Project | What it is | Stack |
|---------|------------|-------|
| **[Demand Forecasting & Inventory Optimization](https://github.com/deniskusmahendra/demand-forecasting-and-inventory-optimization)** | Holt-Winters forecasting and an ABC-XYZ inventory matrix for replenishment planning. | `SQL` `Python` `Power BI` |
| **[Marketing & Conversion Funnel](https://github.com/deniskusmahendra/marketing-and-conversion-funnel)** | GA4 event data in BigQuery to find checkout drop-offs and the best traffic sources. | `BigQuery` `SQL` `Power BI` |
| **[Customer Retention & Segmentation](https://github.com/deniskusmahendra/customer-retention-and-segmentation)** | RFM segmentation and cohort analysis to find high-value customers and track retention. | `Python` `SQL` `Power BI` |
| **[Sales Performance Analysis](https://github.com/deniskusmahendra/sales-performance-analysis)** | Power BI dashboard of sales KPIs, revenue trends, and regional performance. | `PostgreSQL` `Power BI` |

## 🎯 Goals

**Now:** Building LLM-powered apps and AI agents, and learning LangChain, retrieval (RAG), and evaluation ([my coursework](https://github.com/deniskusmahendra/learning-ai-engineering)).

**Next:** Going deeper into the foundations of AI: machine learning, neural networks, deep learning, and natural language processing (NLP), so I understand how the models I build with work, not just how to call them.
