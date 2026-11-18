---
layout: default
title: Pankaj Yadav
permalink: /
author_profile: false
---

{% include base_path %}

<style>
  /* Home-page-only styles. Site-wide colors/fonts live in assets/css/custom.css */
  .py-home { padding: 48px 1.2em 0 1.2em; }           /* clears the fixed top menu */
  .py-wrap { max-width: 1040px; margin: 0 auto; }
  .py-home section { scroll-margin-top: 100px; }

  /* ---- Hero ---- */
  .py-hero {
    display: grid;
    grid-template-columns: 260px 1fr;
    gap: 52px;
    align-items: center;
    padding: 16px 8px 48px 8px;
    border-bottom: 1px solid var(--py-rule);
  }
  .py-portrait { position: relative; width: 100%; }
  .py-portrait::before {
    content: "";
    position: absolute;
    inset: 12px -12px -12px 12px;
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
    object-position: center 15%;   /* lower % = show more of the top of the photo */
    border-radius: 4px;
    box-shadow: 0 18px 40px rgba(0,0,0,0.45);
  }
  .py-hero-text h1 {
    font-family: 'Cormorant Garamond', Georgia, serif;
    font-weight: 500;
    font-style: italic;
    color: var(--py-heading);
    font-size: clamp(2.8rem, 6vw, 4.4rem);
    line-height: 1.05;
    margin: 0;
    border: none;
  }
  .py-divider { width: 64px; height: 2px; background: var(--py-gold); margin: 20px 0 16px 0; }
  .py-tagline {
    font-family: 'Inter', sans-serif;
    color: var(--py-gold-soft);
    font-size: 0.85rem;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 5px;
    margin: 0 0 22px 0;
  }
  .py-intro { font-size: 1.24rem; line-height: 1.7; margin: 0; }
  .py-intro strong { color: var(--py-heading); font-weight: 500; }

  /* ---- Section labels ---- */
  .py-label {
    font-family: 'Inter', sans-serif;
    font-size: 0.76rem;
    font-weight: 600;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--py-gold);
    margin: 0 0 18px 0;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--py-rule);
  }
  .py-block { padding: 52px 8px 0 8px; }

  /* ---- News + Timeline (side by side) ---- */
  .py-two { display: grid; grid-template-columns: 1.15fr 1fr; gap: 48px; }
  .py-news { list-style: none; margin: 0; padding: 0; }
  .py-news li {
    display: grid;
    grid-template-columns: 86px 1fr;
    gap: 16px;
    padding: 12px 0;
    border-bottom: 1px dashed var(--py-rule);
    font-size: 1.05rem;
    line-height: 1.55;
  }
  .py-news li:last-child { border-bottom: none; }
  .py-date {
    font-family: 'Inter', sans-serif;
    font-size: 0.72rem;
    font-weight: 600;
    letter-spacing: 1px;
    text-transform: uppercase;
    color: var(--py-gold-soft);
    background: rgba(201,169,110,0.10);
    border: 1px solid rgba(201,169,110,0.30);
    border-radius: 4px;
    padding: 4px 0;
    text-align: center;
    height: fit-content;
    margin-top: 3px;
  }
  .py-news em { color: var(--py-heading); }

  .py-timeline { list-style: none; margin: 0; padding: 0 0 0 4px; position: relative; }
  .py-timeline::before {
    content: "";
    position: absolute;
    left: 9px; top: 8px; bottom: 8px;
    width: 1px;
    background: linear-gradient(var(--py-gold), var(--py-rule));
  }
  .py-timeline li { position: relative; padding: 0 0 24px 34px; }
  .py-timeline li:last-child { padding-bottom: 0; }
  .py-timeline li::before {
    content: "";
    position: absolute;
    left: 0; top: 6px;
    width: 11px; height: 11px;
    border-radius: 50%;
    background: var(--py-bg);
    border: 2px solid var(--py-gold);
  }
  .py-timeline li.py-now::before { background: var(--py-gold); box-shadow: 0 0 0 4px rgba(201,169,110,0.18); }
  .py-tl-year {
    font-family: 'Inter', sans-serif;
    font-size: 0.72rem;
    font-weight: 600;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: var(--py-gold-soft);
  }
  .py-tl-title { display: block; color: var(--py-heading); font-size: 1.12rem; font-weight: 500; margin-top: 2px; }
  .py-tl-sub { display: block; color: var(--py-text-dim); font-size: 1rem; line-height: 1.5; }

  /* ---- Research interest boxes ---- */
  .py-grid4 { display: grid; grid-template-columns: repeat(4, 1fr); gap: 18px; }
  .py-box {
    background: var(--py-bg-raised);
    border: 1px solid var(--py-rule);
    border-top: 2px solid var(--py-gold);
    border-radius: 6px;
    padding: 22px 20px 20px 20px;
    transition: transform 0.2s ease, border-color 0.2s ease;
  }
  .py-box:hover { transform: translateY(-3px); border-color: #3a4a6a; border-top-color: var(--py-gold-soft); }
  .py-box-num {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 1.6rem;
    color: var(--py-gold);
    line-height: 1;
  }
  .py-box h4 {
    font-family: 'Cormorant Garamond', Georgia, serif;
    font-size: 1.3rem;
    font-weight: 600;
    line-height: 1.25;
    color: var(--py-heading);
    margin: 10px 0 8px 0;
  }
  .py-box p { margin: 0; font-size: 0.98rem; line-height: 1.55; color: var(--py-text-dim); }

  /* ---- Recent publication cards ---- */
  .py-grid2 { display: grid; grid-template-columns: 1fr 1fr; gap: 22px; }
  .py-paper {
    display: flex;
    flex-direction: column;
    background: var(--py-bg-raised);
    border: 1px solid var(--py-rule);
    border-left: 3px solid var(--py-gold);
    border-radius: 6px;
    padding: 24px 26px;
  }
  .py-venue {
    font-family: 'Inter', sans-serif;
    font-size: 0.72rem;
    font-weight: 600;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    color: var(--py-gold-soft);
    margin: 0 0 10px 0;
  }
  .py-paper h4 {
    font-family: 'Cormorant Garamond', Georgia, serif;
    font-size: 1.42rem;
    font-weight: 600;
    line-height: 1.28;
    color: var(--py-heading);
    margin: 0 0 8px 0;
  }
  .py-authors { font-size: 1rem; color: var(--py-text-dim); margin: 0 0 12px 0; }
  .py-authors strong { color: var(--py-text); font-weight: 500; }
  .py-paper p.py-sum { font-size: 1.02rem; line-height: 1.6; margin: 0 0 18px 0; }
  .py-actions { margin-top: auto; display: flex; gap: 10px; flex-wrap: wrap; }
  .py-actions a, .py-links a {
    font-family: 'Inter', sans-serif;
    font-size: 0.8rem;
    font-weight: 500;
    letter-spacing: 1px;
    padding: 7px 18px;
    border: 1px solid rgba(224,204,159,0.4);
    border-radius: 999px;
    transition: all 0.2s ease;
  }
  .py-actions a:hover, .py-links a:hover { background: var(--py-gold-soft); color: var(--py-bg); }
  .py-more { text-align: right; margin: 16px 0 0 0; font-family: 'Inter', sans-serif; font-size: 0.85rem; letter-spacing: 1px; }

  /* ---- Philosophy, contact, connect, visitors ---- */
  .py-narrow { max-width: 760px; margin: 0 auto; }
  .py-quote {
    margin: 0;
    padding: 20px 26px;
    background: var(--py-bg-raised);
    border-left: 3px solid var(--py-gold);
    border-radius: 0 4px 4px 0;
    font-style: italic;
    font-size: 1.15rem;
  }
  .py-contact { text-align: center; margin: 40px 0 0 0; font-size: 1.12rem; color: var(--py-text-dim); }
  .py-contact strong { color: var(--py-heading); font-weight: 500; }
  .py-contact a { border-bottom: 1px solid rgba(224,204,159,0.4); }
  .py-connect {
    margin: 48px 0 0 0;
    padding: 44px 24px;
    background: var(--py-bg-raised);
    border: 1px solid var(--py-rule);
    border-radius: 6px;
    text-align: center;
  }
  .py-connect h2 { font-size: 2rem; margin: 0 0 22px 0; border: none; }
  .py-links { display: flex; flex-wrap: wrap; justify-content: center; gap: 12px; }
  .py-visitors { text-align: center; padding: 52px 8px 40px 8px; }
  .py-visitors .py-label { border: none; text-align: center; }
  .py-visitors img { max-width: 100%; height: auto; border-radius: 6px; border: 1px solid var(--py-rule); box-shadow: 0 8px 24px rgba(0,0,0,0.35); }

  /* ---- Responsive ---- */
  @media (max-width: 960px) {
    .py-grid4 { grid-template-columns: repeat(2, 1fr); }
  }
  @media (max-width: 800px) {
    .py-home { padding-top: 32px; }
    .py-hero { grid-template-columns: 1fr; gap: 36px; text-align: center; }
    .py-portrait { max-width: 230px; margin: 0 auto; }
    .py-divider { margin: 18px auto 14px auto; }
    .py-tagline { letter-spacing: 3px; font-size: 0.78rem; }
    .py-intro { font-size: 1.12rem; }
    .py-two, .py-grid2 { grid-template-columns: 1fr; }
    .py-two { gap: 52px; }
  }
  @media (max-width: 520px) {
    .py-grid4 { grid-template-columns: 1fr; }
    .py-news li { grid-template-columns: 1fr; gap: 6px; }
    .py-date { width: fit-content; padding: 4px 10px; }
  }
</style>

<div class="py-home"><div class="py-wrap">
<!-- ================= HERO ================= -->
<section class="py-hero">
<div class="py-portrait"><img src="{{ base_path }}/images/healthcare.png" alt="Pankaj Yadav"></div>
<div class="py-hero-text">
<h1>Pankaj Yadav</h1>
<div class="py-divider"></div>
<p class="py-tagline">Probabilistic AI Research</p>
<p class="py-intro">Hi! I am <strong>Pankaj Yadav</strong>, a PhD researcher focusing on mitigating AI data bias, statistical inference, and deep generative models across healthcare, solar energy, and finance.</p>
</div>
</section>
<!-- ================= NEWS + ACADEMIC JOURNEY ================= -->
<section class="py-block py-two">
<div>
<h3 class="py-label">News</h3>
<ul class="py-news">
<li><span class="py-date">Nov 2026</span><span>Paper <em>“Are Kolmogorov–Arnold Networks Suitable for Imbalanced Data Classification?”</em> published in IEEE Transactions on Emerging Topics in Computational Intelligence.</span></li>
<li><span class="py-date">2026</span><span>Paper <em>“Hedging rainfall volatility in Indian agriculture: A quantile-gamma approach to weather derivatives”</em> published in the Journal of Climate Finance.</span></li>
<li><span class="py-date">Feb 2025</span><span>Systematic mapping study of GANs for data imbalance released on arXiv.</span></li>
<li><span class="py-date">Dec 2024</span><span>Solar PV power forecasting paper published at the International Advanced Computing Conference (IACC), Springer.</span></li>
<li><span class="py-date">May 2022</span><span>Received the <em>Best Student Paper Award</em> at ICT4AWE 2022.</span></li>
</ul>
</div>
<div>
<h3 class="py-label">Academic Journey</h3>
<ul class="py-timeline">
<li class="py-now"><span class="py-tl-year">Present</span><span class="py-tl-title">PhD in Mathematics</span><span class="py-tl-sub">Indian Institute of Technology (IIT) Jodhpur, Mathematics Department<br>Supervisor: Dr. Vivek Vijay</span></li>
<li><span class="py-tl-year">2021</span><span class="py-tl-title">M.Sc. in Mathematics</span><span class="py-tl-sub">IIT Jodhpur</span></li>
<li><span class="py-tl-year">2019</span><span class="py-tl-title">CSIR Junior Research Fellowship</span><span class="py-tl-sub">Council of Scientific &amp; Industrial Research, India</span></li>
<li><span class="py-tl-year">2018</span><span class="py-tl-title">B.Sc. (Hons) in Mathematics</span><span class="py-tl-sub">University of Delhi</span></li>
</ul>
</div>
</section>
<!-- ================= RESEARCH INTERESTS ================= -->
<section class="py-block">
<h3 class="py-label">Research Interests</h3>
<div class="py-grid4">
<div class="py-box"><div class="py-box-num">01</div><h4>Probabilistic Modeling &amp; Statistical Inference</h4><p>Quantifying uncertainty in real-world data, from tail risk to distributional forecasting.</p></div>
<div class="py-box"><div class="py-box-num">02</div><h4>Deep Generative Models &amp; AI-based Data Generation</h4><p>GANs and other generative models that create realistic synthetic data where real samples are scarce.</p></div>
<div class="py-box"><div class="py-box-num">03</div><h4>Imbalanced &amp; Rare-Event Learning</h4><p>Learning from minority classes and extreme events, with oversampling methods that come with guarantees.</p></div>
<div class="py-box"><div class="py-box-num">04</div><h4>Interpretable ML for Critical Domains</h4><p>Healthcare, solar energy and climate finance, where models must be reliable and explainable.</p></div>
</div>
</section>
<!-- ================= RECENT PUBLICATIONS ================= -->
<section class="py-block">
<h3 class="py-label">Recent Publications</h3>
<div class="py-grid2">
<article class="py-paper">
<p class="py-venue">IEEE Trans. Emerging Topics in Computational Intelligence · 2026</p>
<h4>Are Kolmogorov–Arnold Networks Suitable for Imbalanced Data Classification?</h4>
<p class="py-authors"><strong>P. Yadav</strong> and V. Vijay</p>
<p class="py-sum">Evaluates Kolmogorov–Arnold Networks (KANs) under structured class imbalance against parameter-matched MLPs and XGBoost baselines.</p>
<div class="py-actions"><a href="https://doi.org/10.1109/TETCI.2026.3747841" target="_blank" rel="noopener">DOI</a><a href="{{ base_path }}/publication/2026-kans-imbalance">Details</a></div>
</article>
<article class="py-paper">
<p class="py-venue">Journal of Climate Finance · 2026</p>
<h4>Hedging Rainfall Volatility in Indian Agriculture: A Quantile-Gamma Approach to Weather Derivatives</h4>
<p class="py-authors"><strong>P. Yadav</strong> and V. Vijay</p>
<p class="py-sum">A quantile–gamma XGBoost/SARIMA framework for weather-derivative triggers across drought and flood regimes.</p>
<div class="py-actions"><a href="https://doi.org/10.1016/j.jclimf.2026.100082" target="_blank" rel="noopener">DOI</a><a href="{{ base_path }}/publication/2026-rainfall-hedging">Details</a></div>
</article>
</div>
<p class="py-more"><a href="{{ base_path }}/publications/">All publications →</a></p>
</section>
<!-- ================= PHILOSOPHY + CONTACT ================= -->
<section class="py-block py-narrow">
<h3 class="py-label">Philosophy &amp; Approach</h3>
<p class="py-quote">As uncertainty in the world increases—the inevitable Law of Thermodynamics—life will continue to surprise you. Keep Body, Soul, and Spirit in check, and the mortgage will be paid.</p>
<p class="py-contact"><strong>Contact:</strong> <a href="mailto:yadav.58@iitj.ac.in">yadav.58@iitj.ac.in</a></p>
</section>
<!-- ================= CONNECT ================= -->
<div class="py-connect">
<h2>Connect with Me</h2>
<div class="py-links">
<a href="https://scholar.google.co.in/citations?hl=en" target="_blank" rel="noopener">Google Scholar</a>
<a href="https://www.linkedin.com/in/pankaj-yadav-867a40200?utm_source=share_via&utm_content=profile&utm_medium=member_ios" target="_blank" rel="noopener">LinkedIn</a>
<a href="https://github.com/rogue816" target="_blank" rel="noopener">GitHub</a>
<a href="https://orcid.org" target="_blank" rel="noopener">ORCID</a>
</div>
</div>
<!-- Live Flat Map Analytics Widget Section -->
<div class="py-visitors">
<h3 class="py-label">Global Visitor Reach</h3>
<a href="https://mapmyvisitors.com/web/1c9ds" title="Visit tracker" target="_blank" rel="noopener"><img src="https://mapmyvisitors.com/map.png?d=sKAaxWpSIhqPpJsq6envxHh9wm5d5RZV3FmR5YPehIo&cl=ffffff" alt="Visitor Map"></a>
</div>
</div></div>
