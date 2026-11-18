---
layout: default
title: Pankaj Yadav
permalink: /
author_profile: false
---

{% include base_path %}

<style>
  /* Home-page-only styles. Site-wide colors/fonts live in assets/css/custom.css */
  .py-home { padding: 0 1.2em; }
  .py-hero {
    max-width: 960px;
    margin: 40px auto 0 auto;
    padding: 40px 8px 56px 8px;
    display: grid;
    grid-template-columns: minmax(220px, 340px) 1fr;
    gap: 56px;
    align-items: center;
    border-bottom: 1px solid var(--py-rule);
  }
  .py-portrait { position: relative; width: 100%; }
  .py-portrait::before {
    content: "";
    position: absolute;
    inset: 14px -14px -14px 14px;
    border: 1px solid var(--py-gold);
    border-radius: 4px;
    opacity: 0.7;
  }
  .py-portrait img {
    position: relative;
    display: block;
    width: 100%;
    aspect-ratio: 3 / 4;
    object-fit: cover;
    object-position: center 15%;
    border-radius: 4px;
    box-shadow: 0 18px 40px rgba(0,0,0,0.45);
  }
  .py-hero-text h1 {
    font-family: 'Cormorant Garamond', Georgia, serif;
    font-weight: 500;
    font-style: italic;
    color: var(--py-heading);
    font-size: clamp(3rem, 7vw, 4.8rem);
    line-height: 1.05;
    margin: 0;
    border: none;
  }
  .py-divider { width: 64px; height: 2px; background: var(--py-gold); margin: 22px 0 18px 0; }
  .py-tagline {
    font-family: 'Inter', sans-serif;
    color: var(--py-gold-soft);
    font-size: 0.88rem;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 5px;
    margin: 0 0 26px 0;
  }
  .py-intro { font-size: 1.28rem; line-height: 1.7; margin: 0; }
  .py-intro strong { color: var(--py-heading); font-weight: 500; }
  .py-body { max-width: 760px; margin: 0 auto; padding: 56px 8px 16px 8px; font-size: 1.18rem; line-height: 1.75; }
  .py-section { margin: 0 0 46px 0; }
  .py-section h3 {
    font-family: 'Inter', sans-serif;
    font-size: 0.76rem;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--py-gold);
    margin: 0 0 14px 0;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--py-rule);
  }
  .py-section ul { list-style: none; padding: 0; margin: 0; }
  .py-section li { position: relative; padding: 6px 0 6px 24px; }
  .py-section li::before {
    content: "";
    position: absolute;
    left: 2px; top: 0.95em;
    width: 7px; height: 7px;
    border: 1px solid var(--py-gold);
    transform: rotate(45deg);
  }
  .py-section li strong { color: var(--py-heading); font-weight: 500; }
  .py-quote {
    margin: 0;
    padding: 20px 26px;
    background: var(--py-bg-raised);
    border-left: 3px solid var(--py-gold);
    border-radius: 0 4px 4px 0;
    font-style: italic;
  }
  .py-contact { text-align: center; margin: 6px 0 0 0; font-size: 1.12rem; color: var(--py-text-dim); }
  .py-contact strong { color: var(--py-heading); font-weight: 500; }
  .py-contact a { border-bottom: 1px solid rgba(224,204,159,0.4); }
  .py-connect {
    max-width: 960px;
    margin: 48px auto 0 auto;
    padding: 48px 24px;
    background: var(--py-bg-raised);
    border: 1px solid var(--py-rule);
    border-radius: 6px;
    text-align: center;
  }
  .py-connect h2 { font-size: 2.1rem; margin: 0 0 24px 0; border: none; }
  .py-links { display: flex; flex-wrap: wrap; justify-content: center; gap: 12px; }
  .py-links a {
    font-family: 'Inter', sans-serif;
    font-size: 0.85rem;
    font-weight: 500;
    letter-spacing: 1px;
    padding: 9px 22px;
    border: 1px solid rgba(224,204,159,0.4);
    border-radius: 999px;
    transition: all 0.2s ease;
  }
  .py-links a:hover { background: var(--py-gold-soft); color: var(--py-bg); }
  .py-visitors { text-align: center; padding: 56px 8px 40px 8px; }
  .py-visitors h3 {
    font-family: 'Inter', sans-serif;
    font-size: 0.76rem;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--py-gold);
    margin: 0 0 20px 0;
  }
  .py-visitors img { max-width: 100%; height: auto; border-radius: 6px; border: 1px solid var(--py-rule); box-shadow: 0 8px 24px rgba(0,0,0,0.35); }
  @media (max-width: 760px) {
    .py-hero { grid-template-columns: 1fr; gap: 40px; text-align: center; padding-top: 24px; }
    .py-portrait { max-width: 260px; margin: 0 auto; }
    .py-divider { margin: 20px auto 16px auto; }
    .py-tagline { letter-spacing: 3px; font-size: 0.8rem; }
    .py-intro { font-size: 1.15rem; }
    .py-body { font-size: 1.1rem; padding-top: 44px; }
  }
</style>

<div class="py-home">
<div class="py-hero">
<div class="py-portrait"><img src="{{ base_path }}/images/healthcare.png" alt="Pankaj Yadav"></div>
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
<a href="https://mapmyvisitors.com/web/1c9ds" title="Visit tracker" target="_blank" rel="noopener"><img src="https://mapmyvisitors.com/map.png?d=sKAaxWpSIhqPpJsq6envxHh9wm5d5RZV3FmR5YPehIo&cl=ffffff" alt="Visitor Map"></a>
</div>
</div>
