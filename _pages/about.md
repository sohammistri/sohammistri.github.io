---
permalink: /
title: ""
excerpt: "Home page"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
.home-intro {
  font-size: 1.05em;
  line-height: 1.75;
  color: #494e52;
  margin-bottom: 2em;
  padding: 1.25em 1.5em;
  background: #f7fbfd;
  border-left: 4px solid #52adc8;
  border-radius: 0 4px 4px 0;
}
.home-intro a { color: #52adc8; text-decoration: none; }
.home-intro a:hover { text-decoration: underline; }

.home-section { margin-bottom: 2em; }

.home-section-title {
  font-size: 1.25em;
  font-weight: 700;
  color: #2d3135;
  margin-top: 0;
  margin-bottom: 0.85em;
  padding-bottom: 0.4em;
  border-bottom: 2px solid #52adc8;
}

.home-card {
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.06);
  padding: 1.15em 1.4em;
  margin-bottom: 0.85em;
  transition: box-shadow 0.18s ease, transform 0.18s ease;
}
.home-card:last-child { margin-bottom: 0; }
.home-card:hover { box-shadow: 0 5px 18px rgba(0,0,0,0.11); transform: translateY(-2px); }
.home-card .card-title { font-size: 1em; font-weight: 700; color: #2d3135; margin: 0 0 0.2em 0; }
.home-card .card-subtitle {
  font-size: 0.8em;
  color: #7a8288;
  margin: 0 0 0.65em 0;
  display: flex;
  align-items: center;
  gap: 0.4em;
  flex-wrap: wrap;
}
.home-card .card-subtitle a { color: #52adc8; text-decoration: none; }
.home-card .card-subtitle a:hover { text-decoration: underline; }
.home-card .card-body { font-size: 0.92em; color: #494e52; line-height: 1.65; margin: 0; }
.home-card .card-body a { color: #52adc8; text-decoration: none; }
.home-card .card-body a:hover { text-decoration: underline; }
.home-card .card-badge {
  display: inline-block;
  margin-top: 0.6em;
  margin-right: 0.3em;
  padding: 0.2em 0.65em;
  background: #d9eef5;
  color: #2e7d96;
  border-radius: 3px;
  font-size: 0.7em;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}

/* Company logo badges */
.co-badge {
  display: inline-block;
  width: 22px;
  height: 22px;
  border-radius: 4px;
  vertical-align: middle;
  flex-shrink: 0;
}
.co-badge img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  border-radius: 4px;
}

.home-cards-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0.85em;
}
.home-cards-grid .home-card { margin-bottom: 0; }
@media (min-width: 768px) {
  .home-cards-grid { grid-template-columns: repeat(2, 1fr); }
}

.interest-tags { display: flex; flex-wrap: wrap; gap: 0.5em; }
.interest-tag {
  display: inline-block;
  padding: 0.35em 0.9em;
  background: #f0f1f1;
  border: 1px solid #d3d5d6;
  border-radius: 20px;
  font-size: 0.8em;
  color: #494e52;
  font-weight: 500;
}

.achievement-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
  gap: 0.75em;
}
.achievement-card {
  text-align: center;
  padding: 1.1em 0.75em;
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 8px;
  box-shadow: 0 1px 4px rgba(0,0,0,0.05);
}
.achievement-card .achievement-rank { font-size: 1.953em; font-weight: 800; color: #52adc8; line-height: 1.1; }
.achievement-card .achievement-exam { font-size: 0.7em; font-weight: 700; color: #494e52; text-transform: uppercase; letter-spacing: 0.06em; margin-top: 0.3em; }
.achievement-card .achievement-year { font-size: 0.625em; color: #7a8288; margin-top: 0.2em; }

.nav-cards {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 0.85em;
}
@media (min-width: 768px) {
  .nav-cards { grid-template-columns: repeat(3, 1fr); }
}
.nav-card {
  display: block;
  text-align: center;
  padding: 1.2em 0.75em;
  background: #fff;
  border: 1px solid #e8e8e8;
  border-radius: 8px;
  text-decoration: none !important;
  color: #494e52 !important;
  font-weight: 600;
  font-size: 0.8em;
  transition: background 0.18s ease, color 0.18s ease, box-shadow 0.18s ease, transform 0.18s ease;
  box-shadow: 0 1px 4px rgba(0,0,0,0.05);
}
.nav-card .nav-card-icon { font-size: 1.35em; display: block; margin-bottom: 0.4em; color: #52adc8; transition: color 0.18s ease; }
.nav-card:hover { background: #52adc8 !important; color: #fff !important; border-color: #52adc8; box-shadow: 0 5px 14px rgba(82,173,200,0.35); transform: translateY(-2px); }
.nav-card:hover .nav-card-icon { color: #fff; }
</style>

<div class="home-intro">
  Applied Scientist at <a href="https://www.microsoft.com/en-us/research/group/microsoft-turing/">Microsoft Turing</a>, building AI reasoning and agent capabilities for <a href="https://www.microsoft.com/en-us/microsoft-365/copilot">M365 Copilot</a>. IIT Bombay CSE '23. Interested in LLMs, NLP, and applied ML.
</div>

<div class="home-section">
  <h2 class="home-section-title">Current Role</h2>
  <div class="home-card">
    <div class="card-title">Applied Scientist</div>
    <div class="card-subtitle">
      <span class="co-badge"><img src="/images/logos/microsoft.png" alt="Microsoft"></span>
      <a href="https://www.microsoft.com/en-us/research/group/microsoft-turing/">Microsoft Turing</a>
      &middot; Aug 2024 &ndash; Present
    </div>
    <div class="card-body">
      Working on M365 Copilot's AI reasoning and agent capabilities. Key contributions:
      <ul style="margin: 0.5em 0 0.5em 1.2em; padding: 0;">
        <li>Built the <strong>Analyst Agent</strong> — prompt-engineered Python Code Interpreter (CI) integration that improved CI trigger rate by <strong>~100%</strong> and user satisfaction by <strong>~150%</strong>.</li>
        <li>Improved numerical citation rendering for CI output, yielding a <strong>40% improvement</strong> in P99/P95 ChatLTR.</li>
        <li>Drove GPT-5 transition; prompt structure optimizations reduced ChatFTR by <strong>30%</strong> across performance tiers.</li>
        <li>Developed <strong>synthetic data generation pipelines</strong> for fine-tuning reasoning models across code generation, data analysis, web search, and multi-site crawling use cases.</li>
        <li>Built <strong>synthetic tenant generation</strong> systems producing realistic enterprise environments (emails, meetings, calendar events) for agent training and evaluation.</li>
        <li>Implemented agentic graders for the <strong>Outlook Agent</strong> to detect hallucinations and measure inbox coverage.</li>
      </ul>
      <span class="card-badge">LLMs</span><span class="card-badge">Prompt Engineering</span><span class="card-badge">Agent Systems</span><span class="card-badge">Synthetic Data</span>
    </div>
  </div>
</div>

<div class="home-section">
  <h2 class="home-section-title">Education</h2>
  <div class="home-card">
    <div class="card-title">B.Tech in Computer Science &amp; Engineering (with Honors)</div>
    <div class="card-subtitle">
      <span class="co-badge"><img src="/images/logos/iitb.png" alt="IIT Bombay"></span>
      <a href="https://www.iitb.ac.in/">IIT Bombay</a>
      &middot; 2019 &ndash; 2023
    </div>
    <div class="card-body">
      Minor in Data Science and Machine Learning &nbsp;&middot;&nbsp; CGPA: <strong>9.04 / 10</strong>
    </div>
  </div>
</div>

<div class="home-section">
  <h2 class="home-section-title">Full-time Experience</h2>
  <div class="home-card">
    <div class="card-title">Data Analyst II</div>
    <div class="card-subtitle">
      <span class="co-badge"><img src="/images/logos/walmart.png" alt="Walmart"></span>
      <a href="https://www.walmartglobaltech.com/">Walmart Global Tech India</a>
      &middot; Jul 2023 &ndash; Jul 2024
    </div>
    <div class="card-body">
      Worked on the <strong>Smart Subs</strong> team, recommending substitute items when products go out of stock. Trained <strong>XGBoost</strong> and <strong>Neural Network</strong> models to rerank substitutes based on user preferences from historical data. Improved quantity ratio logic to account for item pricing, achieving a <strong>10% reduction</strong> in average price of substitutes recommended to customers.
      <br><span class="card-badge">ML</span><span class="card-badge">Recommender Systems</span><span class="card-badge">XGBoost</span>
    </div>
  </div>
</div>

<div class="home-section">
  <h2 class="home-section-title">Internships</h2>
  <div class="home-cards-grid">
    <div class="home-card">
      <div class="card-title">Machine Learning Intern</div>
      <div class="card-subtitle">
        <span class="co-badge"><img src="/images/logos/knowdis.png" alt="KnowDis"></span>
        KnowDis Data Science
        &middot; Jan 2023 &ndash; May 2023
      </div>
      <div class="card-body">
        Developed deep learning models for <strong>background removal</strong> and <strong>human body parsing</strong> as part of a deep fashion project. Fine-tuned a <strong>ViT-based Segformer</strong> on semantic segmentation datasets, and integrated <strong>Segment Anything</strong> and <strong>Grounding DINO</strong> for targeted object retention.
        <br><span class="card-badge">Computer Vision</span><span class="card-badge">ViT / Segformer</span>
      </div>
    </div>
    <div class="home-card">
      <div class="card-title">Quantitative Trader Intern</div>
      <div class="card-subtitle">
        <span class="co-badge"><img src="/images/logos/quadeye.png" alt="Quadeye"></span>
        <a href="https://www.quadeye.com/">Quadeye Securities</a>
        &middot; May 2022 &ndash; Jul 2022
      </div>
      <div class="card-body">
        Developed <strong>crypto trading strategies</strong> using Quadeye's proprietary tech stack. Backtested strategies on historical data with constraints on gross exposure, delta, volumes, positions, and orders — ensuring liquidation of positions upon expiry.
        <br><span class="card-badge">Quant Finance</span><span class="card-badge">Algo Trading</span>
      </div>
    </div>
  </div>
</div>

<div class="home-section">
  <h2 class="home-section-title">Research Interests</h2>
  <div class="interest-tags">
    <span class="interest-tag">Applied Machine Learning</span>
    <span class="interest-tag">Large Language Models</span>
    <span class="interest-tag">Natural Language Processing</span>
    <span class="interest-tag">Computer Vision</span>
  </div>
</div>

<div class="home-section">
  <h2 class="home-section-title">Academic Achievements</h2>
  <div class="achievement-cards">
    <div class="achievement-card">
      <div class="achievement-rank">AIR 48</div>
      <div class="achievement-exam">JEE Advanced</div>
      <div class="achievement-year">2019</div>
    </div>
    <div class="achievement-card">
      <div class="achievement-rank">AIR 42</div>
      <div class="achievement-exam">JEE Main</div>
      <div class="achievement-year">2019</div>
    </div>
    <div class="achievement-card">
      <div class="achievement-rank">AIR 19</div>
      <div class="achievement-exam">KVPY</div>
      <div class="achievement-year">&nbsp;</div>
    </div>
  </div>
</div>

<div class="home-section">
  <h2 class="home-section-title">Explore</h2>
  <div class="nav-cards">
    <a class="nav-card" href="/projects/">
      <span class="nav-card-icon"><i class="fas fa-code"></i></span>
      Projects
    </a>
    <a class="nav-card" href="/blog/">
      <span class="nav-card-icon"><i class="fas fa-pen"></i></span>
      Blog Posts
    </a>
    <a class="nav-card" href="/cv/">
      <span class="nav-card-icon"><i class="fas fa-file-alt"></i></span>
      CV
    </a>
  </div>
</div>
