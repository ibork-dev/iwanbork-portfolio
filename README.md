<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Welcome — Projects</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--muted:#9aa4b2;--accent1:#7c3aed;--accent2:#06b6d4}
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background:linear-gradient(180deg,#061025 0%, #07122a 60%);color:#e6eef6;
      -webkit-font-smoothing:antialiased;line-height:1.45;padding:32px;
    }

    header{max-width:1100px;margin:0 auto 28px}
    .brand{display:flex;align-items:center;gap:16px}
    .logo{
      width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent1),var(--accent2));
      display:grid;place-items:center;font-weight:700;color:white;font-size:20px;
      box-shadow:0 6px 20px rgba(12,18,30,.6);
    }
    h1{margin:0;font-size:28px}
    p.lead{margin:8px 0 0;color:var(--muted);max-width:880px}

    .toc{max-width:1100px;margin:22px auto;padding:18px 20px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border:1px solid rgba(255,255,255,.03);border-radius:12px;display:flex;flex-wrap:wrap;gap:12px;align-items:center}
    .toc a{color:var(--accent2);text-decoration:none;padding:8px 12px;border-radius:8px;background:transparent;font-weight:600}
    .toc a:hover{background:rgba(255,255,255,0.02)}

    main{max-width:1100px;margin:28px auto;display:grid;grid-template-columns:1fr;gap:18px}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:16px}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));border-radius:12px;padding:12px;border:1px solid rgba(255,255,255,0.03);box-shadow:0 6px 18px rgba(3,6,14,.6);transition:transform .22s ease,box-shadow .22s ease}
    .card:hover{transform:translateY(-6px);box-shadow:0 18px 36px rgba(2,6,23,.6)}
    .media{position:relative;border-radius:10px;overflow:hidden}
    .media img{display:block;width:100%;height:180px;object-fit:cover;transition:transform .35s ease}
    .card:hover .media img{transform:scale(1.03)}

    .title-row{display:flex;justify-content:space-between;align-items:center;margin-top:12px}
    .title-row a.title{color:#e6eef6;text-decoration:none;font-weight:700}
    .title-row a.title:hover{color:var(--accent1)}
    .desc{color:var(--muted);margin-top:8px;font-size:14px}

    .meta{display:flex;gap:8px;align-items:center;margin-top:10px}
    .tag{padding:6px 8px;border-radius:8px;background:rgba(255,255,255,0.02);font-size:12px;color:var(--muted);border:1px solid rgba(255,255,255,0.02)}

    footer{max-width:1100px;margin:28px auto;color:var(--muted);font-size:13px}

    @media (max-width:520px){.media img{height:140px}}

    /* smooth anchor scroll */
    html{scroll-behavior:smooth}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <div class="logo">W</div>
      <div>
        <h1>Welcome</h1>
        <p class="lead">This page is a visual index of my projects. Click a gif or title to open that project's GitHub repository.</p>
      </div>
    </div>
  </header>

  <nav class="toc" aria-label="Table of contents">
    <!-- Replace these anchors with project IDs below or add new ones -->
    <a href="#project-1">Project One</a>
    <a href="#project-2">Project Two</a>
    <a href="#project-3">Project Three</a>
  </nav>

  <main>
    <section class="grid" id="projects">

      <!-- Project card template. Duplicate for each project. -->
      <article class="card" id="project-1">
        <a class="media" href="https://github.com/your-username/project-one" target="_blank" rel="noopener noreferrer">
          <img alt="Project One demo" src="https://media.giphy.com/media/your-gif-link1/giphy.gif" onerror="this.src='data:image/svg+xml;utf8,<svg xmlns=\'http://www.w3.org/2000/svg\' width=\'800\' height=\'450\'><rect width=\'100%\' height=\'100%\' fill=\'%230b1220\' /><text x=\'50%\' y=\'50%\' fill=\'%239aa4b2\' font-size=\'24\' text-anchor=\'middle\' dominant-baseline=\'middle\'>Replace GIF URL</text></svg>'"/>
        </a>

        <div class="title-row">
          <a class="title" href="https://github.com/your-username/project-one" target="_blank" rel="noopener noreferrer">Project One</a>
          <div class="meta">
            <div class="tag">Demo</div>
            <div class="tag">JavaScript</div>
          </div>
        </div>

        <p class="desc">Short description. What it does and why it is interesting. Add bullets in the repo page.</p>
      </article>

      <article class="card" id="project-2">
        <a class="media" href="https://github.com/your-username/project-two" target="_blank" rel="noopener noreferrer">
          <img alt="Project Two demo" src="https://media.giphy.com/media/your-gif-link2/giphy.gif" onerror="this.src='data:image/svg+xml;utf8,<svg xmlns=\'http://www.w3.org/2000/svg\' width=\'800\' height=\'450\'><rect width=\'100%\' height=\'100%\' fill=\'%230b1220\' /><text x=\'50%\' y=\'50%\' fill=\'%239aa4b2\' font-size=\'24\' text-anchor=\'middle\' dominant-baseline=\'middle\'>Replace GIF URL</text></svg>'"/>
        </a>

        <div class="title-row">
          <a class="title" href="https://github.com/your-username/project-two" target="_blank" rel="noopener noreferrer">Project Two</a>
          <div class="meta">
            <div class="tag">Web app</div>
            <div class="tag">React</div>
          </div>
        </div>

        <p class="desc">Short description. Key features and technologies used. Keep it one line here.</p>
      </article>

      <article class="card" id="project-3">
        <a class="media" href="https://github.com/your-username/project-three" target="_blank" rel="noopener noreferrer">
          <img alt="Project Three demo" src="https://media.giphy.com/media/your-gif-link3/giphy.gif" onerror="this.src='data:image/svg+xml;utf8,<svg xmlns=\'http://www.w3.org/2000/svg\' width=\'800\' height=\'450\'><rect width=\'100%\' height=\'100%\' fill=\'%230b1220\' /><text x=\'50%\' y=\'50%\' fill=\'%239aa4b2\' font-size=\'24\' text-anchor=\'middle\' dominant-baseline=\'middle\'>Replace GIF URL</text></svg>'"/>
        </a>

        <div class="title-row">
          <a class="title" href="https://github.com/your-username/project-three" target="_blank" rel="noopener noreferrer">Project Three</a>
          <div class="meta">
            <div class="tag">Utility</div>
            <div class="tag">Python</div>
          </div>
        </div>

        <p class="desc">Short description. What problem it solves and a quick note on usage or demo link.</p>
      </article>

    </section>

    <footer>
      <p>To add or reorder projects duplicate a <code>&lt;article class="card"&gt;</code> block. Replace the <code>href</code> and <code>src</code> values with your GitHub repo and gif URLs. This file is a standalone HTML index. For GitHub README.md use the animated-gif links and regular markdown linking instead.</p>
    </footer>
  </main>
</body>
</html>
