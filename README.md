<!--
Academic GitHub Page Template (single-file)
Save this file as `index.html` in your GitHub Pages repo (e.g. `username.github.io`) or in a docs/ folder.
Customize the content blocks (ABOUT, RESEARCH, PUBLICATIONS, TEACHING, CV, CONTACT).
No build step required — plain HTML/CSS/JS.
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Your Name — Researcher | Academic Page</title>
  <meta name="description" content="Personal academic page for Your Name — research, publications, teaching, and contact." />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>📚</text></svg>">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa6b2; --accent:#7dd3fc;
      --glass: rgba(255,255,255,0.03);
      --maxw:1100px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background:linear-gradient(180deg,#071126 0%, #071821 100%);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding:32px 16px;
      display:flex;justify-content:center;
    }
    .container{width:100%;max-width:var(--maxw)}
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
    .brand{display:flex;gap:16px;align-items:center}
    .avatar{width:72px;height:72px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#60a5fa);display:flex;align-items:center;justify-content:center;font-weight:700;font-size:28px}
    h1{margin:0;font-size:24px}
    p.lead{margin:0;color:var(--muted)}

    nav{display:flex;gap:10px}
    .nav-btn{background:transparent;border:1px solid rgba(255,255,255,0.05);padding:8px 12px;border-radius:10px;color:var(--muted);cursor:pointer}
    .nav-btn.active{border-color:rgba(125,211,252,0.18);color:var(--accent)}

    .grid{display:grid;grid-template-columns: 1fr 340px;gap:22px}
    @media (max-width:900px){.grid{grid-template-columns:1fr}}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:14px;padding:18px;border:1px solid rgba(255,255,255,0.03)}
    .section-title{display:flex;align-items:center;gap:8px;margin-bottom:12px}
    .section-title h2{margin:0;font-size:18px}
    .meta{color:var(--muted);font-size:14px}

    /* Publications list */
    .pub{padding:12px;border-radius:10px;margin-bottom:10px;background:var(--glass);border:1px solid rgba(255,255,255,0.02)}
    .pub h3{margin:0;font-size:15px}
    .pub .info{color:var(--muted);font-size:13px;margin-top:6px}

    /* Right column */
    .profile-meta{display:flex;flex-direction:column;gap:12px}
    .chips{display:flex;flex-wrap:wrap;gap:8px}
    .chip{padding:8px 10px;border-radius:999px;border:1px solid rgba(255,255,255,0.03);background:rgba(255,255,255,0.02);font-size:13px}

    /* simple search / filter */
    .search{display:flex;gap:8px}
    .search input{flex:1;padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}
    .search button{padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:var(--muted)}

    footer{margin-top:26px;color:var(--muted);font-size:13px;text-align:center}
    a{color:inherit}

    .btn-primary{background:linear-gradient(90deg,#7dd3fc,#60a5fa);color:#04263b;padding:10px 14px;border-radius:10px;border:none;cursor:pointer}

    /* timeline / teaching */
    .teach-list{display:flex;flex-direction:column;gap:8px}
    .teach-item{padding:10px;border-radius:8px;background:rgba(255,255,255,0.015);border:1px solid rgba(255,255,255,0.02)}

    /* small helpers */
    .muted{color:var(--muted)}
    .right{display:flex;gap:8px;align-items:center}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="avatar">YN</div>
        <div>
          <h1>Your Name <span style="font-weight:400; color:var(--muted); font-size:15px"> — Assistant Professor / PhD</span></h1>
          <p class="lead">Research: Machine Learning, Reinforcement Learning, Sequential Decision Making</p>
        </div>
      </div>
      <div class="right">
        <nav id="main-nav">
          <button class="nav-btn active" data-target="about">About</button>
          <button class="nav-btn" data-target="research">Research</button>
          <button class="nav-btn" data-target="publications">Publications</button>
          <button class="nav-btn" data-target="teaching">Teaching</button>
        </nav>
        <a class="btn-primary" id="download-cv" href="#">Download CV</a>
      </div>
    </header>

    <main class="grid">
      <section>
        <div id="about" class="card section" data-section>
          <div class="section-title"><h2>About</h2><span class="muted"> • short bio</span></div>
          <p>Hello — I'm <strong>Your Name</strong>. I work on reinforcement learning, function approximation, and safe decision making. My page lists publications, projects, and teaching. Replace this paragraph with a 2–4 sentence academic bio.</p>

          <div style="margin-top:14px;display:flex;gap:12px;flex-wrap:wrap">
            <a href="#research" class="chip">Research overview</a>
            <a href="#publications" class="chip">Publications</a>
            <a href="#teaching" class="chip">Teaching</a>
          </div>

          <div style="margin-top:18px">
            <div class="section-title"><h2>Selected Projects</h2></div>
            <div class="card" style="padding:12px;margin-bottom:8px">
              <strong>Project A</strong>
              <div class="muted">Short project description. Link to repo or demo.</div>
            </div>
            <div class="card" style="padding:12px">
              <strong>Project B</strong>
              <div class="muted">Short project description. Link to repo or demo.</div>
            </div>
          </div>
        </div>

        <div id="research" class="card section" data-section style="margin-top:18px;display:none">
          <div class="section-title"><h2>Research</h2><span class="muted"> • interests & summary</span></div>
          <p>High-level research summary (3–5 sentences). You can add bullets for themes.</p>
          <ul class="muted">
            <li>Reinforcement learning theory and algorithms</li>
            <li>Function approximation and generalization</li>
            <li>Applications: robotics, healthcare, operations research</li>
          </ul>

          <div style="margin-top:12px">
            <h3>Preprints & Ongoing</h3>
            <div class="pub">
              <h3>Title of Ongoing Work</h3>
              <div class="info">Authors • draft (2025) • abstract: Very short blurb about the paper.</div>
            </div>
          </div>
        </div>

        <div id="publications" class="card section" data-section style="margin-top:18px;display:none">
          <div class="section-title"><h2>Publications</h2><span class="muted"> • selected</span></div>

          <div class="search" style="margin-bottom:12px">
            <input id="pub-filter" placeholder="Filter by keyword, venue, or year" />
            <button id="clear-filter">Clear</butto
