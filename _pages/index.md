---
layout: home
title: Pankaj Yadav
permalink: /
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,600;1,500&family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">

<style>
  :root {
    --bg: #0f1724;          /* page background: deep blue-slate, easy on the eyes */
    --bg-raised: #162133;   /* cards / quote / bands */
    --text: #d6dbe3;        /* body text: soft off-white, not pure white */
    --text-dim: #9aa4b2;
    --heading: #f1ece2;
    --gold: #c9a96e;
    --gold-soft: #e0cc9f;
    --rule: #26324a;
  }

  /* ---- Make the whole site dark, including the theme's header & footer ---- */
  html, body { background: var(--bg) !important; color: var(--text); }
  .site-header, .site-footer {
    background: var(--bg) !important;
    border-color: var(--rule) !important;
  }
  .site-header { border-top: 3px solid var(--gold) !important; border-bottom: 1px solid var(--rule) !important; }
  .site-title, .site-title:visited { color: var(--heading) !important; font-family: 'Cormorant Garamond', Georgia, serif; font-size: 1.5rem; }
  .site-nav .page-link, .site-nav .page-link:visited { color: var(--text-dim) !important; }
  .site-nav .page-link:hover { color: var(--gold) !important; }
  .site-nav { background: var(--bg) !important; border-color: var(--rule) !important; }
  .site-nav .menu-icon svg path { fill: var(--text-dim) !important; }
  .site-footer, .site-footer * { color: var(--text-dim) !important; }
  .site-footer a { color: var(--gold-soft) !important; }
  .page-content { background: var(--bg); }
  a { color: var(--gold-soft); }

  /* ---- Hero: portrait beside name (no cropping of a vertical photo) ---- */
  .py-hero {
    max-width: 960px;
    margin: 24px auto 0 auto;
    padding: 40px 8px 56px 8px;
    display: grid;
    grid-template-columns: minmax(220px, 340px) 1fr;
    gap: 56px;
    align-items: center;
    border-bottom: 1px solid var(--rule);
  }
  .py-portrait {
    position: relative;
    width: 100%;
  }
  .py-portrait::before {           /* offset gold frame */
    content: "";
    position: absolute;
    inset: 14px -14px -14px 14px;
    border: 1px solid var(--gold);
    border-radius: 4px;
    opacity: 0.7;
  }
  .py-portrait img {
    position: relative;
    display: block;
    width: 100%;
    aspect-ratio: 3 / 4;
    object-fit: cover;
    object-position: center 15%;   /* raise or lower to adjust framing */
    border-radius: 4px;
    box-shadow: 0 18px 40px rgba(0,0,0,0.45);
  }
  .py-hero-text h1 {
    font-family: 'Cormorant Garamond', Georgia, serif;
    font-weight: 500;
    font-style: italic;
    color: var(--heading);
    font-size: clamp(3rem, 7vw, 4.8rem);
    line-height: 1.05;
    letter-spacing: 0.5px;
    margin: 0;
    border: none;
  }
  .py-divider { width: 64px; height: 2px; background: var(--gold); margin: 22px 0 18px 0; }
  .py-tagline {
    font-family: 'Inter', -apple-system, 'Segoe UI', sans-serif;
    color: var(--gold-soft);
    font-size: 0.88rem;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 5px;
    margin: 0 0 26px 0;
  }
  .py-intro {
    font-family: 'EB Garamond', Georgia, serif;
    font-size: 1.28rem;
    line-height: 1.7;
    color: var(--text);
    margin: 0;
  }
  .py-intro strong { color: var(--heading); font-weight: 500; }

  /* ---- Body ---- */
  .py-body {
    max-width: 760px;
    margin: 0 auto;
    padding: 56px 8px 16px 8px;
    font-family: 'EB Garamond', Georgia, serif;
    color: var(--text);
    font-size: 1.18rem;
    line-height: 1.75;
  }
  .py-section { margin: 0 0 46px 0; }
  .py-section h3 {
    font-family: 'Inter', sans-serif;
    font-size: 0.76rem;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--gold);
    margin: 0 0 14px 0;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--rule);
  }
  .py-section ul { list-style: none; padding: 0; margin: 0; }
  .py-section li { position: relative; padding: 6px 0 6px 24px; }
  .py-section li::before {
    content: "";
    position: absolute;
    left: 2px; top: 0.95em;
    width: 7px; height: 7px;
    border: 1px solid var(--gold);
    transform: rotate(45deg);
  }
  .py-section li strong { color: var(--heading); font-weight: 500; }
  .py-quote {
    margin: 0;
    padding: 20px 26px;
    background: var(--bg-raised);
    border-left: 3px solid var(--gold);
    border-radius: 0 4px 4px 0;
    font-style: italic;
    color: var(--text);
  }
  .py-contact { text-align: center; margin: 6px 0 0 0; font-size: 1.12rem; color: var(--text-dim); }
  .py-contact strong { color: var(--heading); font-weight: 500; }
  .py-contact a { color: var(--gold-soft); text-decoration: none; border-bottom: 1px solid rgba(224,204,159,0.4); }
  .py-contact a:hover { color: var(--gold); }

  /* ---- Connect ---- */
  .py-connect {
    max-width: 960px;
    margin: 48px auto 0 auto;
    padding: 48px 24px;
    background: var(--bg-raised);
    border: 1px solid var(--rule);
    border-radius: 6px;
    text-align: center;
  }
  .py-connect h2 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 500;
    font-size: 2.1rem;
    color: var(--heading);
    margin: 0 0 24px 0;
    border: none;
  }
  .py-links { display: flex; flex-wrap: wrap; justify-content: center; gap: 12px; }
  .py-links a {
    font-family: 'Inter', sans-serif;
    font-size: 0.85rem;
    font-weight: 500;
    letter-spacing: 1px;
    color: var(--gold-soft);
    text-decoration: none;
    padding: 9px 22px;
    border: 1px solid rgba(224,204,159,0.4);
    border-radius: 999px;
    transition: all 0.2s ease;
  }
  .py-links a:hover { background: var(--gold-soft); color: var(--bg); }

  /* ---- Visitors ---- */
  .py-visitors { text-align: center; padding: 56px 8px 40px 8px; }
  .py-visitors h3 {
    font-family: 'Inter', sans-serif;
    font-size: 0.76rem;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--gold);
    margin: 0 0 20px 0;
  }
  .py-visitors img {
    max-width: 100%;
    height: auto;
    border-radius: 6px;
    border: 1px solid var(--rule);
    box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  }

  /* ---- Mobile ---- */
  @media (max-width: 760px) {
    .py-hero { grid-template-columns: 1fr; gap: 40px; text-align: center; padding-top: 24px; }
    .py-portrait { max-width: 260px; margin: 0 auto; }
    .py-divider { margin: 20px auto 16px auto; }
    .py-tagline { letter-spacing: 3px; font-size: 0.8rem; }
    .py-intro { font-size: 1.15rem; }
    .py-body { font-size: 1.1rem; padding-top: 44px; }
  }
</style>

<div class="py-hero">
  <div class="py-portrait">
    <img src="/pankajyadav.github.io/images/healthcare.png" alt="Pankaj Yadav">
  </div>
  <div class="py-hero-text">
    <h1>Pankaj Yadav</h1>
    <div class="py-divider"></div>
    <p class="py-tagline">Probabilistic AI Research</p>
    <p class="py-intro">Hi! I am <strong>Pankaj Yadav</strong>, a PhD researcher focusing on mitigating AI data bias, statistical inference, and deep generative models across healthcare, solar energy, and finance.</p>
  </div>
</div>

<div class="py-body">

  <div class="py-section">
    <h3>Academic Background</h3>
    <ul>
      <li><strong>PhD in Mathematics</strong>, Indian Institute of Technology (IIT) Jodhpur, Mathematics Department</li>
      <li><strong>M.Sc. in Mathematics</strong>, IIT Jodhpur</li>
      <li><strong>B.Sc. (Hons) in Mathematics</strong>, University of Delhi</li>
    </ul>
  </div>

  <div class="py-section">
    <h3>Research Interests</h3>
    <ul>
      <li><strong>Probabilistic Modeling &amp; Statistical Inference</strong></li>
      <li><strong>Deep Generative Models &amp; AI-based Data Generation</strong></li>
    </ul>
  </div>

  <div class="py-section">
    <h3>Philosophy &amp; Approach</h3>
    <p class="py-quote">As uncertainty in the world increases—the inevitable Law of Thermodynamics—life will continue to surprise you. Keep Body, Soul, and Spirit in check, and the mortgage will be paid.</p>
  </div>

  <p class="py-contact"><strong>Contact:</strong> <a href="mailto:yadav.58@iitj.ac.in">yadav.58@iitj.ac.in</a></p>

</div>

<div class="py-connect">
  <h2>Connect with Me</h2>
  <div class="py-links">
    <a href="https://google.co.in" target="_blank" rel="noopener">Google Scholar</a>
    <a href="https://linkedin.com" target="_blank" rel="noopener">LinkedIn</a>
    <a href="https://github.com" target="_blank" rel="noopener">GitHub</a>
    <a href="https://orcid.org" target="_blank" rel="noopener">ORCID</a>
  </div>
</div>

<!-- Live Flat Map Analytics Widget Section -->
<div class="py-visitors">
  <h3>Global Visitor Reach</h3>
  <a href="https://mapmyvisitors.com/web/1c9ds" title="Visit tracker" target="_blank" rel="noopener">
    <img src="https://mapmyvisitors.com/map.png?d=sKAaxWpSIhqPpJsq6envxHh9wm5d5RZV3FmR5YPehIo&cl=ffffff" alt="Visitor Map">
  </a>
</div>
