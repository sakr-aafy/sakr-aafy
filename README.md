<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Dev Profile</title>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --surface-0: #f1efe8;
    --surface-1: #f7f6f3;
    --surface-2: #ffffff;
    --text-primary: #1a1a18;
    --text-secondary: #5f5e5a;
    --text-muted: #888780;
    --border: rgba(0,0,0,0.1);
    --border-strong: rgba(0,0,0,0.18);
    --border-accent: #185fa5;
    --bg-accent: #e6f1fb;
    --text-accent: #0c447c;
    --bg-pro: #eeedfe;
    --text-pro: #3c3489;
    --border-pro: #534ab7;
    --bg-danger: #fcebeb;
    --text-danger: #a32d2d;
    --border-danger: #e24b4a;
    --bg-success: #eaf3de;
    --text-success: #3b6d11;
    --border-success: #639922;
    --radius: 8px;
    --font-sans: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --surface-0: #1a1a18;
      --surface-1: #252523;
      --surface-2: #2e2e2b;
      --text-primary: #f0ede8;
      --text-secondary: #b4b2a9;
      --text-muted: #888780;
      --border: rgba(255,255,255,0.1);
      --border-strong: rgba(255,255,255,0.18);
      --border-accent: #378add;
      --bg-accent: #042c53;
      --text-accent: #85b7eb;
      --bg-pro: #26215c;
      --text-pro: #afa9ec;
      --border-pro: #7f77dd;
      --bg-danger: #501313;
      --text-danger: #f09595;
      --border-danger: #e24b4a;
      --bg-success: #173404;
      --text-success: #97c459;
      --border-success: #639922;
    }
  }

  body {
    background: var(--surface-0);
    font-family: var(--font-sans);
    color: var(--text-primary);
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    padding: 2rem 1rem;
  }

  .profile-wrap {
    width: 100%;
    max-width: 680px;
  }

  .avatar-ring {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    background: var(--bg-accent);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 28px;
    font-weight: 500;
    color: var(--text-accent);
    border: 2px solid var(--border-accent);
    flex-shrink: 0;
  }

  .header-card {
    background: var(--surface-2);
    border: 0.5px solid var(--border);
    border-radius: 12px;
    padding: 1.5rem;
    display: flex;
    align-items: center;
    gap: 1.25rem;
    margin-bottom: 1rem;
  }

  .section-card {
    background: var(--surface-1);
    border: 0.5px solid var(--border);
    border-radius: 12px;
    padding: 1.25rem;
    margin-bottom: 1rem;
  }

  .section-label {
    font-size: 11px;
    font-weight: 500;
    letter-spacing: .07em;
    text-transform: uppercase;
    color: var(--text-muted);
    margin-bottom: .75rem;
  }

  .tech-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .tech-pill {
    display: flex;
    align-items: center;
    gap: 6px;
    background: var(--surface-2);
    border: 0.5px solid var(--border);
    border-radius: var(--radius);
    padding: 5px 10px;
    font-size: 13px;
    color: var(--text-secondary);
  }

  .tech-pill img {
    width: 16px;
    height: 16px;
  }

  .social-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .social-btn {
    display: flex;
    align-items: center;
    gap: 6px;
    padding: 7px 14px;
    border-radius: var(--radius);
    border: 0.5px solid var(--border-strong);
    font-size: 13px;
    font-weight: 500;
    cursor: pointer;
    text-decoration: none;
    background: transparent;
    transition: background .15s;
  }

  .social-btn:hover {
    background: var(--surface-1);
  }

  .tag {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 12px;
    font-weight: 500;
  }

  .expertise-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
    gap: 10px;
  }

  .expertise-card {
    border-radius: var(--radius);
    padding: 10px 12px;
  }

  .expertise-card p { margin: 0; }

  .dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #3a3;
    display: inline-block;
  }
</style>
</head>
<body>

<div class="profile-wrap">

  <!-- Header -->
  <div class="header-card">
    <div class="avatar-ring">FS</div>
    <div style="flex:1; min-width:0;">
      <p style="font-size:20px; font-weight:500; margin:0 0 4px; color:var(--text-primary);">Full Stack Developer</p>
      <p style="font-size:14px; color:var(--text-secondary); margin:0 0 8px;">Angular · Flask · Node.js</p>
      <div style="display:flex; flex-wrap:wrap; gap:6px;">
        <span class="tag" style="background:var(--bg-accent); color:var(--text-accent);">AI enthusiast</span>
        <span class="tag" style="background:var(--bg-pro); color:var(--text-pro);">Cybersecurity</span>
        <span class="tag" style="background:var(--bg-success); color:var(--text-success);">Open to work</span>
      </div>
    </div>
    <div style="display:flex; flex-direction:column; align-items:flex-end; gap:4px;">
      <span class="dot"></span>
      <span style="font-size:12px; color:var(--text-muted);">Available</span>
    </div>
  </div>

  <!-- Tech Stack -->
  <div class="section-card">
    <div class="section-label">Tech stack</div>
    <div class="tech-grid">
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="">JavaScript</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" alt="">TypeScript</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" alt="">Angular</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="">React</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="">Python</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="">Node.js</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="">Java</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" alt="">C#</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" alt="">Flutter</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" alt="">Firebase</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" alt="">Bootstrap</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="">Git</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" alt="">Linux</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="">HTML5</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="">CSS3</div>
      <div class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apache/apache-original.svg" alt="">Apache</div>
    </div>
  </div>

  <!-- Expertise -->
  <div class="section-card">
    <div class="section-label">Expertise areas</div>
    <div class="expertise-grid">
      <div class="expertise-card" style="border:0.5px solid var(--border-accent); background:var(--bg-accent);">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--text-accent)" stroke-width="2"><rect x="2" y="3" width="20" height="14" rx="2"/><path d="M8 21h8M12 17v4"/></svg>
        <p style="font-size:13px; font-weight:500; margin:6px 0 2px; color:var(--text-accent);">Full stack</p>
        <p style="font-size:12px; color:var(--text-secondary);">Frontend & backend</p>
      </div>
      <div class="expertise-card" style="border:0.5px solid var(--border-pro); background:var(--bg-pro);">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--text-pro)" stroke-width="2"><path d="M12 2a8 8 0 0 1 8 8c0 5-8 12-8 12S4 15 4 10a8 8 0 0 1 8-8z"/><circle cx="12" cy="10" r="3"/></svg>
        <p style="font-size:13px; font-weight:500; margin:6px 0 2px; color:var(--text-pro);">AI / ML</p>
        <p style="font-size:12px; color:var(--text-secondary);">Models & integrations</p>
      </div>
      <div class="expertise-card" style="border:0.5px solid var(--border-danger); background:var(--bg-danger);">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--text-danger)" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
        <p style="font-size:13px; font-weight:500; margin:6px 0 2px; color:var(--text-danger);">Cybersecurity</p>
        <p style="font-size:12px; color:var(--text-secondary);">Secure dev practices</p>
      </div>
      <div class="expertise-card" style="border:0.5px solid var(--border-success); background:var(--bg-success);">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--text-success)" stroke-width="2"><rect x="5" y="2" width="14" height="20" rx="2"/><path d="M12 18h.01"/></svg>
        <p style="font-size:13px; font-weight:500; margin:6px 0 2px; color:var(--text-success);">Mobile</p>
        <p style="font-size:12px; color:var(--text-secondary);">Flutter & cross-platform</p>
      </div>
    </div>
  </div>

  <!-- Social -->
  <div class="section-card">
    <div class="section-label">Connect</div>
    <div class="social-grid">
      <a class="social-btn" style="color:#0077B5; border-color:#0077B5;" href="#">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="#0077B5"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
        LinkedIn
      </a>
      <a class="social-btn" style="color:#D14836; border-color:#D14836;" href="#">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#D14836" stroke-width="2"><rect width="20" height="16" x="2" y="4" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        Gmail
      </a>
      <a class="social-btn" style="color:#1877F2; border-color:#1877F2;" href="#">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="#1877F2"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/></svg>
        Facebook
      </a>
      <a class="social-btn" style="color:#FF0000; border-color:#FF0000;" href="#">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#FF0000" stroke-width="2"><path d="M2.5 17a24.12 24.12 0 0 1 0-10 2 2 0 0 1 1.4-1.4 49.56 49.56 0 0 1 16.2 0A2 2 0 0 1 21.5 7a24.12 24.12 0 0 1 0 10 2 2 0 0 1-1.4 1.4 49.55 49.55 0 0 1-16.2 0A2 2 0 0 1 2.5 17"/><path d="m10 15 5-3-5-3z" fill="#FF0000"/></svg>
        YouTube
      </a>
      <a class="social-btn" style="color:#E4405F; border-color:#E4405F;" href="#">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#E4405F" stroke-width="2"><rect width="20" height="20" x="2" y="2" rx="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/></svg>
        Instagram
      </a>
    </div>
  </div>

</div>
</body>
</html>
