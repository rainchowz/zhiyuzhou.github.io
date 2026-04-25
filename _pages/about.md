---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
:root {
  --zz-blue: #2f6fb3;
  --zz-blue-dark: #174f8a;
  --zz-blue-soft: #eaf4ff;
  --zz-blue-line: #c7ddf5;
  --zz-text: #243447;
  --zz-muted: #6b7f96;
  --zz-border: #dbe8f6;
  --zz-bg: #f8fbff;
}

/* Sidebar polish */
.author__name {
  color: var(--zz-blue-dark);
  font-weight: 800;
}

.author__urls a,
.author__urls_sm a,
.zz-home a {
  color: var(--zz-blue-dark);
  text-decoration: none;
  transition: color 0.2s ease, transform 0.2s ease;
}

.author__urls a:hover,
.author__urls_sm a:hover,
.zz-home a:hover {
  color: var(--zz-blue);
  text-decoration: none;
}

.author__urls a {
  display: inline-block;
}

.author__urls a:hover {
  transform: translateX(3px);
}

.author__urls li {
  transition: transform 0.2s ease;
}

.author__urls li:hover {
  transform: translateX(2px);
}

/* Navigation active state */
.masthead__menu-item a {
  transition: color 0.2s ease;
}

.masthead__menu-item a.is-active {
  color: var(--zz-blue-dark) !important;
  font-weight: 800;
}

.zz-home {
  color: var(--zz-text);
}

.zz-home .anchor {
  display: block;
  position: relative;
  top: -84px;
  visibility: hidden;
}

.zz-intro a,
.zz-paper-title a,
.zz-row-right a {
  display: inline-block;
}

.zz-intro a:hover,
.zz-paper-title a:hover,
.zz-row-right a:hover {
  transform: translateY(-1px);
}

.zz-section-title {
  display: flex;
  align-items: center;
  gap: 0.55rem;
  margin-top: 2.1rem;
  margin-bottom: 1rem;
  padding-bottom: 0.35rem;
  border-bottom: 2px solid var(--zz-blue-line);
  color: var(--zz-blue-dark);
  font-size: 1.55rem;
  font-weight: 800;
  letter-spacing: 0;
}

.zz-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 1.85rem;
  height: 1.85rem;
  border-radius: 8px;
  background: var(--zz-blue-soft);
  color: var(--zz-blue-dark);
  font-size: 1.05rem;
  line-height: 1;
  transition: transform 0.2s ease, background 0.2s ease;
}

.zz-section-title:hover .zz-icon {
  transform: translateY(-2px) rotate(-3deg);
  background: #dceeff;
}

.zz-intro {
  padding: 1.1rem 1.25rem;
  border-left: 4px solid var(--zz-blue);
  background: linear-gradient(90deg, rgba(234, 244, 255, 0.9), rgba(248, 251, 255, 0.45));
  border-radius: 8px;
}

.zz-intro p {
  margin: 0 0 0.85rem;
}

.zz-intro p:last-child {
  margin-bottom: 0;
}

.zz-highlight {
  display: inline-block;
  font-weight: 800;
  color: var(--zz-blue-dark);
  transition: transform 0.2s ease;
}

.zz-highlight:hover {
  transform: translateX(4px);
}

.zz-news {
  margin: 0;
  padding-left: 1.1rem;
}

.zz-news li {
  margin-bottom: 0.55rem;
  transition: transform 0.2s ease;
}

.zz-news li:hover {
  transform: translateX(4px);
}

.zz-date {
  font-weight: 800;
  color: var(--zz-blue-dark);
}

.zz-paper {
  display: grid;
  grid-template-columns: minmax(150px, 230px) 1fr;
  gap: 1.25rem;
  align-items: center;
  padding: 1.2rem 0;
  border-bottom: 1px solid var(--zz-border);
  transition: transform 0.22s ease;
}

.zz-paper:hover {
  transform: translateY(-2px);
}

.zz-paper-cover {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  border: 1px solid var(--zz-border);
  background: var(--zz-bg);
  box-shadow: 0 8px 20px rgba(47, 111, 179, 0.10);
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
}

.zz-paper-cover::after {
  content: "";
  position: absolute;
  top: -20%;
  left: -80%;
  width: 45%;
  height: 140%;
  background: linear-gradient(
    90deg,
    rgba(255, 255, 255, 0),
    rgba(255, 255, 255, 0.55),
    rgba(255, 255, 255, 0)
  );
  transform: skewX(-18deg);
  transition: left 0.65s ease;
  pointer-events: none;
}

.zz-paper-cover:hover {
  transform: translateY(-3px);
  border-color: var(--zz-blue-line);
  box-shadow: 0 12px 28px rgba(47, 111, 179, 0.18);
}

.zz-paper-cover:hover::after {
  left: 130%;
}

.zz-paper-cover img {
  display: block;
  width: 100%;
  height: auto;
}

.zz-badge {
  position: absolute;
  top: 0.55rem;
  left: 0.55rem;
  padding: 0.22rem 0.55rem;
  border-radius: 6px;
  background: rgba(23, 79, 138, 0.92);
  color: #fff;
  font-size: 0.78rem;
  font-weight: 800;
  z-index: 1;
}

.zz-paper-title {
  margin: 0 0 0.45rem;
  font-size: 1.05rem;
  line-height: 1.35;
  font-weight: 800;
}

.zz-paper-authors,
.zz-paper-note {
  margin: 0.35rem 0;
  color: var(--zz-muted);
  line-height: 1.55;
}

.zz-paper-note {
  color: var(--zz-text);
}

.zz-two-col-list {
  margin-top: 0.3rem;
  border-top: 1px solid var(--zz-border);
}

.zz-row {
  display: grid;
  grid-template-columns: minmax(180px, 240px) 1fr;
  gap: 1.25rem;
  padding: 1rem 0;
  border-bottom: 1px solid var(--zz-border);
  align-items: center;
  transition: transform 0.22s ease, background 0.22s ease;
}

.zz-row:hover {
  transform: translateX(4px);
  background: linear-gradient(90deg, rgba(234, 244, 255, 0.45), rgba(255, 255, 255, 0));
}

.zz-row-left {
  color: var(--zz-muted);
  font-size: 0.95rem;
  line-height: 1.45;
}

.zz-row-left strong {
  display: block;
  color: var(--zz-blue-dark);
  font-weight: 800;
}

.zz-row-right {
  line-height: 1.55;
}

.zz-row-title {
  margin: 0 0 0.25rem;
  color: var(--zz-text);
  font-size: 1.03rem;
  font-weight: 800;
}

.zz-row-meta {
  margin: 0.15rem 0;
  color: var(--zz-muted);
}

.zz-education-left,
.zz-experience-left {
  display: grid;
  grid-template-columns: 58px 1fr;
  gap: 0.75rem;
  align-items: center;
}

.zz-school-logo,
.zz-lab-logo {
  width: 58px;
  height: 58px;
  border-radius: 8px;
  object-fit: cover;
  border: 1px solid var(--zz-border);
  box-shadow: 0 4px 12px rgba(47, 111, 179, 0.10);
  transition: transform 0.22s ease, box-shadow 0.22s ease;
}

.zz-row:hover .zz-school-logo,
.zz-row:hover .zz-lab-logo {
  transform: translateY(-2px);
  box-shadow: 0 8px 18px rgba(47, 111, 179, 0.16);
}

.zz-date-range {
  display: inline-block;
  margin-top: 0.18rem;
  line-height: 1.35;
  white-space: nowrap;
}

@media (max-width: 700px) {
  .zz-paper,
  .zz-row {
    grid-template-columns: 1fr;
    gap: 0.75rem;
  }

  .zz-paper-cover {
    max-width: 280px;
  }

  .zz-section-title {
    font-size: 1.35rem;
  }

  .zz-date-range {
    white-space: normal;
  }
}
</style>

<div class="zz-home">

<span class='anchor' id='about-me'></span>

<h1 class="zz-section-title"><span class="zz-icon">👋</span>About Me</h1>

<div class="zz-intro" markdown="1">

I am **Zhiyu Zhou** (**周志宇** in Chinese), a senior undergraduate student in **Software Engineering** at **Jilin University**, advised by <a href="https://www.hongxiaxie.net/" target="_blank" rel="noopener noreferrer"><strong>Prof. Hongxia Xie</strong></a>.

My current research focuses on **multimodal large language models (MLLMs)**, **embodied AI**, and **computer vision**. I am particularly interested in the synergy among **perception**, **understanding**, and **action**, with the goal of building intelligent systems that can interact more naturally with the physical world and better align with human-like cognitive processes.

<span class="zz-highlight">My long-term goal is to advance artificial intelligence from understanding toward perception and action in the real world.</span>

**Email:** [zhouzy1622@mails.jlu.edu.cn](mailto:zhouzy1622@mails.jlu.edu.cn)

</div>

<span class='anchor' id='news'></span>

<h1 class="zz-section-title"><span class="zz-icon">🔥</span>News</h1>

<ul class="zz-news">
  <li><span class="zz-date">2026.02</span>: Our work <strong>MindPower</strong> was accepted to <strong>CVPR 2026</strong>.</li>
</ul>

<span class='anchor' id='publications'></span>

<h1 class="zz-section-title"><span class="zz-icon">📝</span>Publications</h1>

<div class="zz-paper">
  <div class="zz-paper-cover">
    <div class="zz-badge">PinpointQA</div>
    <img src="images/pinpointqa.png" alt="PinpointQA project preview">
  </div>
  <div>
    <p class="zz-paper-title">
      <a href="https://rainchowz.github.io/PinpointQA/" target="_blank" rel="noopener noreferrer">PinpointQA: A Dataset and Benchmark for Small Object-Centric Spatial Understanding in Indoor Videos</a>
    </p>
    <p class="zz-paper-authors">
      <strong>Zhiyu Zhou</strong>, Peilin Liu, Ruoxuan Zhang, Luyang Zhang, Cheng Zhang, Hongxia Xie, Wen-Huang Cheng
    </p>
    <p class="zz-paper-note">
      PinpointQA focuses on small object-centric spatial understanding in indoor videos, providing a dataset and benchmark for evaluating fine-grained spatial perception and reasoning.
    </p>
  </div>
</div>

<div class="zz-paper">
  <div class="zz-paper-cover">
    <div class="zz-badge">CVPR 2026</div>
    <img src="images/mindpower.png" alt="MindPower project preview">
  </div>
  <div>
    <p class="zz-paper-title">
      <a href="https://zhangdaxia22.github.io/MindPower/" target="_blank" rel="noopener noreferrer">MindPower: Enabling Theory-of-Mind Reasoning in VLM-based Embodied Agents</a>
    </p>
    <p class="zz-paper-authors">
      Ruoxuan Zhang, Qiyun Zheng, <strong>Zhiyu Zhou</strong>, Ziqi Liao, Siyu Wu, Jian-Yu Jiang-Lin, Bin Wen, Hongxia Xie, Jianlong Fu, Wen-Huang Cheng
    </p>
    <p class="zz-paper-note">
      <strong>CVPR 2026.</strong> MindPower explores Theory-of-Mind reasoning in vision-language-model-based embodied agents, aiming to improve how agents infer intentions, beliefs, and goals during embodied interaction.
    </p>
  </div>
</div>

<span class='anchor' id='education'></span>

<h1 class="zz-section-title"><span class="zz-icon">🎓</span>Education</h1>

<div class="zz-two-col-list">
  <div class="zz-row">
    <div class="zz-row-left zz-education-left">
      <img class="zz-school-logo" src="images/jilin-university.jpg" alt="Jilin University">
      <div>
        <strong>Jilin University</strong>
        <span class="zz-date-range">Sept. 2022 - Jun. 2026</span><br>
        <span>Expected</span>
      </div>
    </div>
    <div class="zz-row-right">
      <p class="zz-row-title">B.Eng. in Software Engineering</p>
      <p class="zz-row-meta">Senior undergraduate student, School of Software, Jilin University.</p>
    </div>
  </div>
</div>

<span class='anchor' id='experience'></span>

<h1 class="zz-section-title"><span class="zz-icon">🧪</span>Experience</h1>

<div class="zz-two-col-list">
  <div class="zz-row">
    <div class="zz-row-left zz-experience-left">
      <img class="zz-lab-logo" src="images/avclab.png" alt="Affective Vision Computing Lab">
      <div>
        <strong>Research Assistant</strong>
        <span class="zz-date-range">2025 - Present</span>
      </div>
    </div>
    <div class="zz-row-right">
      <p class="zz-row-title">Affective Vision Computing (AVC) Lab, Jilin University</p>
      <p class="zz-row-meta">Supervisor: <a href="https://www.hongxiaxie.net/" target="_blank" rel="noopener noreferrer">Prof. Hongxia Xie</a></p>
    </div>
  </div>
</div>

<span class='anchor' id='honors-and-awards'></span>

<h1 class="zz-section-title"><span class="zz-icon">🏆</span>Honors and Awards</h1>

<div class="zz-two-col-list">
  <div class="zz-row">
    <div class="zz-row-left">
      <strong>Undergraduate Scholarship</strong>
      <span class="zz-date-range">2022 - 2025</span>
    </div>
    <div class="zz-row-right">
      <p class="zz-row-title">Jilin University</p>
      <p class="zz-row-meta">Awarded during undergraduate study.</p>
    </div>
  </div>
</div>

</div>
