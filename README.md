[fatma_github_readme.html](https://github.com/user-attachments/files/29000037/fatma_github_readme.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Fatma Zahra Dorgham – GitHub Profile README</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet"/>
<style>
  :root {
    --bg: #0D1117;
    --surface: #161B22;
    --surface2: #1C2128;
    --border: #30363D;
    --border2: #21262D;
    --text: #E6EDF3;
    --muted: #8B949E;
    --purple: #A78BFA;
    --purple-dim: #6D28D9;
    --purple-glow: #7C3AED22;
    --cyan: #22D3EE;
    --cyan-dim: #0891B2;
    --green: #3FB950;
    --orange: #F97316;
    --pink: #F472B6;
    --yellow: #E3B341;
    --font-mono: 'JetBrains Mono', 'Fira Code', monospace;
    --font-sans: 'Inter', -apple-system, sans-serif;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: var(--font-sans);
    min-height: 100vh;
    padding: 0;
    line-height: 1.6;
  }

  /* ── COPY BUTTON ── */
  #copy-btn {
    position: fixed;
    top: 20px;
    right: 20px;
    background: var(--purple-dim);
    color: #fff;
    border: none;
    padding: 10px 18px;
    border-radius: 8px;
    font-family: var(--font-mono);
    font-size: 13px;
    cursor: pointer;
    z-index: 100;
    display: flex;
    align-items: center;
    gap: 8px;
    transition: background 0.2s;
  }
  #copy-btn:hover { background: #7C3AED; }
  #copy-btn.copied { background: #16a34a; }

  /* ── LAYOUT ── */
  .readme {
    max-width: 860px;
    margin: 0 auto;
    padding: 40px 24px 80px;
  }

  /* ── HEADER HERO ── */
  .hero {
    text-align: center;
    padding: 48px 0 36px;
  }

  .hero-greeting {
    font-family: var(--font-mono);
    font-size: 14px;
    color: var(--cyan);
    letter-spacing: 0.1em;
    text-transform: uppercase;
    margin-bottom: 12px;
  }

  .hero-name {
    font-size: clamp(28px, 5vw, 48px);
    font-weight: 700;
    background: linear-gradient(135deg, var(--purple) 0%, var(--cyan) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 8px;
    line-height: 1.2;
  }

  .hero-title {
    font-size: 18px;
    font-weight: 400;
    color: var(--muted);
    margin-bottom: 24px;
  }

  .hero-title span {
    color: var(--purple);
    font-weight: 500;
  }

  /* ── TERMINAL BLOCK ── */
  .terminal {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    overflow: hidden;
    margin: 0 auto 40px;
    max-width: 640px;
    text-align: left;
  }

  .terminal-bar {
    background: var(--surface2);
    border-bottom: 1px solid var(--border);
    padding: 10px 16px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .terminal-dot {
    width: 12px;
    height: 12px;
    border-radius: 50%;
  }
  .dot-red   { background: #FF5F57; }
  .dot-yellow { background: #FFBD2E; }
  .dot-green { background: #28C840; }

  .terminal-title {
    font-family: var(--font-mono);
    font-size: 12px;
    color: var(--muted);
    margin-left: 8px;
  }

  .terminal-body {
    padding: 20px 24px;
    font-family: var(--font-mono);
    font-size: 13.5px;
    line-height: 1.9;
  }

  .t-prompt { color: var(--green); }
  .t-cmd    { color: var(--cyan); }
  .t-key    { color: var(--purple); }
  .t-val    { color: var(--text); }
  .t-str    { color: var(--yellow); }
  .t-comment{ color: var(--muted); }
  .t-cursor {
    display: inline-block;
    width: 8px;
    height: 1em;
    background: var(--cyan);
    vertical-align: text-bottom;
    animation: blink 1s step-end infinite;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

  /* ── BADGES ── */
  .badges {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    justify-content: center;
    margin-bottom: 48px;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 5px 12px;
    border-radius: 6px;
    font-size: 12px;
    font-family: var(--font-mono);
    font-weight: 500;
    border: 1px solid;
    text-decoration: none;
    transition: opacity 0.2s;
  }
  .badge:hover { opacity: 0.8; }
  .badge-purple { background: #2D1B69; border-color: var(--purple); color: var(--purple); }
  .badge-cyan   { background: #083344; border-color: var(--cyan); color: var(--cyan); }
  .badge-green  { background: #0D2818; border-color: var(--green); color: var(--green); }
  .badge-orange { background: #2C1A06; border-color: var(--orange); color: var(--orange); }

  /* ── SECTION ── */
  .section {
    margin-bottom: 48px;
  }

  .section-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 20px;
    padding-bottom: 12px;
    border-bottom: 1px solid var(--border);
  }

  .section-icon {
    font-size: 20px;
  }

  .section-title {
    font-family: var(--font-mono);
    font-size: 16px;
    font-weight: 500;
    color: var(--text);
  }

  .section-line {
    flex: 1;
    height: 1px;
    background: linear-gradient(to right, var(--border), transparent);
  }

  /* ── ABOUT ── */
  .about-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 12px;
  }

  .about-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 16px;
    display: flex;
    align-items: flex-start;
    gap: 12px;
  }

  .about-icon {
    font-size: 20px;
    flex-shrink: 0;
    margin-top: 1px;
  }

  .about-label {
    font-size: 11px;
    color: var(--muted);
    font-family: var(--font-mono);
    text-transform: uppercase;
    letter-spacing: 0.08em;
    margin-bottom: 3px;
  }

  .about-value {
    font-size: 13.5px;
    color: var(--text);
    font-weight: 500;
  }

  /* ── SKILLS ── */
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 12px;
  }

  .skill-category {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 16px;
  }

  .skill-cat-header {
    display: flex;
    align-items: center;
    gap: 8px;
    margin-bottom: 12px;
  }

  .skill-cat-dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    flex-shrink: 0;
  }

  .skill-cat-name {
    font-family: var(--font-mono);
    font-size: 12px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.08em;
  }

  .skill-list {
    display: flex;
    flex-wrap: wrap;
    gap: 5px;
  }

  .skill-tag {
    background: var(--surface2);
    border: 1px solid var(--border2);
    border-radius: 4px;
    padding: 3px 7px;
    font-family: var(--font-mono);
    font-size: 11.5px;
    color: var(--muted);
  }

  /* ── PROJECTS ── */
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 14px;
  }

  .project-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 20px;
    position: relative;
    overflow: hidden;
    transition: border-color 0.2s, transform 0.2s;
  }
  .project-card:hover {
    transform: translateY(-2px);
  }

  .project-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 2px;
  }

  .proj-purple::before { background: var(--purple); }
  .proj-cyan::before   { background: var(--cyan); }
  .proj-green::before  { background: var(--green); }
  .proj-orange::before { background: var(--orange); }
  .proj-pink::before   { background: var(--pink); }
  .proj-yellow::before { background: var(--yellow); }

  .proj-purple:hover { border-color: var(--purple); }
  .proj-cyan:hover   { border-color: var(--cyan); }
  .proj-green:hover  { border-color: var(--green); }
  .proj-orange:hover { border-color: var(--orange); }
  .proj-pink:hover   { border-color: var(--pink); }
  .proj-yellow:hover { border-color: var(--yellow); }

  .proj-header {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    margin-bottom: 8px;
    gap: 12px;
  }

  .proj-icon { font-size: 22px; }

  .proj-name {
    font-size: 15px;
    font-weight: 600;
    color: var(--text);
    font-family: var(--font-mono);
    flex: 1;
  }

  .proj-desc {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.6;
    margin-bottom: 12px;
  }

  .proj-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 5px;
  }

  .proj-tag {
    font-family: var(--font-mono);
    font-size: 11px;
    padding: 2px 7px;
    border-radius: 4px;
    font-weight: 500;
  }

  .tag-purple { background: #2D1B69; color: var(--purple); }
  .tag-cyan   { background: #083344; color: var(--cyan); }
  .tag-green  { background: #0D2818; color: var(--green); }
  .tag-orange { background: #2C1A06; color: var(--orange); }
  .tag-pink   { background: #2D1130; color: var(--pink); }
  .tag-yellow { background: #2D1F00; color: var(--yellow); }
  .tag-gray   { background: var(--surface2); color: var(--muted); }

  /* ── EXPERIENCE ── */
  .timeline {
    position: relative;
    padding-left: 24px;
  }

  .timeline::before {
    content: '';
    position: absolute;
    left: 6px;
    top: 0;
    bottom: 0;
    width: 1px;
    background: linear-gradient(to bottom, var(--purple), var(--border));
  }

  .timeline-item {
    position: relative;
    margin-bottom: 28px;
  }

  .timeline-item::before {
    content: '';
    position: absolute;
    left: -21px;
    top: 6px;
    width: 9px;
    height: 9px;
    border-radius: 50%;
    border: 2px solid var(--purple);
    background: var(--bg);
  }

  .tl-header {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    gap: 12px;
    flex-wrap: wrap;
    margin-bottom: 4px;
  }

  .tl-role {
    font-weight: 600;
    font-size: 14.5px;
    color: var(--text);
  }

  .tl-date {
    font-family: var(--font-mono);
    font-size: 11.5px;
    color: var(--muted);
    white-space: nowrap;
  }

  .tl-org {
    font-size: 13px;
    color: var(--purple);
    font-weight: 500;
    margin-bottom: 6px;
  }

  .tl-desc {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.65;
  }

  /* ── CERTIFICATIONS ── */
  .certs-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 12px;
  }

  .cert-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 16px 18px;
    display: flex;
    align-items: center;
    gap: 14px;
  }

  .cert-icon {
    width: 42px;
    height: 42px;
    border-radius: 8px;
    background: #1A1136;
    border: 1px solid var(--purple-dim);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 22px;
    flex-shrink: 0;
  }

  .cert-name {
    font-size: 13.5px;
    font-weight: 600;
    color: var(--text);
    margin-bottom: 3px;
  }

  .cert-org {
    font-family: var(--font-mono);
    font-size: 11.5px;
    color: var(--purple);
  }

  /* ── STATS ── */
  .stats-row {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
    gap: 12px;
    margin-bottom: 20px;
  }

  .stat-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 16px;
    text-align: center;
  }

  .stat-num {
    font-family: var(--font-mono);
    font-size: 28px;
    font-weight: 700;
    background: linear-gradient(135deg, var(--purple), var(--cyan));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .stat-label {
    font-size: 12px;
    color: var(--muted);
    margin-top: 4px;
  }

  /* ── CONTACT ── */
  .contact-row {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    justify-content: center;
  }

  .contact-btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 9px 18px;
    border-radius: 8px;
    font-size: 13.5px;
    font-family: var(--font-mono);
    text-decoration: none;
    border: 1px solid;
    transition: all 0.2s;
    color: inherit;
  }

  .contact-btn:hover { transform: translateY(-1px); }
  .btn-purple { background: #2D1B69; border-color: var(--purple); color: var(--purple); }
  .btn-cyan   { background: #083344; border-color: var(--cyan);   color: var(--cyan); }
  .btn-gray   { background: var(--surface); border-color: var(--border); color: var(--muted); }
  .btn-purple:hover { background: #3D2480; }
  .btn-cyan:hover   { background: #0C4460; }
  .btn-gray:hover   { background: var(--surface2); color: var(--text); }

  /* ── FOOTER ── */
  .footer {
    text-align: center;
    padding: 32px 0 16px;
    border-top: 1px solid var(--border);
    margin-top: 48px;
  }

  .footer-text {
    font-family: var(--font-mono);
    font-size: 12px;
    color: var(--muted);
  }

  .footer-text span { color: var(--purple); }

  /* ── ANIMATIONS ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  .readme > * {
    animation: fadeUp 0.4s ease both;
  }
  .readme > *:nth-child(1) { animation-delay: 0.05s; }
  .readme > *:nth-child(2) { animation-delay: 0.1s; }
  .readme > *:nth-child(3) { animation-delay: 0.15s; }
  .readme > *:nth-child(4) { animation-delay: 0.2s; }
  .readme > *:nth-child(5) { animation-delay: 0.25s; }
  .readme > *:nth-child(6) { animation-delay: 0.3s; }
  .readme > *:nth-child(7) { animation-delay: 0.35s; }
  .readme > *:nth-child(8) { animation-delay: 0.4s; }

  /* ── RESPONSIVE ── */
  @media (max-width: 480px) {
    .readme { padding: 24px 16px 60px; }
    .hero { padding: 28px 0 24px; }
  }
</style>
</head>
<body>

<button id="copy-btn" onclick="copyMarkdown()">📋 Copy as Markdown</button>

<div class="readme">

  <!-- HERO -->
  <div class="hero">
    <p class="hero-greeting">👋 Hey there, I'm</p>
    <h1 class="hero-name">Fatma Zahra Dorgham</h1>
    <p class="hero-title">
      AI Engineering Student &nbsp;·&nbsp; <span>ESPRIT Tunis</span> &nbsp;·&nbsp; Full-Stack × ML
    </p>
  </div>

  <!-- TERMINAL -->
  <div class="terminal">
    <div class="terminal-bar">
      <div class="terminal-dot dot-red"></div>
      <div class="terminal-dot dot-yellow"></div>
      <div class="terminal-dot dot-green"></div>
      <span class="terminal-title">fatma@esprit ~ profile.json</span>
    </div>
    <div class="terminal-body">
      <span class="t-prompt">→</span> <span class="t-cmd">cat</span> me.json<br>
      {<br>
      &nbsp;&nbsp;<span class="t-key">"name"</span>: <span class="t-str">"Fatma Zahra Dorgham"</span>,<br>
      &nbsp;&nbsp;<span class="t-key">"role"</span>: <span class="t-str">"AI Engineering Student @ ESPRIT"</span>,<br>
      &nbsp;&nbsp;<span class="t-key">"location"</span>: <span class="t-str">"Tunis, Tunisia 🇹🇳"</span>,<br>
      &nbsp;&nbsp;<span class="t-key">"focus"</span>: [<span class="t-str">"AI"</span>, <span class="t-str">"Computer Vision"</span>, <span class="t-str">"NLP"</span>, <span class="t-str">"Full-Stack"</span>],<br>
      &nbsp;&nbsp;<span class="t-key">"currently"</span>: <span class="t-str">"Building intelligent systems at ESPRIT"</span>,<br>
      &nbsp;&nbsp;<span class="t-key">"languages"</span>: [<span class="t-str">"Python"</span>, <span class="t-str">"Java"</span>, <span class="t-str">"C"</span>, <span class="t-str">"C++"</span>, <span class="t-str">"PHP"</span>],<br>
      &nbsp;&nbsp;<span class="t-key">"seeking"</span>: <span class="t-str">"Internship in AI / Full-Stack Dev"</span><br>
      } <span class="t-cursor"></span>
    </div>
  </div>

  <!-- BADGES -->
  <div class="badges">
    <span class="badge badge-purple">🧠 Machine Learning</span>
    <span class="badge badge-cyan">👁️ Computer Vision</span>
    <span class="badge badge-purple">💬 NLP & LLMs</span>
    <span class="badge badge-cyan">⚡ Generative AI</span>
    <span class="badge badge-green">🚀 Flask · Django · React</span>
    <span class="badge badge-orange">🐧 Linux · Docker</span>
    <span class="badge badge-green">📊 Power BI · SQL Server</span>
  </div>

  <!-- ABOUT -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">👩‍💻</span>
      <span class="section-title">about_me</span>
      <div class="section-line"></div>
    </div>
    <div class="about-grid">
      <div class="about-card">
        <span class="about-icon">🎓</span>
        <div>
          <div class="about-label">Education</div>
          <div class="about-value">Cycle Ingénieur – IA<br>ESPRIT, 2023 – Present</div>
        </div>
      </div>
      <div class="about-card">
        <span class="about-icon">📍</span>
        <div>
          <div class="about-label">Location</div>
          <div class="about-value">Tunis, Tunisia 🇹🇳</div>
        </div>
      </div>
      <div class="about-card">
        <span class="about-icon">🔭</span>
        <div>
          <div class="about-label">Currently Building</div>
          <div class="about-value">AI-powered SaaS platforms with RAG & LLMs</div>
        </div>
      </div>
      <div class="about-card">
        <span class="about-icon">🌱</span>
        <div>
          <div class="about-label">Always Learning</div>
          <div class="about-value">Diffusion Models, Generative AI, MLOps</div>
        </div>
      </div>
      <div class="about-card">
        <span class="about-icon">💼</span>
        <div>
          <div class="about-label">Open To</div>
          <div class="about-value">AI/ML Internships & Full-Stack Roles</div>
        </div>
      </div>
      <div class="about-card">
        <span class="about-icon">✉️</span>
        <div>
          <div class="about-label">Reach Me</div>
          <div class="about-value">dorgham.fatmaa@gmail.com</div>
        </div>
      </div>
    </div>
  </div>

  <!-- SKILLS -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">⚙️</span>
      <span class="section-title">tech_stack</span>
      <div class="section-line"></div>
    </div>
    <div class="skills-grid">
      <div class="skill-category">
        <div class="skill-cat-header">
          <div class="skill-cat-dot" style="background: var(--purple)"></div>
          <span class="skill-cat-name" style="color: var(--purple)">AI & ML</span>
        </div>
        <div class="skill-list">
          <span class="skill-tag">Machine Learning</span>
          <span class="skill-tag">Deep Learning</span>
          <span class="skill-tag">Computer Vision</span>
          <span class="skill-tag">NLP</span>
          <span class="skill-tag">LLMs</span>
          <span class="skill-tag">RAG</span>
          <span class="skill-tag">Generative AI</span>
        </div>
      </div>
      <div class="skill-category">
        <div class="skill-cat-header">
          <div class="skill-cat-dot" style="background: var(--cyan)"></div>
          <span class="skill-cat-name" style="color: var(--cyan)">Languages</span>
        </div>
        <div class="skill-list">
          <span class="skill-tag">Python</span>
          <span class="skill-tag">Java</span>
          <span class="skill-tag">C</span>
          <span class="skill-tag">C++</span>
          <span class="skill-tag">PHP</span>
          <span class="skill-tag">JavaScript</span>
          <span class="skill-tag">HTML5</span>
          <span class="skill-tag">CSS</span>
        </div>
      </div>
      <div class="skill-category">
        <div class="skill-cat-header">
          <div class="skill-cat-dot" style="background: var(--green)"></div>
          <span class="skill-cat-name" style="color: var(--green)">Frameworks</span>
        </div>
        <div class="skill-list">
          <span class="skill-tag">Flask</span>
          <span class="skill-tag">Django</span>
          <span class="skill-tag">React.js</span>
          <span class="skill-tag">Bootstrap</span>
          <span class="skill-tag">jQuery</span>
        </div>
      </div>
      <div class="skill-category">
        <div class="skill-cat-header">
          <div class="skill-cat-dot" style="background: var(--orange)"></div>
          <span class="skill-cat-name" style="color: var(--orange)">Data & BI</span>
        </div>
        <div class="skill-list">
          <span class="skill-tag">SQL Server</span>
          <span class="skill-tag">MySQL</span>
          <span class="skill-tag">SSIS</span>
          <span class="skill-tag">Power BI</span>
          <span class="skill-tag">DAX</span>
        </div>
      </div>
      <div class="skill-category">
        <div class="skill-cat-header">
          <div class="skill-cat-dot" style="background: var(--pink)"></div>
          <span class="skill-cat-name" style="color: var(--pink)">DevOps & Tools</span>
        </div>
        <div class="skill-list">
          <span class="skill-tag">Git</span>
          <span class="skill-tag">Docker</span>
          <span class="skill-tag">Linux</span>
          <span class="skill-tag">VS Code</span>
          <span class="skill-tag">Colab</span>
          <span class="skill-tag">Kaggle</span>
        </div>
      </div>
      <div class="skill-category">
        <div class="skill-cat-header">
          <div class="skill-cat-dot" style="background: var(--yellow)"></div>
          <span class="skill-cat-name" style="color: var(--yellow)">Methodology</span>
        </div>
        <div class="skill-list">
          <span class="skill-tag">SCRUM</span>
          <span class="skill-tag">Agile</span>
          <span class="skill-tag">ETL Pipelines</span>
          <span class="skill-tag">FlutterFlow</span>
        </div>
      </div>
    </div>
  </div>

  <!-- STATS -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">📈</span>
      <span class="section-title">by_the_numbers</span>
      <div class="section-line"></div>
    </div>
    <div class="stats-row">
      <div class="stat-card">
        <div class="stat-num">6+</div>
        <div class="stat-label">Academic Projects</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">2</div>
        <div class="stat-label">NVIDIA Certifications</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">2</div>
        <div class="stat-label">Industry Internships</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">3+</div>
        <div class="stat-label">Years Coding</div>
      </div>
    </div>
  </div>

  <!-- PROJECTS -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">🚀</span>
      <span class="section-title">featured_projects</span>
      <div class="section-line"></div>
    </div>
    <div class="projects-grid">

      <div class="project-card proj-purple">
        <div class="proj-header">
          <span class="proj-icon">🧠</span>
          <span class="proj-name">SCALEUP</span>
        </div>
        <p class="proj-desc">AI-powered SaaS platform helping startup founders structure and validate their projects. Combines CV, OCR, NLP & LLMs to auto-generate Business Model Canvases.</p>
        <div class="proj-tags">
          <span class="proj-tag tag-purple">LLMs</span>
          <span class="proj-tag tag-purple">RAG</span>
          <span class="proj-tag tag-cyan">Computer Vision</span>
          <span class="proj-tag tag-gray">Flask</span>
          <span class="proj-tag tag-gray">React.js</span>
        </div>
      </div>

      <div class="project-card proj-orange">
        <div class="proj-header">
          <span class="proj-icon">📊</span>
          <span class="proj-name">NAPOLEON</span>
        </div>
        <p class="proj-desc">Data engineering & BI platform analyzing associations in Île-de-France. Full ETL pipeline, Data Warehouse, Power BI dashboards, and ML models (GMM, XGBoost).</p>
        <div class="proj-tags">
          <span class="proj-tag tag-orange">Power BI</span>
          <span class="proj-tag tag-orange">XGBoost</span>
          <span class="proj-tag tag-gray">SSIS</span>
          <span class="proj-tag tag-gray">Django</span>
          <span class="proj-tag tag-gray">Python</span>
        </div>
      </div>

      <div class="project-card proj-cyan">
        <div class="proj-header">
          <span class="proj-icon">🐾</span>
          <span class="proj-name">PETORIA</span>
        </div>
        <p class="proj-desc">Animal welfare web app with vet appointment scheduling, a symptom-based chatbot assistant, and a Deep Learning CNN model for medical image analysis.</p>
        <div class="proj-tags">
          <span class="proj-tag tag-cyan">Deep Learning</span>
          <span class="proj-tag tag-cyan">CNN</span>
          <span class="proj-tag tag-gray">Django</span>
          <span class="proj-tag tag-gray">Python</span>
        </div>
      </div>

      <div class="project-card proj-green">
        <div class="proj-header">
          <span class="proj-icon">⚽</span>
          <span class="proj-name">TAKWIRA</span>
        </div>
        <p class="proj-desc">Desktop app for managing football matches and competitions. Features an interactive OpenStreetMap integration and Arduino-based QR code access control at stadiums.</p>
        <div class="proj-tags">
          <span class="proj-tag tag-green">C++</span>
          <span class="proj-tag tag-green">Qt</span>
          <span class="proj-tag tag-gray">Arduino</span>
          <span class="proj-tag tag-gray">MySQL</span>
        </div>
      </div>

      <div class="project-card proj-yellow">
        <div class="proj-header">
          <span class="proj-icon">🌿</span>
          <span class="proj-name">GREEN&GO</span>
        </div>
        <p class="proj-desc">Web platform connecting farmers and consumers directly. Full CRUD system, OpenStreetMap for locating points of sale, and QR-code ticket generation for agricultural events.</p>
        <div class="proj-tags">
          <span class="proj-tag tag-yellow">PHP</span>
          <span class="proj-tag tag-yellow">MySQL</span>
          <span class="proj-tag tag-gray">JavaScript</span>
          <span class="proj-tag tag-gray">OpenStreetMap</span>
        </div>
      </div>

      <div class="project-card proj-pink">
        <div class="proj-header">
          <span class="proj-icon">⚔️</span>
          <span class="proj-name">LEGACY OF JUSTICE</span>
        </div>
        <p class="proj-desc">2D game built in C with SDL1.2. Custom game engine with collision detection, sprite animation, score management, and multi-level gameplay logic.</p>
        <div class="proj-tags">
          <span class="proj-tag tag-pink">C</span>
          <span class="proj-tag tag-pink">SDL 1.2</span>
          <span class="proj-tag tag-gray">Game Dev</span>
          <span class="proj-tag tag-gray">Git</span>
        </div>
      </div>

    </div>
  </div>

  <!-- EXPERIENCE -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">💼</span>
      <span class="section-title">experience</span>
      <div class="section-line"></div>
    </div>
    <div class="timeline">
      <div class="timeline-item">
        <div class="tl-header">
          <span class="tl-role">Software Engineering Intern</span>
          <span class="tl-date">Jul – Aug 2025</span>
        </div>
        <div class="tl-org">Orange Tunisie · Tunis</div>
        <p class="tl-desc">Explored enterprise network infrastructure and technical operations. Worked with Linux virtual machines, containerization with Docker, and contributed to development tasks in a professional tech environment.</p>
      </div>
      <div class="timeline-item">
        <div class="tl-header">
          <span class="tl-role">Software Engineering Intern</span>
          <span class="tl-date">Jul – Aug 2024</span>
        </div>
        <div class="tl-org">Farouk Abdelkarim Consulting · Tunis</div>
        <p class="tl-desc">Participated in an Agile software project using React.js and Flutter. Gained hands-on experience with professional tools (VS Code, Git, Trello, PostgreSQL), sprint ceremonies, and team collaboration in a real consulting environment.</p>
      </div>
    </div>
  </div>

  <!-- CERTIFICATIONS -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">🏆</span>
      <span class="section-title">certifications</span>
      <div class="section-line"></div>
    </div>
    <div class="certs-grid">
      <div class="cert-card">
        <div class="cert-icon">🟢</div>
        <div>
          <div class="cert-name">Fundamentals of Deep Learning</div>
          <div class="cert-org">NVIDIA Deep Learning Institute · 2025</div>
        </div>
      </div>
      <div class="cert-card">
        <div class="cert-icon">🟢</div>
        <div>
          <div class="cert-name">Generative AI with Diffusion Models</div>
          <div class="cert-org">NVIDIA Deep Learning Institute · 2026</div>
        </div>
      </div>
    </div>
  </div>

  <!-- CONTACT -->
  <div class="section">
    <div class="section-header">
      <span class="section-icon">📬</span>
      <span class="section-title">get_in_touch</span>
      <div class="section-line"></div>
    </div>
    <div class="contact-row">
      <a href="mailto:dorgham.fatmaa@gmail.com" class="contact-btn btn-purple">✉️ Email Me</a>
      <a href="https://linkedin.com/in/fatma-zahra-dorgham" class="contact-btn btn-cyan" target="_blank">💼 LinkedIn</a>
      <a href="tel:+21654122877" class="contact-btn btn-gray">📞 +216 54 122 877</a>
    </div>
  </div>

  <!-- FOOTER -->
  <div class="footer">
    <p class="footer-text">
      Made with <span>♥</span> in Tunis &nbsp;·&nbsp; Always building, always learning &nbsp;·&nbsp;
      <span>open to opportunities</span>
    </p>
  </div>

</div>

<script>
function copyMarkdown() {
  const md = `# Hi there, I'm Fatma Zahra Dorgham 👋

> **AI Engineering Student · ESPRIT Tunis · Full-Stack × ML**

\`\`\`json
{
  "name": "Fatma Zahra Dorgham",
  "role": "AI Engineering Student @ ESPRIT",
  "location": "Tunis, Tunisia 🇹🇳",
  "focus": ["AI", "Computer Vision", "NLP", "Full-Stack"],
  "currently": "Building intelligent systems at ESPRIT",
  "seeking": "Internship in AI / Full-Stack Dev"
}
\`\`\`

---

## 👩‍💻 About Me

- 🎓 Cycle Ingénieur – IA at **ESPRIT** (2023 – Present)
- 📍 Based in **Tunis, Tunisia**
- 🔭 Currently building AI-powered SaaS platforms with RAG & LLMs
- 🌱 Always learning: Diffusion Models, Generative AI, MLOps
- 💼 Open to AI/ML internships & Full-Stack roles
- ✉️ Reach me: **dorgham.fatmaa@gmail.com**

---

## ⚙️ Tech Stack

**AI & ML**  
\`Machine Learning\` \`Deep Learning\` \`Computer Vision\` \`NLP\` \`LLMs\` \`RAG\` \`Generative AI\`

**Languages**  
\`Python\` \`Java\` \`C\` \`C++\` \`PHP\` \`JavaScript\` \`HTML5\` \`CSS\`

**Frameworks**  
\`Flask\` \`Django\` \`React.js\` \`Bootstrap\` \`jQuery\`

**Data & BI**  
\`SQL Server\` \`MySQL\` \`SSIS\` \`Power BI\` \`DAX\`

**DevOps & Tools**  
\`Git\` \`Docker\` \`Linux\` \`VS Code\` \`Google Colab\` \`Kaggle\`

---

## 🚀 Featured Projects

| Project | Description | Stack |
|---------|------------|-------|
| **SCALEUP** 🧠 | AI SaaS platform for startups – auto-generates Business Model Canvas using CV, OCR, NLP & LLMs | Python, Flask, React, RAG, LLMs |
| **NAPOLEON** 📊 | Data engineering & BI platform with ETL pipeline, Data Warehouse & ML models (GMM, XGBoost) | Python, SSIS, Power BI, Django |
| **PETORIA** 🐾 | Animal welfare app with vet scheduling, symptom chatbot & CNN medical image analysis | Python, Django, Deep Learning |
| **TAKWIRA** ⚽ | Desktop football management app with interactive maps & Arduino QR-code access control | C++, Qt, MySQL, Arduino |
| **GREEN&GO** 🌿 | Farm-to-consumer web platform with CRUD, geolocation & QR ticket generation | PHP, MySQL, JavaScript |
| **Legacy of Justice** ⚔️ | 2D game with custom engine, collision detection & multi-level gameplay | C, SDL 1.2 |

---

## 💼 Experience

**Software Engineering Intern** · Orange Tunisie *(Jul–Aug 2025)*  
Linux VMs, Docker containerization, enterprise network infrastructure & development tasks.

**Software Engineering Intern** · Farouk Abdelkarim Consulting *(Jul–Aug 2024)*  
Agile project with React.js & Flutter, Git, PostgreSQL, sprint ceremonies & team collaboration.

---

## 🏆 Certifications

- 🟢 **Fundamentals of Deep Learning** – NVIDIA DLI, 2025
- 🟢 **Generative AI with Diffusion Models** – NVIDIA DLI, 2026

---

## 🌍 Languages

- 🇹🇳 Arabic – Native
- 🇫🇷 French – B2
- 🇬🇧 English – B2

---

## 📬 Get In Touch

[![Email](https://img.shields.io/badge/Email-dorgham.fatmaa%40gmail.com-purple?style=flat-square&logo=gmail)](mailto:dorgham.fatmaa@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-fatma--zahra--dorgham-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/fatma-zahra-dorgham)

---

*Made with ♥ in Tunis · Always building, always learning · Open to opportunities*
`;

  navigator.clipboard.writeText(md).then(() => {
    const btn = document.getElementById('copy-btn');
    btn.textContent = '✅ Copied!';
    btn.classList.add('copied');
    setTimeout(() => {
      btn.textContent = '📋 Copy as Markdown';
      btn.classList.remove('copied');
    }, 2500);
  });
}
</script>

</body>
</html>
