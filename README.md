<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rainier | Cloud & Automation Engineer</title>
  <meta name="description" content="Cloud enthusiast focused on Infrastructure Automation, Kubernetes, Azure, and scalable platform engineering." />
  <meta name="author" content="Rainier" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #0e1116;
      --bg-alt: #161b22;
      --bg-soft: #1f242c;
      --text: #dbe2ec;
      --text-dim: #9aa4b1;
      --accent: #3b82f6;
      --accent-accent: #60a5fa;
      --gradient: linear-gradient(135deg,#3b82f6,#6366f1 55%,#8b5cf6);
      --radius: 14px;
      --code: #1b2330;
      --callout: #10253d;
      --success: #10b981;
      --danger: #ef4444;
      --warn: #f59e0b;
      font-size: 16px;
    }
    [data-theme="light"] {
      --bg: #f8fafc;
      --bg-alt: #ffffff;
      --bg-soft: #f1f5f9;
      --text: #1e293b;
      --text-dim: #475569;
      --code: #f1f5f9;
      --callout: #e0f2fe;
    }
    * { box-sizing: border-box; }
    body { margin:0; font-family: 'Inter', system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', Helvetica, Arial, sans-serif; background: var(--bg); color: var(--text); -webkit-font-smoothing: antialiased; }
    a { color: var(--accent); text-decoration: none; }
    a:hover { color: var(--accent-accent); }
    header.hero { padding: 4.5rem 1.25rem 3rem; text-align:center; position:relative; overflow:hidden; }
    header.hero::before { content:""; position:absolute; inset:0; background:radial-gradient(circle at 50% 30%, rgba(99,102,241,0.35), transparent 70%); pointer-events:none; }
    .hero-inner { max-width:900px; margin:0 auto; position:relative; }
    .badge-row { display:flex; flex-wrap:wrap; gap:.5rem; justify-content:center; margin:1.75rem auto 0; }
    .badge { padding:.45rem .75rem; background:var(--bg-soft); border:1px solid #27313d; font-size:.75rem; letter-spacing:.05em; text-transform:uppercase; border-radius:999px; font-weight:600; color:var(--text-dim); display:inline-flex; align-items:center; gap:.4rem; }
    h1.gradient { font-size:clamp(2.2rem,5.5vw,3.4rem); margin:0 0 .85rem; line-height:1.1; background:var(--gradient); -webkit-background-clip:text; color:transparent; font-weight:700; }
    h2.subtitle { font-weight:600; margin:0 0 1.1rem; font-size:clamp(1.05rem,2.4vw,1.35rem); color:var(--text-dim); }
    p.lead { font-size:1.05rem; max-width:780px; margin:0 auto; line-height:1.6; }
    nav.quick { margin-top:2.75rem; display:flex; justify-content:center; gap:.75rem; flex-wrap:wrap; }
    nav.quick a { background:var(--bg-soft); border:1px solid #27313d; padding:.65rem 1rem; border-radius:var(--radius); font-size:.8rem; font-weight:500; letter-spacing:.03em; position:relative; }
    nav.quick a:hover { background:#243042; }
    main { max-width:1060px; margin:0 auto; padding:0 1.25rem 4rem; }
    section { margin:3.25rem 0; }
    section:first-of-type { margin-top:0; }
    h3.section-title { font-size:1.15rem; letter-spacing:.07em; text-transform:uppercase; font-weight:700; margin:0 0 1.25rem; color:var(--accent-accent); display:flex; align-items:center; gap:.6rem; }
    h3.section-title span.emoji { filter: grayscale(10%) brightness(1.1); }
    .card-grid { display:grid; gap:1rem; grid-template-columns:repeat(auto-fit,minmax(240px,1fr)); }
    .info-card { background:var(--bg-alt); padding:1rem 1.1rem 1.15rem; border:1px solid #202a35; border-radius:var(--radius); position:relative; overflow:hidden; }
    .info-card::before { content:""; position:absolute; inset:0; background:linear-gradient(145deg,rgba(59,130,246,.08),transparent 60%); pointer-events:none; }
    .info-card h4 { margin:.15rem 0 .5rem; font-size:.95rem; font-weight:600; }
    .info-card p { margin:0; font-size:.8rem; line-height:1.4; color:var(--text-dim); }
    ul.inline-list { list-style:none; padding:0; margin:.25rem 0 0; display:flex; flex-wrap:wrap; gap:.5rem .85rem; font-size:.8rem; }
    ul.inline-list li { background:var(--bg-alt); border:1px solid #283341; padding:.4rem .7rem; border-radius:8px; font-weight:500; }
    .two-col { display:grid; gap:2.4rem; grid-template-columns:repeat(auto-fit,minmax(300px,1fr)); align-items:start; }
    .proj-list { list-style:none; margin:0; padding:0; display:flex; flex-direction:column; gap:1rem; }
    .proj { background:var(--bg-alt); border:1px solid #202a35; border-radius:var(--radius); padding:1rem 1.15rem 1.2rem; position:relative; overflow:hidden; }
    .proj::before { content:""; position:absolute; inset:0; background:linear-gradient(120deg, rgba(96,165,250,.10), transparent 55%); }
    .proj h4 { margin:0 0 .4rem; font-size:.9rem; font-weight:600; letter-spacing:.03em; }
    .proj p { margin:0; font-size:.78rem; line-height:1.45; color:var(--text-dim); }
    .contact { display:flex; flex-wrap:wrap; gap:1rem; }
    .contact a.btn { background:var(--gradient); color:#fff; padding:.85rem 1.2rem; border-radius:var(--radius); font-weight:600; font-size:.85rem; letter-spacing:.03em; display:inline-flex; gap:.55rem; align-items:center; box-shadow:0 4px 22px -6px rgba(99,102,241,.5); }
    .contact a.btn.secondary { background:var(--bg-alt); color:var(--text); box-shadow:none; border:1px solid #2a3644; }
    .contact a.btn.secondary:hover { background:#273240; }
    footer { margin:4rem 0 0; padding:2rem 1rem 3rem; text-align:center; font-size:.7rem; color:var(--text-dim); }
    hr.sep { border:0; height:1px; background:linear-gradient(90deg, transparent, #2b3847, transparent); margin:3.5rem 0 2.75rem; }
    .fade { animation: fadeIn .8s cubic-bezier(.4,0,.2,1); }
    @keyframes fadeIn { from { opacity:0; transform: translateY(6px); } to { opacity:1; transform: none; } }
    /* Dark mode toggle */
    .theme-toggle { position:fixed; top:1rem; right:1rem; z-index:50; }
    .theme-toggle button { background:var(--bg-alt); color:var(--text-dim); border:1px solid #2b3644; border-radius:999px; padding:.55rem .95rem; font-size:.7rem; font-weight:600; letter-spacing:.07em; cursor:pointer; display:inline-flex; align-items:center; gap:.35rem; }
    .theme-toggle button:hover { color:var(--text); }
    code { font-family: ui-monospace, SFMono-Regular, 'SF Mono', Menlo, Consolas, 'Liberation Mono', monospace; background:var(--code); padding:.15rem .35rem; border-radius:6px; font-size:.75rem; }
    @media (max-width:640px) { header.hero { padding:3.5rem 1rem 2.5rem; } .contact a.btn { flex:1 1 auto; justify-content:center; } }
  </style>
</head>
<body>
  <div class="theme-toggle">
    <button id="themeButton" aria-label="Toggle theme" title="Toggle light/dark mode">🌗 <span id="themeLabel">Dark</span></button>
  </div>
  <header class="hero fade">
    <div class="hero-inner">
      <h1 class="gradient">Hi, I'm Rainier <span aria-hidden="true">👋</span></h1>
      <h2 class="subtitle">☁ Cloud & DevOps Specialist | ⚙ Infrastructure & Automation</h2>
      <p class="lead">I’m a cloud enthusiast, engineer, and problem solver passionate about building efficient, scalable solutions. From cloud architecture to scripting and automation, I love simplifying complexity and enabling teams to deliver faster, safer, and repeatable outcomes. Deeply into <strong>Cloud Infrastructure</strong> & <strong>Infrastructure Automation</strong>.</p>
      <div class="badge-row">
        <div class="badge">Azure</div>
        <div class="badge">Kubernetes</div>
        <div class="badge">Terraform</div>
        <div class="badge">Platform Automation</div>
        <div class="badge">DevOps</div>
        <div class="badge">Infrastructure</div>
      </div>
      <nav class="quick" aria-label="Quick navigation">
        <a href="#journey">Journey</a>
        <a href="#tech">Tech</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>
  <main>
    <section id="journey" class="fade">
      <h3 class="section-title"><span class="emoji">🌐</span> Explore My Journey</h3>
      <div class="two-col">
        <div>
          <p>Find me on LinkedIn or via my portfolio.</p>
          <div class="info-card">
            <h4>Online Profiles</h4>
            <p>
              <a href="https://rainier.cloudkid.link" rel="noopener" target="_blank">Portfolio</a>
              &nbsp;•&nbsp;
              <a href="https://www.linkedin.com/in/rainier-cloudkid/" rel="noopener" target="_blank">LinkedIn</a>
            </p>
          </div>
        </div>
        <div>
          <div class="info-card">
            <h4>Technologies</h4>
            <ul class="inline-list">
              <li>Cloudflare</li>
              <li>Automation Pipelines</li>
              <li>Cloud Architecture</li>
              <li>Observability</li>
              <li>Security Posture</li>
              <li>Platform Enablement</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  <section id="tech" class="fade">
    <h3 class="section-title"><span class="emoji">🔧</span> Tech</h3>
    <div class="two-col">
      <div>
        <div class="info-card">
          <h4>Cloud & Platforms</h4>
          <p>Azure · AWS · GitHub · Cloudflare · GCP · Digital Ocean · Linode (Akamai Cloud)</p>
        </div>
        <div class="info-card" style="margin-top:1rem;">
          <h4>Infrastructure & Automation</h4>
          <p>Terraform · Ansible · Jenkins · Cloudflare Workers · Kubernetes</p>
        </div>
      </div>
      <div>
        <div class="info-card">
          <h4>Languages & Tooling</h4>
          <p>PowerShell · NodeJS · C# · Scriban</p>
        </div>
        <div class="info-card" style="margin-top:1rem;">
          <h4>Focus Areas</h4>
          <ul class="inline-list">
            <li>Infrastructure & Automation</li>
            <li>Observability</li>
            <li>Security & Posture</li>
            <li>Platform Enablement</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <section id="projects" class="fade">
    <h3 class="section-title"><span class="emoji">💡</span> Projects</h3>
    <div class="proj-list">
      <a href="https://korbanministries.co.za/" target="_blank" rel="noopener"><div class="proj">
        <h4>Korban Ministries</h4>
        <p>Online Gospel Ministry platform (content & delivery infrastructure).</p>
      </div></a>
      <a href="https://online.cloudkid.link/" target="_blank" rel="noopener"><div class="proj">
        <h4>Webinar Platform</h4>
        <p>Self-hosted webinar/event delivery site (automation & reliability focus).</p>
      </div></a>
      <a href="https://wedding.cloudkid.link/" target="_blank" rel="noopener"><div class="proj" >
        <h4>Wedding Photo Gallery</h4>
        <p>Static optimized media gallery hosted via edge delivery.</p>
      </div></a>
    </div>
  </section>

  <section id="contact" class="fade">
    <h3 class="section-title"><span class="emoji">💬</span> Contact</h3>
    <p>Best ways to reach me for collaboration or opportunities:</p>
    <div class="contact">
      <a class="btn" href="https://www.linkedin.com/in/rainier-cloudkid/" target="_blank" rel="noopener">LinkedIn</a>
      <a class="btn secondary" href="mailto:rainier@cloudkid.link" rel="nofollow noopener">Email</a>
      <a class="btn secondary" href="https://rainier.cloudkid.link" target="_blank" rel="noopener">Portfolio</a>
    </div>
  </section>
  </main>
  <footer>
    <p><span id="year"></span> • Crafted with automation mindset ⚙️</p>
  </footer>
  <script>
    (function(){
      const root = document.documentElement;
      const btn = document.getElementById('themeButton');
      const label = document.getElementById('themeLabel');
      const stored = localStorage.getItem('theme-pref');
      if(stored){ root.setAttribute('data-theme', stored); label.textContent = stored === 'dark' ? 'Dark' : 'Light'; }
      btn.addEventListener('click', () => {
        const current = root.getAttribute('data-theme') || 'dark';
        const next = current === 'dark' ? 'light' : 'dark';
        root.setAttribute('data-theme', next);
        localStorage.setItem('theme-pref', next);
        label.textContent = next === 'dark' ? 'Dark' : 'Light';
      });
      document.getElementById('year').textContent = new Date().getFullYear();
    })();
  </script>
</body>
</html>
