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
    <span style={{ color: '#F8FAFC', fontSize: 40, fontWeight: 800, lineHeight: 1.04, letterSpacing: -1.4 }}>Denis Sam Kusmahendra</span>
    <span style={{ color: '#22D3EE', fontSize: 20, fontWeight: 700, marginTop: 12 }}>Data Analytics & Business Intelligence</span>
    <span style={{ color: '#94A3B8', fontSize: 17, lineHeight: 1.55, marginTop: 12, maxWidth: 570 }}>Transforming raw business data into actionable insights.</span>
  </div>

  <div style={{ position: 'relative', display: 'flex', alignItems: 'center', gap: 9 }}>
    {['SQL • BigQuery', 'Python', 'Power BI • Tableau', 'Excel'].map(function(item) {
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

👋 Hello! I'm Denis Sam Kusmahendra, a Statistics undergraduate at Jakarta State University passionate about Business Intelligence, Data Analytics, and leveraging data to solve real-world business problems.

🗂️ Over the past several months, I've built end-to-end analytics projects using SQL, Python, Power BI, and BigQuery, focusing on sales performance, customer behavior, marketing funnel optimization, and inventory forecasting. Through these projects, I've learned how to translate data into actionable insights that support better business decisions.

🎥 I also create beginner-friendly SQL and data analytics tutorials on YouTube, strengthening my ability to communicate technical concepts clearly and translate data concepts into practical examples.

## 🛠 Toolbox

![SQL](https://img.shields.io/badge/SQL-336791?style=flat&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white) ![Statsmodels](https://img.shields.io/badge/Statsmodels-003B57?style=flat) ![Power%20BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black) ![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat&logo=googlebigquery&logoColor=white) ![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)

## 📌 Selected Work

| Project | What it demonstrates | Stack |
|---------|----------------------|-------|
| **[Sales Performance & Business Dashboard](https://github.com/deniskusmahendra/sales-performance-analysis)** | Interactive Power BI dashboard analyzing sales KPIs, revenue trends, and regional performance using the Olist e-commerce dataset. | `PostgreSQL` `Power BI` |
| **[Customer Retention & Segmentation Analysis](https://github.com/deniskusmahendra/customer-retention-and-segmentation)** | Applied RFM segmentation and Cohort Analysis to identify high-value customers and evaluate customer retention over time. | `Python` `SQL` `Power BI` |
| **[Marketing Performance & Funnel Analytics](https://github.com/deniskusmahendra/marketing-and-conversion-funnel)** | Analyzed GA4 event data in BigQuery to identify checkout funnel drop-offs, conversion rates, and marketing performance. | `BigQuery` `SQL` `Power BI` |
| **[Demand Forecasting & Inventory Optimization](https://github.com/deniskusmahendra/demand-forecasting-and-inventory-optimization)** | Built Holt-Winters forecasting models and an ABC-XYZ inventory matrix to support inventory planning and replenishment decisions. | `SQL` `Python` `Power BI` |
| **[YouTube — Data & BI Tools Tutorials](https://www.youtube.com/@deniskusmahendra)** | Created a 5-part SQL tutorial series using PostgreSQL and a fictional e-commerce database, demonstrating technical communication and teaching ability. | `SQL` `PostgreSQL` |

**Now:** Building new analytics projects and continuously improving my SQL, Python, Power BI, Tableau, and Google BigQuery skills while exploring Business Intelligence and Operations Analytics.
