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
    --navy: #14213d;
    --navy-deep: #0b1426;
    --gold: #b08d57;
    --gold-soft: #d8c39a;
    --ink: #2b2b2b;
    --muted: #5f6673;
    --paper: #fbfaf7;
    --rule: #e6e0d4;
  }

  .py-hero {
    position: relative;
    height: 560px;
    margin: -2em -2em 0 -2em;
    background-image: url('/pankajyadav.github.io/images/healthcare.png');
    background-size: cover;
    background-position: center 30%;
    background-repeat: no-repeat;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }
  .py-hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(180deg, rgba(11,20,38,0.35) 0%, rgba(11,20,38,0.55) 60%, rgba(11,20,38,0.85) 100%);
  }
  .py-hero-inner {
    position: relative;
    text-align: center;
    padding: 0 24px;
  }
  .py-hero h1 {
    font-family: 'Cormorant Garamond', 'Georgia', serif;
    font-weight: 500;
    font-style: italic;
    color: #ffffff;
    font-size: clamp(3rem, 8vw, 5.2rem);
    letter-spacing: 1px;
    line-height: 1.05;
    margin: 0;
    text-shadow: 0 4px 20px rgba(0,0,0,0.45);
  }
  .py-hero .py-divider {
    width: 72px;
    height: 2px;
    background: var(--gold-soft);
    margin: 22px auto 18px auto;
  }
  .py-hero p {
    font-family: 'Inter', -apple-system, 'Segoe UI', sans-serif;
    color: #ece6da;
    font-size: 0.95rem;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 5px;
    margin: 0;
  }

  .py-body {
    max-width: 760px;
    margin: 0 auto;
    padding: 64px 8px 24px 8px;
    font-family: 'EB Garamond', 'Georgia', serif;
    color: var(--ink);
    font-size: 1.18rem;
    line-height: 1.75;
  }
  .py-intro {
    font-size: 1.32rem;
    line-height: 1.7;
    text-align: center;
    color: var(--navy);
    margin: 0 0 56px 0;
  }
  .py-intro strong { color: var(--navy-deep); font-weight: 500; }

  .py-section { margin: 0 0 48px 0; }
  .py-section h3 {
    font-family: 'Inter', sans-serif;
    font-size: 0.78rem;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--gold);
    margin: 0 0 14px 0;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--rule);
  }
  .py-section ul { list-style: none; padding: 0; margin: 0; }
  .py-section li {
    position: relative;
    padding: 6px 0 6px 22px;
  }
  .py-section li::before {
    content: "";
    position: absolute;
    left: 2px;
    top: 0.95em;
    width: 7px;
    height: 7px;
    border: 1px solid var(--gold);
    transform: rotate(45deg);
  }
  .py-section li strong { color: var(--navy); font-weight: 500; }

  .py-quote {
    margin: 0;
    padding: 18px 24px;
    background: var(--paper);
    border-left: 3px solid var(--gold);
    font-style: italic;
    color: #3d4250;
  }

  .py-contact {
    text-align: center;
    margin: 8px 0 0 0;
    font-size: 1.1rem;
    color: var(--muted);
  }
  .py-contact a { color: var(--navy); text-decoration: none; border-bottom: 1px solid var(--gold-soft); }
  .py-contact a:hover { color: var(--gold); }

  .py-connect {
    background: var(--navy);
    margin: 56px -2em 0 -2em;
    padding: 56px 24px;
    text-align: center;
  }
  .py-connect h2 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 500;
    font-size: 2.1rem;
    color: #ffffff;
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
    padding: 9px 20px;
    border: 1px solid rgba(216,195,154,0.45);
    border-radius: 999px;
    transition: all 0.2s ease;
  }
  .py-links a:hover { background: var(--gold-soft); color: var(--navy); }

  .py-visitors { text-align: center; padding: 56px 8px 40px 8px; }
  .py-visitors h3 {
    font-family: 'Inter', sans-serif;
    font-size: 0.78rem;
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
    box-shadow: 0 6px 18px rgba(20,33,61,0.10);
  }

  @media (max-width: 640px) {
    .py-hero { height: 420px; background-position: center 25%; }
    .py-hero p { letter-spacing: 3px; font-size: 0.8rem; }
    .py-body { font-size: 1.1rem; padding-top: 44px; }
    .py-intro { font-size: 1.18rem; }
  }
</style>

<div class="py-hero">
  <div class="py-hero-inner">
    <h1>Pankaj Yadav</h1>
    <div class="py-divider"></div>
    <p>Probabilistic AI Research</p>
  </div>
</div>

<div class="py-body">

  <p class="py-intro">Hi! I am <strong>Pankaj Yadav</strong>, a PhD researcher focusing on mitigating AI data bias, statistical inference, and deep generative models across healthcare, solar energy, and finance.</p>

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
