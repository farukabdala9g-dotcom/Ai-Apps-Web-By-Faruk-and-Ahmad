<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>AI Apps Blog — Project</title>
<style>
  :root{
    --bg:#0b1020; --panel:#0f1833; --ink:#e5e7eb; --muted:#9aa3b2;
    --brand:#7c3aed; --brand2:#06b6d4; --accent:#22c55e; --card:#121a36; --ring: rgba(124,58,237,.35);
  }
  *{box-sizing:border-box}
  html,body{
    margin:0;
    background:
      radial-gradient(1200px 600px at 10% -10%, rgba(124,58,237,.25), transparent 60%),
      radial-gradient(1000px 500px at 90% 10%, rgba(6,182,212,.18), transparent 60%),
      var(--bg);
    color:var(--ink);
    font-family:system-ui,-apple-system,Segoe UI,Roboto,Inter,Arial,sans-serif
  }
  a{color:var(--brand2); text-decoration:none}
  a:hover{text-decoration:underline}
  header{
    position:sticky; top:0; z-index:40;
    backdrop-filter:saturate(1.2) blur(10px);
    background:linear-gradient(180deg, rgba(15,24,51,.9), rgba(15,24,51,.5));
    border-bottom:1px solid rgba(255,255,255,.06);
  }
  .container{max-width:1200px; margin:0 auto; padding:20px}
  .hero{display:grid; gap:10px; padding:16px 0 8px}
  .title{font-size:clamp(28px,4vw,48px); font-weight:800; letter-spacing:.3px; line-height:1.05}
  .subtitle{color:var(--muted); font-size:clamp(14px,2vw,18px)}
  .badges{display:flex; gap:10px; flex-wrap:wrap; margin-top:8px}
  .badge{
    background:linear-gradient(90deg, rgba(124,58,237,.25), rgba(6,182,212,.25));
    border:1px solid rgba(255,255,255,.12); color:#e6e6ff;
    padding:6px 10px; border-radius:999px; font-size:13px
  }
  nav.categories{display:flex; gap:10px; flex-wrap:wrap; margin:14px 0 18px}
  nav.categories a{
    padding:8px 12px; border:1px solid rgba(255,255,255,.08);
    border-radius:999px; color:#cfe8ff; background:rgba(18,26,54,.7);
  }
  nav.categories a:hover{outline:2px solid var(--ring)}
  section{scroll-margin-top:90px; margin:28px 0}
  .section-head{display:flex; align-items:end; justify-content:space-between; margin-bottom:12px}
  .section-head h2{margin:0; font-size:clamp(20px,3vw,28px)}
  .section-head .hint{color:var(--muted); font-size:14px}
  .grid{display:grid; gap:16px; grid-template-columns:repeat(1, minmax(0,1fr));}
  @media(min-width:720px){ .grid{grid-template-columns:repeat(2, minmax(0,1fr));} }
  @media(min-width:1024px){ .grid{grid-template-columns:repeat(3, minmax(0,1fr));} }

  .card{
    background:linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02));
    border:1px solid rgba(255,255,255,.08);
    border-radius:18px; overflow:hidden;
    box-shadow:0 10px 30px rgba(0,0,0,.35);
    display:flex; flex-direction:column;
  }
  .card-head{display:flex; gap:12px; padding:16px 16px 12px; align-items:center; border-bottom:1px solid rgba(255,255,255,.06)}
  .logo{
    width:56px; height:56px; border-radius:12px;
    background:#0b1020; border:1px solid rgba(255,255,255,.12); object-fit:cover
  }
  .app-name{font-weight:700; font-size:18px; letter-spacing:.2px}
  .pill{margin-left:auto; font-size:12px; color:#bfe3ff; border:1px solid rgba(255,255,255,.12); padding:3px 8px; border-radius:999px}
  .card-body{padding:12px 16px 8px; color:var(--muted); font-size:14px; min-height:68px}
  .actions{display:flex; gap:10px; padding:8px 16px 16px; align-items:center}
  .btn{
    display:inline-flex; gap:8px; align-items:center; justify-content:center;
    padding:10px 12px; font-weight:600; font-size:14px; border-radius:12px; border:1px solid rgba(255,255,255,.14);
    background:linear-gradient(90deg, rgba(124,58,237,.35), rgba(6,182,212,.35));
    color:white; text-decoration:none; flex:1;
  }
  .btn.secondary{background:transparent}
  iframe{width:100%; aspect-ratio:16/9; border:0; border-top:1px solid rgba(255,255,255,.06)}
  footer{margin:40px 0 24px; color:var(--muted); font-size:14px; text-align:center}
  .top{position:fixed; right:16px; bottom:16px; z-index:50}
  .top a{display:inline-block; padding:10px 12px; background:var(--brand); color:white; border-radius:12px; border:1px solid rgba(255,255,255,.2)}
</style>
</head>
<body>

<header>
  <div class="container hero">
    <div class="title">AI Apps Blog</div>
    <div class="subtitle">Explore AI tools by category. Each app includes logo, name, function, link, and a direct YouTube tutorial.</div>
    <div class="badges">
      <span class="badge">33 apps</span>
      <span class="badge">Logo · Name · Function · Link · Video</span>
      <span class="badge">Assessed — Sept 2025</span>
    </div>
    <nav class="categories">
      <a href="#text">Text</a>
      <a href="#logo">Logo</a>
      <a href="#presentations">Presentations</a>
      <a href="#music">Music</a>
      <a href="#mindmaps">Mind Maps</a>
      <a href="#images">Images</a>
      <a href="#avatars">Avatars</a>
      <a href="#videos">Videos</a>
      <a href="#voice">Voice</a>
      <a href="#sound">Sound-Audio</a>
      <a href="#clonevoice">Clone Voice</a>
    </nav>
  </div>
</header>

<main class="container">

  <!-- ========== TEXT ========== -->
  <section id="text">
    <div class="section-head">
      <h2>Text</h2>
      <div class="hint">Writing assistance and text generation</div>
    </div>
    <div class="grid">

      <!-- ChatGPT -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=openai.com&sz=128" alt="ChatGPT">
          <div class="app-name">ChatGPT</div>
          <span class="pill">Text</span>
        </div>
        <div class="card-body">AI assistant for writing, summarizing, translating, and Q&A.</div>
        <div class="actions">
          <a class="btn" href="https://openai.com/chatgpt" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=g5oEAoKdrdw" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/g5oEAoKdrdw" title="ChatGPT tutorial"></iframe>
      </article>

      <!-- Jasper -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=jasper.ai&sz=128" alt="Jasper">
          <div class="app-name">Jasper</div>
          <span class="pill">Text</span>
        </div>
        <div class="card-body">Marketing copy and blog writing with AI templates.</div>
        <div class="actions">
          <a class="btn" href="https://www.jasper.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=W9y2rodf7Zg" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/W9y2rodf7Zg" title="Jasper tutorial"></iframe>
      </article>

      <!-- Copy.ai -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=copy.ai&sz=128" alt="Copy.ai">
          <div class="app-name">Copy.ai</div>
          <span class="pill">Text</span>
        </div>
        <div class="card-body">Generates captions, ads, and product descriptions.</div>
        <div class="actions">
          <a class="btn" href="https://www.copy.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=9EfoYaa_iLY" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/9EfoYaa_iLY" title="Copy.ai tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== LOGO ========== -->
  <section id="logo">
    <div class="section-head">
      <h2>Logo</h2>
      <div class="hint">Logo creation with AI</div>
    </div>
    <div class="grid">

      <!-- Looka -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=looka.com&sz=128" alt="Looka">
          <div class="app-name">Looka</div>
          <span class="pill">Logo</span>
        </div>
        <div class="card-body">Automatic logo maker and branding kits for businesses.</div>
        <div class="actions">
          <a class="btn" href="https://looka.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=SkKw9yWkoLE" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/SkKw9yWkoLE" title="Looka tutorial"></iframe>
      </article>

      <!-- Designhill Logo Maker -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=designhill.com&sz=128" alt="Designhill">
          <div class="app-name">Designhill Logo Maker</div>
          <span class="pill">Logo</span>
        </div>
        <div class="card-body">Logo generator with customization options.</div>
        <div class="actions">
          <a class="btn" href="https://www.designhill.com/tools/logo-maker" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=fefPjzCYt40" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/fefPjzCYt40" title="Designhill tutorial"></iframe>
      </article>

      <!-- Tailor Brands -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=tailorbrands.com&sz=128" alt="Tailor Brands">
          <div class="app-name">Tailor Brands</div>
          <span class="pill">Logo</span>
        </div>
        <div class="card-body">AI logo creator with brand kits and assets.</div>
        <div class="actions">
          <a class="btn" href="https://www.tailorbrands.com/logo-maker" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=mwrSyR7d7sU" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/mwrSyR7d7sU" title="Tailor Brands tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== PRESENTATIONS ========== -->
  <section id="presentations">
    <div class="section-head">
      <h2>Presentations</h2>
      <div class="hint">Decks and storytelling with AI</div>
    </div>
    <div class="grid">

      <!-- Beautiful.ai -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=beautiful.ai&sz=128" alt="Beautiful.ai">
          <div class="app-name">Beautiful.ai</div>
          <span class="pill">Presentations</span>
        </div>
        <div class="card-body">Smart slide layouts and automated design.</div>
        <div class="actions">
          <a class="btn" href="https://www.beautiful.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=Q1DXOpBhepE" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/Q1DXOpBhepE" title="Beautiful.ai tutorial"></iframe>
      </article>

      <!-- Tome -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=tome.app&sz=128" alt="Tome">
          <div class="app-name">Tome</div>
          <span class="pill">Presentations</span>
        </div>
        <div class="card-body">Generative storytelling and presentation creation.</div>
        <div class="actions">
          <a class="btn" href="https://tome.app" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=gagDblJWwi8" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/watch?v=wnGlF0OhL6I" title=Tome tutorial"></iframe>
      </article>

      <!-- Gamma -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=gamma.app&sz=128" alt="Gamma">
          <div class="app-name">Gamma</div>
          <span class="pill">Presentations</span>
        </div>
        <div class="card-body">Create slide decks and visual docs in minutes.</div>
        <div class="actions">
          <a class="btn" href="https://gamma.app" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=KcbXKUR7-a0" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/KcbXKUR7-a0" title="Gamma tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== MUSIC ========== -->
  <section id="music">
    <div class="section-head">
      <h2>Music</h2>
      <div class="hint">Composition and music generation</div>
    </div>
    <div class="grid">

      <!-- Aiva -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=aiva.ai&sz=128" alt="Aiva">
          <div class="app-name">Aiva</div>
          <span class="pill">Music</span>
        </div>
        <div class="card-body">AI music composer for film, games, and ads.</div>
        <div class="actions">
          <a class="btn" href="https://www.aiva.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=2_TVZBbJQGE" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/2_TVZBbJQGE" title="Aiva tutorial"></iframe>
      </article>

      <!-- Soundraw -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=soundraw.io&sz=128" alt="Soundraw">
          <div class="app-name">Soundraw</div>
          <span class="pill">Music</span>
        </div>
        <div class="card-body">Generate tracks by genre, mood, and duration.</div>
        <div class="actions">
          <a class="btn" href="https://soundraw.io" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=fqLcgF8Hf1M" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/fqLcgF8Hf1M" title="Soundraw tutorial"></iframe>
      </article>

      <!-- Boomy -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=boomy.com&sz=128" alt="Boomy">
          <div class="app-name">Boomy</div>
          <span class="pill">Music</span>
        </div>
        <div class="card-body">Create original songs and publish them online.</div>
        <div class="actions">
          <a class="btn" href="https://boomy.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=R9fYX5-0RVo" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/R9fYX5-0RVo" title="Boomy tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== MIND MAPS ========== -->
  <section id="mindmaps">
    <div class="section-head">
      <h2>Mind Maps</h2>
      <div class="hint">Idea mapping and organization</div>
    </div>
    <div class="grid">

      <!-- MindMeister -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=mindmeister.com&sz=128" alt="MindMeister">
          <div class="app-name">MindMeister (AI)</div>
          <span class="pill">Mind Maps</span>
        </div>
        <div class="card-body">Collaborative mind maps with AI features.</div>
        <div class="actions">
          <a class="btn" href="https://www.mindmeister.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=PuhmVJWOL84" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/PuhmVJWOL84" title="MindMeister tutorial"></iframe>
      </article>

      <!-- XMind -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=xmind.app&sz=128" alt="XMind">
          <div class="app-name">XMind (AI)</div>
          <span class="pill">Mind Maps</span>
        </div>
        <div class="card-body">Mind maps with templates, outline, and export.</div>
        <div class="actions">
          <a class="btn" href="https://xmind.app" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=07-BTkpWJEI" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/07-BTkpWJEI" title="XMind AI Quick Start"></iframe>
      </article>

      <!-- Whimsical -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=whimsical.com&sz=128" alt="Whimsical">
          <div class="app-name">Whimsical (AI)</div>
          <span class="pill">Mind Maps</span>
        </div>
        <div class="card-body">Diagrams, wireframes, and maps with real-time collaboration.</div>
        <div class="actions">
          <a class="btn" href="https://whimsical.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=6bJb7ZJWvj0" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/6bJb7ZJWvj0" title="Whimsical Mind Maps"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== IMAGES ========== -->
  <section id="images">
    <div class="section-head">
      <h2>Images</h2>
      <div class="hint">Image generation and editing</div>
    </div>
    <div class="grid">

      <!-- DALL·E -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=openai.com&sz=128" alt="DALL·E">
          <div class="app-name">DALL·E</div>
          <span class="pill">Images</span>
        </div>
        <div class="card-body">Generate images from natural language prompts.</div>
        <div class="actions">
          <a class="btn" href="https://openai.com/dall-e-3" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=ri1FCeVHGPg" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/ri1FCeVHGPg" title="DALL·E tutorial 2025"></iframe>
      </article>

      <!-- Midjourney -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=midjourney.com&sz=128" alt="Midjourney">
          <div class="app-name">Midjourney</div>
          <span class="pill">Images</span>
        </div>
        <div class="card-body">High-quality generative art with advanced prompting.</div>
        <div class="actions">
          <a class="btn" href="https://www.midjourney.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=cLYhZe9ZegA" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/cLYhZe9ZegA" title="Midjourney Full Course 2025"></iframe>
      </article>

      <!-- Stable Diffusion -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=stability.ai&sz=128" alt="Stable Diffusion">
          <div class="app-name">Stable Diffusion</div>
          <span class="pill">Images</span>
        </div>
        <div class="card-body">Open model for image generation and editing.</div>
        <div class="actions">
          <a class="btn" href="https://stability.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=HkILVJHlsbU" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/HkILVJHlsbU" title="Stable Diffusion tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== AVATARS ========== -->
  <section id="avatars">
    <div class="section-head">
      <h2>Avatars</h2>
      <div class="hint">Virtual presenters and talking avatars</div>
    </div>
    <div class="grid">

      <!-- Synthesia -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=synthesia.io&sz=128" alt="Synthesia">
          <div class="app-name">Synthesia</div>
          <span class="pill">Avatars</span>
        </div>
        <div class="card-body">Create videos with AI avatars and voiceover.</div>
        <div class="actions">
          <a class="btn" href="https://www.synthesia.io" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=7k3N1bUURa4" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/7k3N1bUURa4" title="AI Video in 4 Minutes with Synthesia"></iframe>
      </article>

      <!-- Ready Player Me -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=readyplayer.me&sz=128" alt="Ready Player Me">
          <div class="app-name">Ready Player Me</div>
          <span class="pill">Avatars</span>
        </div>
        <div class="card-body">Create interoperable 3D avatars for apps and games.</div>
        <div class="actions">
          <a class="btn" href="https://readyplayer.me" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=BL_kASDHAO4" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/BL_kASDHAO4" title="Ready Player Me Studio tutorial"></iframe>
      </article>

      <!-- HeyGen -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=heygen.com&sz=128" alt="HeyGen">
          <div class="app-name">HeyGen</div>
          <span class="pill">Avatars</span>
        </div>
        <div class="card-body">Talking avatars with lip-sync and language dubbing.</div>
        <div class="actions">
          <a class="btn" href="https://www.heygen.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=eFwx6fyDOmU" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/eFwx6fyDOmU" title="HeyGen Full Tutorial 2025"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== VIDEOS ========== -->
  <section id="videos">
    <div class="section-head">
      <h2>Videos</h2>
      <div class="hint">AI video creation and editing</div>
    </div>
    <div class="grid">

      <!-- Pictory -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=pictory.ai&sz=128" alt="Pictory">
          <div class="app-name">Pictory</div>
          <span class="pill">Videos</span>
        </div>
        <div class="card-body">Turn scripts or blogs into automatic videos.</div>
        <div class="actions">
          <a class="btn" href="https://pictory.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=F_hBJkHSep0" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/F_hBJkHSep0" title="Pictory 2025 tutorial"></iframe>
      </article>

      <!-- Runway -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=runwayml.com&sz=128" alt="Runway">
          <div class="app-name">Runway (Gen-2/Gen-3)</div>
          <span class="pill">Videos</span>
        </div>
        <div class="card-body">Cutting-edge video generation and editing.</div>
        <div class="actions">
          <a class="btn" href="https://runwayml.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=c38vtLw1nSk" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/c38vtLw1nSk" title="Runway tutorial for beginners"></iframe>
      </article>

      <!-- Lumen5 -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=lumen5.com&sz=128" alt="Lumen5">
          <div class="app-name">Lumen5</div>
          <span class="pill">Videos</span>
        </div>
        <div class="card-body">Social-media videos with AI templates.</div>
        <div class="actions">
          <a class="btn" href="https://lumen5.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=vi51bcImELI" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/vi51bcImELI" title="Lumen5 tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== VOICE ========== -->
  <section id="voice">
    <div class="section-head">
      <h2>Voice</h2>
      <div class="hint">Text-to-speech and narration</div>
    </div>
    <div class="grid">

      <!-- Murf -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=murf.ai&sz=128" alt="Murf">
          <div class="app-name">Murf</div>
          <span class="pill">Voice</span>
        </div>
        <div class="card-body">Realistic voiceovers in many languages.</div>
        <div class="actions">
          <a class="btn" href="https://murf.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=XsXF5BuGuBc" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/XsXF5BuGuBc" title="Murf AI tutorial"></iframe>
      </article>

      <!-- Speechify -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=speechify.com&sz=128" alt="Speechify">
          <div class="app-name">Speechify</div>
          <span class="pill">Voice</span>
        </div>
        <div class="card-body">Reads PDFs, web pages, and documents aloud.</div>
        <div class="actions">
          <a class="btn" href="https://speechify.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=zdgZQqN4OdM" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/zdgZQqN4OdM" title="Speechify tutorial"></iframe>
      </article>

      <!-- Play.ht -->
      <article class="card">
        <div class="card-head">
        <img class="logo" src="https://www.google.com/s2/favicons?domain=play.ht&sz=128" alt="Play.ht">
          <div class="app-name">Play.ht</div>
          <span class="pill">Voice</span>
        </div>
        <div class="card-body">Text-to-speech with cloning and editor tools.</div>
        <div class="actions">
          <a class="btn" href="https://play.ht" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=1pQoSsXE5Ak" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/1pQoSsXE5Ak" title="Play.ht tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== SOUND / AUDIO ========== -->
  <section id="sound">
    <div class="section-head">
      <h2>Sound · Audio</h2>
      <div class="hint">Audio cleanup, editing, and podcast tools</div>
    </div>
    <div class="grid">

      <!-- Adobe Podcast -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=podcast.adobe.com&sz=128" alt="Adobe Podcast">
          <div class="app-name">Adobe Podcast — Enhance Speech</div>
          <span class="pill">Sound</span>
        </div>
        <div class="card-body">Enhance voice and streamline podcast workflows.</div>
        <div class="actions">
          <a class="btn" href="https://podcast.adobe.com/en/enhance" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=4XyOaj9GE5k" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/4XyOaj9GE5k" title="Adobe Enhance Speech v2"></iframe>
      </article>

      <!-- Krisp -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=krisp.ai&sz=128" alt="Krisp">
          <div class="app-name">Krisp</div>
          <span class="pill">Sound</span>
        </div>
        <div class="card-body">Real-time noise cancellation for calls and recordings.</div>
        <div class="actions">
          <a class="btn" href="https://krisp.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=5LwBgkci6T4" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/5LwBgkci6T4" title="Krisp tutorial"></iframe>
      </article>

      <!-- Descript -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=descript.com&sz=128" alt="Descript">
          <div class="app-name">Descript</div>
          <span class="pill">Sound</span>
        </div>
        <div class="card-body">Edit audio/video by transcript (Overdub, Studio Sound).</div>
        <div class="actions">
          <a class="btn" href="https://www.descript.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=RgwJNOXGARI" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/RgwJNOXGARI" title="Descript 2025 tutorial"></iframe>
      </article>

    </div>
  </section>

  <!-- ========== CLONE VOICE ========== -->
  <section id="clonevoice">
    <div class="section-head">
      <h2>Clone Voice</h2>
      <div class="hint">Voice cloning and advanced synthesis</div>
    </div>
    <div class="grid">

      <!-- ElevenLabs -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=elevenlabs.io&sz=128" alt="ElevenLabs">
          <div class="app-name">ElevenLabs</div>
          <span class="pill">Clone Voice</span>
        </div>
        <div class="card-body">Ultra-realistic voices and multilingual cloning.</div>
        <div class="actions">
          <a class="btn" href="https://elevenlabs.io" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=YqS-3QpOmns" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/YqS-3QpOmns" title="ElevenLabs tutorial 2025"></iframe>
      </article>

      <!-- Respeecher -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=respeecher.com&sz=128" alt="Respeecher">
          <div class="app-name">Respeecher</div>
          <span class="pill">Clone Voice</span>
        </div>
        <div class="card-body">Professional voice cloning for film, TV, and games.</div>
        <div class="actions">
          <a class="btn" href="https://www.respeecher.com" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=4hMYidECyg0" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/4hMYidECyg0" title="Respeecher tutorial"></iframe>
      </article>

      <!-- Voice.ai -->
      <article class="card">
        <div class="card-head">
          <img class="logo" src="https://www.google.com/s2/favicons?domain=voice.ai&sz=128" alt="Voice.ai">
          <div class="app-name">Voice.ai</div>
          <span class="pill">Clone Voice</span>
        </div>
        <div class="card-body">Real-time voice changer with celebrity-style models.</div>
        <div class="actions">
          <a class="btn" href="https://voice.ai" target="_blank" rel="noopener">Visit site</a>
          <a class="btn secondary" href="https://www.youtube.com/watch?v=S7rXwsyqXrk" target="_blank" rel="noopener">Watch on YouTube</a>
        </div>
        <iframe src="https://www.youtube.com/embed/S7rXwsyqXrk" title="Voice.ai setup"></iframe>
      </article>

    </div>
  </section>

  <footer>
    <p><strong>AI Apps Blog</strong> · Logo · Name · Function · Link · Direct Video</p>
    <p>Created by: Faruk Abdala & Ahmad Handauz · Date: 9/1/2025</p>
  </footer>

</main>

<div class="top"><a href="#top" onclick="window.scrollTo({top:0,behavior:'smooth'});return false;">↑ Top</a></div>

</body>
</html>
