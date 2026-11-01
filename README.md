<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:2ee6c9,50:3b8cff,100:a35cff&text=Jorge%20Luis%20Villegas%20Oliva&fontColor=ffffff&fontSize=42&fontAlignY=38&desc=IT%20Support%20%C2%B7%20Networking%20%C2%B7%20Azure%20Cloud%20%C2%B7%20Production%20systems&descAlignY=58&animation=fadeIn" width="100%" alt="Jorge Luis Villegas Oliva">

<a href="https://jlvillegas.github.io/portfolio/"><img src="https://readme-typing-svg.demolab.com?font=IBM+Plex+Mono&weight=500&size=20&duration=2600&pause=900&color=2EE6C9&center=true&vCenter=true&width=640&lines=IT+Support+%C2%B7+Help+Desk+%C2%B7+NOC;Networks%3A+Starlink%2C+Omada%2C+MikroTik%2C+Ubiquiti;Microsoft+Azure+certified%3A+AZ-900+%C2%B7+AI-901;I+build+and+run+systems+in+production" alt="IT Support, networking, Azure and production systems"></a>

<p>
<a href="https://jlvillegas.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-2ee6c9?style=for-the-badge&logo=githubpages&logoColor=04161a" alt="Portfolio"></a>
<a href="https://www.linkedin.com/in/jorge-luis-villegas-oliva-212704125/"><img src="https://img.shields.io/badge/LinkedIn-3b8cff?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="mailto:lvillegasjorge@gmail.com"><img src="https://img.shields.io/badge/Email-a35cff?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
<img src="https://img.shields.io/badge/Open%20to-remote%20work-3cf29a?style=for-the-badge" alt="Open to remote work">
<img src="https://img.shields.io/badge/Argentina-UTC--3-1f2937?style=for-the-badge" alt="Argentina, UTC-3">
</p>

**English** · [Español](https://github.com/jlvillegas/jlvillegas/blob/main/README.es.md)

</div>

### 👋 Hi, I'm Jorge

IT and systems technician from Argentina. I keep real businesses running: I've been **Head of IT at a dental clinic since 2015**, I was **IT Systems Lead at a company running SAP**, and I design and install **networks, Starlink links and CCTV** for homes, cabins and businesses.

I also **built and run in production** the clinic's management system — used every day by 5 practitioners, reception and admin — on Docker, PostgreSQL, DigitalOcean and Cloudflare.

Now I'm growing into **cloud on Microsoft Azure** (AZ-900 and AI-901 certified).

> 🎯 **Looking for remote roles:** IT Support / Help Desk · NOC · Network Support · Junior Cloud Administrator (Azure) · Technical Support Engineer
> 🕒 UTC-3 — only 1–2 hours from US Eastern time

### 🧰 What I bring

- 🖥️ **IT Support & Help Desk** — day-to-day support for staff: Windows workstations, printers, software, connectivity and SAP users.
- 🌐 **Networking & security** — Starlink, Wi-Fi 6 mesh, TP-Link Omada, MikroTik, Ubiquiti, TCP/IP; IP cameras (Hikvision, Dahua, EZVIZ), alarms and access control.
- ☁️ **Cloud & servers** — Linux server with Docker Compose, PostgreSQL, DigitalOcean, Cloudflare, auto-deploy from GitHub, automated tests. Azure fundamentals certified.
- 🤖 **AI & automation** — Claude API, Gemini API and n8n workflows that remove manual work.

### 🚀 Featured work

#### 🦷 Clínica Villegas management system — *in production*

Replaced the legacy software, spreadsheets and paper of a dental clinic with 30+ years of history.

- Per-practitioner schedule and online appointments that patients confirm or cancel from a link
- Clinical records with odontogram, X-rays and treatment quotes
- Mercado Pago QR payments confirmed by webhook, daily cash register and practitioner payouts
- Waiting room: the TV calls patients with a neural voice generated on our own server
- AI in the office: clinical dictation and reading of paper records with the Claude API
- Google sign-in and role-based permissions · **53 automated test suites**

```mermaid
flowchart LR
    U["Reception · Dentists<br/>Patients · Waiting-room TV"] --> CF["Cloudflare<br/>(HTTPS)"]
    CF --> WEB
    subgraph SRV["DigitalOcean · Docker Compose"]
        direction TB
        WEB["React + TypeScript"] --> API["Node.js API"]
        API --> DB[("PostgreSQL")]
    end
    subgraph EXT["External services"]
        direction TB
        MP["Mercado Pago<br/>QR + webhook"]
        GO["Google sign-in"]
        AI["Claude API"]
    end
    API --> EXT
    GH["GitHub"] -- "auto-deploy" --> SRV
```

<sub>The code is private because it is a healthcare system. Architecture details and a demo with fake data are in the <a href="https://jlvillegas.github.io/portfolio/">portfolio</a>. Built with AI coding assistants (Claude and Codex).</sub>

#### More projects

| Project | What it is | Status |
|---|---|---|
| [**AI Lead Qualifier**](https://github.com/jlvillegas/ai-lead-qualifier) | n8n workflow: web form → data validation → Gemini qualifies the lead (JSON) → Google Sheets → Gmail alert for hot leads. Leads are never lost, even if the AI fails. | 🟢 Open source + demo video |
| **Wi-Fi 6 for a 10-cabin tourist complex** | Two Starlink Mini uplinks, outdoor access points and Wi-Fi 6 mesh covering the whole property in Nono, Córdoba. The quote split equipment, cabling, labor and monthly service. | ✅ Delivered |
| [**villegasinsumos.com**](https://villegasinsumos.com/) | Online store for medical and dental supplies: 200+ products with variants, search and categories. The cart sends the order by WhatsApp and the site shows if the store is open. | 🟢 Live |
| **Websites for local businesses** | [Clínica Villegas](https://villegascentromedicoodontologico.com/) · [Dentist personal brand](https://odontologa-alejandravillegas.netlify.app/) · [Residencia Franciscus](https://franciscus-merlo-san-luis.netlify.app/) — built to receive inquiries by WhatsApp from mobile. | 🟢 Live |
| [**Portfolio**](https://jlvillegas.github.io/portfolio/) | Hand-made with HTML, CSS and JavaScript, light/dark theme and a status board that checks the published sites. | 🟢 Live |

### 🛠️ Tech I use

<p>
<img src="https://skillicons.dev/icons?i=windows,linux,docker,azure,cloudflare,netlify,git,github,githubactions,vscode,react,ts,js,nodejs,postgres,tailwind,vite,html,css,py&perline=10" alt="Windows, Linux, Docker, Azure, Cloudflare, Netlify, Git, GitHub, GitHub Actions, VS Code, React, TypeScript, JavaScript, Node.js, PostgreSQL, Tailwind, Vite, HTML, CSS, Python">
</p>

<p>
<img src="https://img.shields.io/badge/Starlink-000000?style=flat-square&logo=starlink&logoColor=white" alt="Starlink">
<img src="https://img.shields.io/badge/TP--Link%20Omada-4ACBD6?style=flat-square&logo=tplink&logoColor=white" alt="TP-Link Omada">
<img src="https://img.shields.io/badge/MikroTik-293239?style=flat-square&logo=mikrotik&logoColor=white" alt="MikroTik">
<img src="https://img.shields.io/badge/Ubiquiti-0559C9?style=flat-square&logo=ubiquiti&logoColor=white" alt="Ubiquiti">
<img src="https://img.shields.io/badge/CCTV-Hikvision%20%C2%B7%20Dahua%20%C2%B7%20EZVIZ-c0392b?style=flat-square" alt="CCTV: Hikvision, Dahua, EZVIZ">
<img src="https://img.shields.io/badge/SAP%20ERP-0FAAFF?style=flat-square&logo=sap&logoColor=white" alt="SAP ERP">
<img src="https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white" alt="DigitalOcean">
<img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white" alt="n8n">
<img src="https://img.shields.io/badge/Claude%20API-D97757?style=flat-square&logo=claude&logoColor=white" alt="Claude API">
<img src="https://img.shields.io/badge/Gemini%20API-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini API">
</p>

### 💼 Experience

| Role | Company | Dates |
|---|---|---|
| **Founder & Network / Security Technician** | Villegas Insumos Tecnológicos (self-employed) | Oct 2023 – present |
| **Head of IT & Systems** | Clínica Villegas (dental clinic) | Oct 2015 – present |
| **IT Systems Lead** | Sonne S.R.L. — IT systems, network, servers, CCTV and SAP user support | Oct 2021 – Aug 2023 |

<sub>Full details on <a href="https://www.linkedin.com/in/jorge-luis-villegas-oliva-212704125/">LinkedIn</a>.</sub>

### 🎓 Certifications & education

<p>
<a href="https://learn.microsoft.com/api/credentials/share/en-us/JorgeVillegas-6113/4644DE0052ADC6FE?sharingId=6314E6AE393F7D46"><img src="https://img.shields.io/badge/AZ--900-Azure%20Fundamentals-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Microsoft Certified: Azure Fundamentals (AZ-900)"></a>
<a href="https://learn.microsoft.com/api/credentials/share/en-us/JorgeVillegas-6113/A836E11048C2F42E?sharingId=6314E6AE393F7D46"><img src="https://img.shields.io/badge/AI--901-Azure%20AI%20Fundamentals-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Microsoft Certified: Azure AI Fundamentals (AI-901)"></a>
</p>

- ✅ **Microsoft Certified: Azure Fundamentals (AZ-900)** — Oct 2026 · [verify](https://learn.microsoft.com/api/credentials/share/en-us/JorgeVillegas-6113/4644DE0052ADC6FE?sharingId=6314E6AE393F7D46)
- ✅ **Microsoft Certified: Azure AI Fundamentals (AI-901)** — Oct 2026 · [verify](https://learn.microsoft.com/api/credentials/share/en-us/JorgeVillegas-6113/A836E11048C2F42E?sharingId=6314E6AE393F7D46)
- 📚 Studying: **AZ-104** (Azure Administrator) and **AI-103** (Azure AI Apps and Agents)
- 🎓 Bachelor's in Computer Science (Licenciatura en Informática), Universidad Siglo 21 — 2024–2027 · intermediate degree: University Analyst in Computer Systems
- 🗣️ Spanish (native) · English (intermediate, practicing every day)

### 📫 Let's talk

Open to **remote full-time or contract roles**. The fastest way to reach me is [email](mailto:lvillegasjorge@gmail.com) or [LinkedIn](https://www.linkedin.com/in/jorge-luis-villegas-oliva-212704125/).

<img src="https://capsule-render.vercel.app/api?type=waving&height=100&color=0:a35cff,50:3b8cff,100:2ee6c9&section=footer" width="100%" alt="">
