---
layout: home
title: Pankaj Yadav
permalink: /
---

<style>
  .home-container {
    max-width: 880px;
    margin: 0 auto;
    padding: 10px 15px 60px 15px;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    color: #2c3e50;
    line-height: 1.65;
  }

  /* Quick Anchor Sub-bar for On-Page Sections */
  .section-jump-bar {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    padding-bottom: 14px;
    margin-bottom: 28px;
    border-bottom: 1px solid #eaeaea;
    font-size: 0.92em;
  }
  .section-jump-bar a {
    color: #555;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.2s;
  }
  .section-jump-bar a:hover {
    color: #0066cc;
  }

  /* About Section (Bio Left + Photo Right) */
  .about-grid {
    display: flex;
    gap: 36px;
    align-items: flex-start;
    margin-bottom: 42px;
  }
  .about-text {
    flex: 1;
  }
  .about-text h1 {
    margin: 0 0 6px 0;
    font-size: 2.15em;
    font-weight: 700;
    color: #111;
  }
  .about-role {
    font-size: 1.02em;
    color: #555;
    margin-bottom: 16px;
    font-weight: 500;
  }
  .about-profile {
    width: 205px;
    text-align: center;
    flex-shrink: 0;
  }
  .about-profile img {
    width: 190px;
    height: 190px;
    object-fit: cover;
    border-radius: 8px;
    box-shadow: 0 4px 14px rgba(0, 0, 0, 0.1);
  }
  .profile-caption {
    margin-top: 8px;
    font-size: 0.84em;
    color: #666;
    line-height: 1.4;
  }
  .social-links {
    margin-top: 14px;
    font-size: 0.94em;
  }
  .social-links a {
    color: #0066cc;
    text-decoration: none;
    font-weight: 500;
  }
  .social-links a:hover {
    text-decoration: underline;
  }

  /* Section Headings */
  .timeline-section {
    margin-top: 44px;
    scroll-margin-top: 24px;
  }
  .timeline-section h2 {
    font-size: 1.55em;
    font-weight: 600;
    color: #111;
    border-bottom: 1px solid #e5e5e5;
    padding-bottom: 7px;
    margin-bottom: 18px;
  }

  /* Scrollable News Timeline Table (Brahma Style) */
  .news-box {
    max-height: 290px;
    overflow-y: auto;
    padding-right: 10px;
  }
  .news-table {
    width: 100%;
    border-collapse: collapse;
  }
  .news-table td {
    padding: 8px 0;
    vertical-align: top;
    border-bottom: 1px solid #f2f2f2;
    font-size: 0.94em;
  }
  .news-date {
    width: 105px;
    font-weight: 600;
    color: #555;
    white-space: nowrap;
  }

  /* Research Interests & Doctoral Pillars */
  .clean-list {
    padding-left: 20px;
    margin: 0;
  }
  .clean-list li {
    margin-bottom: 8px;
  }

  /* Publications List */
  .pub-category {
    font-size: 1.12em;
    font-weight: 600;
    color: #222;
    margin: 22px 0 12px 0;
  }
  .pub-item {
    margin-bottom: 18px;
    padding-left: 14px;
    border-left: 3px solid #0066cc;
  }
  .pub-badge {
    display: inline-block;
    background: #f0f6ff;
    color: #0066cc;
    font-weight: 600;
    font-size: 0.78em;
    padding: 1px 6px;
    border-radius: 4px;
    margin-right: 6px;
  }
  .pub-title {
    font-weight: 600;
    color: #111;
    font-size: 1.01em;
  }
  .pub-authors {
    color: #444;
    font-size: 0.92em;
    margin: 2px 0;
  }
  .pub-venue {
    font-style: italic;
    color: #555;
    font-size: 0.91em;
  }
  .award-tag {
    font-style: normal;
    font-weight: 600;
    color: #c27803;
    margin-left: 5px;
  }
  .pub-links a {
    display: inline-block;
    margin-top: 5px;
    margin-right: 8px;
    padding: 2px 8px;
    font-size: 0.8em;
    border: 1px solid #0066cc;
    border-radius: 4px;
    color: #0066cc;
    text-decoration: none;
  }
  .pub-links a:hover {
    background: #0066cc;
    color: #fff;
  }

  /* Education & Achievements */
  .edu-item {
    margin-bottom: 14px;
  }
  .edu-row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    font-weight: 600;
    color: #111;
  }
  .edu-date {
    font-weight: 500;
    color: #666;
    font-size: 0.92em;
  }
  .edu-inst {
    color: #555;
    font-size: 0.94em;
  }
  .achievement-item {
    list-style: none;
    margin-left: -20px;
    margin-bottom: 8px;
  }

  @media (max-width: 700px) {
    .about-grid {
      flex-direction: column-reverse;
      align-items: center;
    }
    .about-text h1, .about-role, .social-links {
      text-align: center;
    }
  }
</style>

<!-- Parallax Hero Banner -->
<div style="
  background-image: url('/pankajyadav.github.io/images/healthcare.png');
  height: 620px;
  background-attachment: fixed;
  background-position: center 22%;
  background-repeat: no-repeat;
  background-size: cover;
  margin: -2em -2em 2.2em -2em;
  display: flex;
  align-items: center;
  justify-content: center;
">
  <div style="text-align: center; padding: 0 20px;">
    <h1 style="font-family: 'Great Vibes', 'Bickham Script', 'Playfair Display', 'Georgia', cursive; color: #ffffff; font-size: 5em; font-weight: normal; font-style: italic; margin: 0; padding: 0; line-height: 1.1; text-shadow: 3px 4px 15px rgba(0,0,0,0.85); letter-spacing: 1px;">Pankaj Yadav</h1>
    <p style="font-family: -apple-system, BlinkMacSystemFont, 'Roboto', 'Segoe UI', sans-serif; color: #e6e6e6; font-size: 1.15em; text-transform: uppercase; letter-spacing: 4px; margin: 14px 0 0 0; font-weight: 500; text-shadow: 2px 2px 8px rgba(0,0,0,0.9);">Probabilistic AI Research</p>
  </div>
</div>

<div class="home-container">

  <!-- Quick Section Jump Links -->
  <div class="section-jump-bar">
    <a href="#about">About</a>
    <a href="#news">News</a>
    <a href="#research">Research</a>
    <a href="#publications">Selected Publications</a>
    <a href="#education">Education</a>
    <a href="#experience">Experience</a>
    <a href="#achievements">Achievements</a>
    <a href="#contact">Contact</a>
  </div>

  <!-- ABOUT -->
  <section id="about" class="about-grid">
    <div class="about-text">
      <h1>Pankaj Yadav</h1>
      <div class="about-role">Ph.D. Research Scholar, Department of Mathematics, IIT Jodhpur</div>
      <p>
        I am a Ph.D. Research Scholar in the Department of Mathematics at the <strong>Indian Institute of Technology Jodhpur</strong>, where I work under the supervision of <strong>Dr. V. V. M. S. Chandramouli</strong>.
      </p>
      <p>
        My research focuses on learning from imbalanced and rare-event data, certified and theoretically grounded oversampling, deep generative models (GANs, VAEs, diffusion) for data augmentation, cost-aware decision thresholds and calibration under prevalence shift, interpretable machine learning for healthcare (geriatrics, sarcopenia, fall risk), and tail-risk modelling in climate finance.
      </p>
      <div class="social-links">
        <a href="https://google.com" target="_blank">Scholar</a> &nbsp;/&nbsp;
        <a href="https://github.com" target="_blank">GitHub</a> &nbsp;/&nbsp;
        <a href="https://linkedin.com" target="_blank">LinkedIn</a> &nbsp;/&nbsp;
        <a href="#contact">Email</a>
      </div>
    </div>
    <div class="about-profile">
      <img src="/pankajyadav.github.io/images/profile.jpg" alt="Pankaj Yadav">
      <div class="profile-caption">Department of Mathematics<br>IIT Jodhpur, India</div>
    </div>
  </section>

  <!-- NEWS TIMELINE -->
  <section id="news" class="timeline-section">
    <h2>News</h2>
    <div class="news-box">
      <table class="news-table">
        <tr>
          <td class="news-date">2026</td>
          <td>Our paper, <em>"Are Kolmogorov–Arnold Networks (KANs) suitable for imbalanced data classification?"</em> has been accepted by <strong>IEEE Transactions on Emerging Topics in Computational Intelligence</strong>.</td>
        </tr>
        <tr>
          <td class="news-date">2026</td>
          <td>Our article, <em>"Hedging rainfall volatility in Indian agriculture: A quantile-gamma approach to weather derivatives"</em> has been published in <strong>Journal of Climate Finance</strong> (Vol. 14).</td>
        </tr>
        <tr>
          <td class="news-date">2026</td>
          <td>Submitted preprints on population-calibrated sarcopenia risk learning, clinically constrained decision frameworks (<strong>SAvRAC</strong>), and interpretable trading decision support.</td>
        </tr>
        <tr>
          <td class="news-date">2025</td>
          <td>Our preprints <em>"Certified Interpolation Safe Oversampling (CISO)"</em> (<a href="https://arxiv.org" target="_blank">arXiv:2501.15790</a>) and <em>"GANs for handling imbalance in data mining"</em> (<a href="https://arxiv.org" target="_blank">arXiv:2502.16535</a>) are now available on arXiv.</td>
        </tr>
        <tr>
          <td class="news-date">2025</td>
          <td>Presented our paper <em>"Solar PV power generation forecasting using synergy of artificial intelligence and metaheuristics based approaches"</em> at <strong>IACC 2025</strong> (Springer).</td>
        </tr>
        <tr>
          <td class="news-date">Sep 2024</td>
          <td>Appointed <strong>General Secretary, Hostel B3</strong> and <strong>Head, Institute Dining Committee</strong> at IIT Jodhpur (2024–2025).</td>
        </tr>
        <tr>
          <td class="news-date">2023</td>
          <td>Published work on elderly muscle power prediction at <strong>IEEE MIPR 2023</strong> and fall-risk oversampling in <strong>Springer CCIS</strong>.</td>
        </tr>
        <tr>
          <td class="news-date">2022</td>
          <td>Our paper <em>"Evaluation of risk factors for fall in elderly people from imbalanced data using SMOTE"</em> received the <strong>Best Student Paper Award</strong> at <strong>ICT4AWE 2022</strong>.</td>
        </tr>
        <tr>
          <td class="news-date">Jan 2022</td>
          <td>Joined IIT Jodhpur as a Ph.D. Research Scholar in Mathematics under the supervision of Dr. V. V. M. S. Chandramouli.</td>
        </tr>
      </table>
    </div>
  </section>

