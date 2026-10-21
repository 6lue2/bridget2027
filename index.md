---
layout: post
title: Portfolio Home
hide: true
show_reading_time: false
---

<div class="bridget-dashboard">

<style>
.bridget-dashboard {
  --navy: #101f2b;
  --navy-light: #192d3b;
  --navy-card: #203744;
  --green: #244e43;
  --green-light: #356b58;
  --sage: #a5c4ad;
  --mint: #d0e5d5;
  --coral: #e88b72;
  --cream: #f2f0e8;
  --muted: #b4c5c7;
  --line: rgba(190, 214, 202, .2);

  color: var(--cream);
  font-family: inherit;
  max-width: 1200px;
  margin: 0 auto;
}

.bridget-dashboard * {
  box-sizing: border-box;
}

.bridget-dashboard a {
  text-decoration: none !important;
}

.bridget-dashboard .bd-hero {
  position: relative;
  overflow: hidden;
  padding: clamp(28px, 5vw, 64px);
  margin: 0 0 28px;
  border-radius: 22px;
  background:
    radial-gradient(ellipse at 95% 5%, rgba(53,107,88,.5), transparent 40%),
    linear-gradient(125deg, #101f2b 0%, #172f3a 60%, #21483e 100%);
  border: 1px solid rgba(190,214,202,.18);
  min-height: 255px;
  display: flex;
  align-items: center;
}

.bridget-dashboard .bd-hero::after {
  content: "ENGINEERING  /  COMPUTER SCIENCE";
  position: absolute;
  right: -18px;
  bottom: 26px;
  font-size: clamp(9px, 1.2vw, 12px);
  letter-spacing: .2em;
  color: rgba(208,229,213,.35);
  transform: rotate(-90deg) translateX(100%);
  transform-origin: right bottom;
}

.bridget-dashboard .bd-hero-content {
  position: relative;
  z-index: 1;
  max-width: 720px;
}

.bridget-dashboard .bd-eyebrow {
  color: var(--sage);
  font-size: .76rem;
  font-weight: 800;
  letter-spacing: .2em;
  text-transform: uppercase;
  margin: 0 0 18px;
}

.bridget-dashboard .bd-hero h1 {
  color: var(--cream);
  font-family: Georgia, "Times New Roman", serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 500;
  letter-spacing: -.055em;
  line-height: .98;
  margin: 0;
}

.bridget-dashboard .bd-hero h1 span {
  color: var(--sage);
  font-style: italic;
}

.bridget-dashboard .bd-hero-copy {
  max-width: 520px;
  color: var(--muted);
  font-size: 1rem;
  line-height: 1.8;
  margin: 22px 0 0;
}

.bridget-dashboard .bd-hero-mark {
  position: absolute;
  right: 8%;
  top: 18%;
  color: rgba(165,196,173,.13);
  font-family: Georgia, serif;
  font-size: clamp(100px, 18vw, 220px);
  line-height: 1;
  font-weight: bold;
  pointer-events: none;
}

.bridget-dashboard .bd-section {
  margin: 0 0 28px;
  padding: clamp(20px, 3.5vw, 38px);
  background: #142733;
  border: 1px solid var(--line);
  border-radius: 22px;
}

.bridget-dashboard .bd-section-head {
  display: grid;
  grid-template-columns: auto 1fr auto;
  gap: 20px;
  align-items: center;
  margin-bottom: 26px;
}

.bridget-dashboard .bd-index {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 60px;
  height: 60px;
  border-radius: 16px;
  color: var(--navy);
  background: var(--sage);
  font-size: 1.2rem;
  font-weight: 900;
  letter-spacing: -.04em;
}

.bridget-dashboard .bd-section:nth-of-type(3) .bd-index {
  background: var(--coral);
}

.bridget-dashboard .bd-section-title {
  margin: 0;
  color: var(--cream);
  font-family: Georgia, "Times New Roman", serif;
  font-size: clamp(1.65rem, 3.5vw, 2.5rem);
  font-weight: 500;
  line-height: 1.1;
  letter-spacing: -.035em;
}

.bridget-dashboard .bd-section-subtitle {
  color: var(--muted);
  margin: 8px 0 0;
  font-size: .92rem;
  line-height: 1.6;
}

.bridget-dashboard .bd-section-tag {
  align-self: start;
  padding: 8px 11px;
  border: 1px solid var(--line);
  border-radius: 99px;
  color: var(--sage);
  font-size: .68rem;
  letter-spacing: .12em;
  white-space: nowrap;
}

.bridget-dashboard .bd-card {
  position: relative;
  overflow: hidden;
  background: var(--navy-light);
  border: 1px solid var(--line);
  border-radius: 16px;
  padding: 24px;
  margin-top: 14px;
  transition: border-color .2s ease, transform .2s ease,
              background .2s ease;
}

.bridget-dashboard .bd-card:hover {
  border-color: rgba(165,196,173,.55);
  background: #1b3340;
}

.bridget-dashboard .bd-card-top {
  display: flex;
  align-items: flex-start;
  gap: 16px;
}

.bridget-dashboard .bd-icon {
  flex: 0 0 44px;
  width: 44px;
  height: 44px;
  display: grid;
  place-items: center;
  border-radius: 13px;
  background: rgba(165,196,173,.12);
  border: 1px solid rgba(165,196,173,.2);
  color: var(--sage);
  font-size: 1.2rem;
}

.bridget-dashboard .bd-card h3 {
  margin: 0;
  color: var(--cream);
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.3rem;
  font-weight: 500;
  line-height: 1.35;
}

.bridget-dashboard .bd-card p {
  color: var(--muted);
  font-size: .9rem;
  line-height: 1.7;
  margin: 5px 0 0;
}

.bridget-dashboard .bd-action {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  margin-top: 18px;
  padding: 11px 16px;
  border-radius: 8px;
  background: var(--green-light);
  color: #fff !important;
  border: 1px solid rgba(208,229,213,.16);
  font-size: .84rem;
  font-weight: 750;
  transition: background .2s ease, transform .2s ease;
}

.bridget-dashboard .bd-action:hover {
  background: #447e68;
  transform: translateY(-1px);
}

.bridget-dashboard .bd-action .bd-arrow {
  color: var(--mint);
  font-size: 1rem;
}

.bridget-dashboard .bd-action-coral {
  background: #824c43;
}

.bridget-dashboard .bd-action-coral:hover {
  background: #a65e50;
}

.bridget-dashboard .bd-subhead {
  display: flex;
  align-items: center;
  gap: 12px;
  margin: 30px 0 14px;
  color: var(--cream);
  font-size: .75rem;
  font-weight: 800;
  letter-spacing: .16em;
  text-transform: uppercase;
}

.bridget-dashboard .bd-subhead::after {
  content: "";
  height: 1px;
  flex: 1;
  background: var(--line);
}

.bridget-dashboard .bd-units {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 12px;
}

.bridget-dashboard .bd-unit {
  position: relative;
  min-height: 150px;
  padding: 19px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  overflow: hidden;
  border: 1px solid var(--line);
  border-radius: 13px;
  background: #1c3540;
  transition: transform .2s ease, border-color .2s ease;
}

.bridget-dashboard .bd-unit:hover {
  transform: translateY(-3px);
  border-color: var(--sage);
}

.bridget-dashboard .bd-unit:nth-child(2) {
  background: #1b3a3c;
}

.bridget-dashboard .bd-unit:nth-child(3) {
  background: #3a3038;
}

.bridget-dashboard .bd-unit:nth-child(4) {
  background: #34352f;
}

.bridget-dashboard .bd-unit-number {
  color: var(--sage);
  font-size: .7rem;
  font-weight: 800;
  letter-spacing: .14em;
}

.bridget-dashboard .bd-unit:nth-child(3) .bd-unit-number {
  color: var(--coral);
}

.bridget-dashboard .bd-unit h4 {
  color: var(--cream);
  margin: 18px 0 5px;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.35rem;
  font-weight: 500;
}

.bridget-dashboard .bd-unit p {
  color: var(--muted);
  margin: 0;
  font-size: .78rem;
  line-height: 1.5;
}

.bridget-dashboard .bd-unit-arrow {
  align-self: flex-end;
  color: var(--sage);
  font-size: 1.15rem;
  margin-top: 10px;
}

.bridget-dashboard .bd-unit:nth-child(3) .bd-unit-arrow {
  color: var(--coral);
}

.bridget-dashboard .bd-lesson-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 10px;
}

.bridget-dashboard .bd-lesson {
  min-width: 0;
  border: 1px solid var(--line);
  border-radius: 12px;
  overflow: hidden;
  background: #1b303b;
}

.bridget-dashboard .bd-lesson:nth-child(2) {
  background: #1c3838;
}

.bridget-dashboard .bd-lesson:nth-child(3) {
  background: #392f35;
}

.bridget-dashboard .bd-lesson:nth-child(4) {
  background: #34352f;
}

.bridget-dashboard .bd-lesson summary {
  list-style: none;
  cursor: pointer;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 8px;
  min-height: 70px;
  padding: 15px;
  color: var(--cream);
  font-size: .84rem;
  font-weight: 700;
}

.bridget-dashboard .bd-lesson summary::-webkit-details-marker {
  display: none;
}

.bridget-dashboard .bd-lesson summary::after {
  content: "+";
  flex-shrink: 0;
  color: var(--sage);
  font-size: 1.2rem;
  font-weight: 400;
}

.bridget-dashboard .bd-lesson[open] summary::after {
  content: "−";
}

.bridget-dashboard .bd-lesson summary:hover {
  color: var(--sage);
}

.bridget-dashboard .bd-lesson-content {
  padding: 0 12px 14px;
}

.bridget-dashboard .bd-lesson-content .bd-action {
  display: flex;
  width: 100%;
  margin-top: 0;
  padding: 10px 8px;
  font-size: .77rem;
}

.bridget-dashboard .bd-standard {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  padding: 22px;
  margin-top: 20px;
  background: linear-gradient(110deg, #1c3837, #1b303b);
  border: 1px solid rgba(165,196,173,.25);
  border-radius: 15px;
}

.bridget-dashboard .bd-standard-copy {
  display: flex;
  align-items: flex-start;
  gap: 15px;
}

.bridget-dashboard .bd-standard .bd-action {
  flex-shrink: 0;
  margin-top: 0;
}

.bridget-dashboard .bd-footer {
  display: flex;
  justify-content: space-between;
  gap: 12px;
  padding: 10px 4px 26px;
  color: var(--muted);
  font-size: .75rem;
  letter-spacing: .04em;
}

.bridget-dashboard .bd-footer span:last-child {
  color: var(--sage);
}

@media (max-width: 760px) {
  .bridget-dashboard .bd-units,
  .bridget-dashboard .bd-lesson-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .bridget-dashboard .bd-section-head {
    grid-template-columns: auto 1fr;
    gap: 14px;
  }

  .bridget-dashboard .bd-section-tag {
    grid-column: 2;
    justify-self: start;
  }

  .bridget-dashboard .bd-standard {
    align-items: flex-start;
    flex-direction: column;
  }
}

@media (max-width: 460px) {
  .bridget-dashboard .bd-hero {
    padding: 28px 22px;
  }

  .bridget-dashboard .bd-hero::after {
    display: none;
  }

  .bridget-dashboard .bd-section {
    padding: 18px;
  }

  .bridget-dashboard .bd-index {
    width: 46px;
    height: 46px;
  }

  .bridget-dashboard .bd-card {
    padding: 18px;
  }

  .bridget-dashboard .bd-units {
    gap: 8px;
  }

  .bridget-dashboard .bd-unit {
    padding: 14px;
    min-height: 135px;
  }

  .bridget-dashboard .bd-lesson summary {
    padding: 12px 10px;
    font-size: .76rem;
  }
}
</style>

<!-- HERO -->

<header class="bd-hero">
  <div class="bd-hero-content">
    <p class="bd-eyebrow">My Portfolio &nbsp; / &nbsp; 2026–2027</p>
    <h1>Bridget <span>Xiao.</span></h1>
    <p class="bd-hero-copy">
      Exploring the intersection of computer science, engineering,
      and thoughtful problem-solving. A record of what I build,
      what I learn, and what comes next.
    </p>
  </div>
  <div class="bd-hero-mark" aria-hidden="true">BX</div>
</header>

<!-- SPRINT 1 -->

<section class="bd-section">
  <div class="bd-section-head">
    <div class="bd-index">01</div>
    <div>
      <h2 class="bd-section-title">Sprint 1 Retrospective</h2>
      <p class="bd-section-subtitle">
        Establishing foundations, exploring core concepts,
        and documenting early progress.
      </p>
    </div>
    <div class="bd-section-tag">FOUNDATIONS</div>
  </div>

  <div class="bd-card">
    <div class="bd-card-top">
      <div class="bd-icon" aria-hidden="true">⌘</div>
      <div>
        <h3>Ground 0</h3>
        <p>Initial setup, project kickoff, and development groundwork.</p>
        <a class="bd-action"
           href="https://github.com/6lue2/bridget2027/issues/2"
           target="_blank" rel="noopener noreferrer">
          View on GitHub <span class="bd-arrow">↗</span>
        </a>
      </div>
    </div>
  </div>

  <div class="bd-subhead">AP Computer Science A <span>01 — 04</span></div>

  <p class="bd-section-subtitle" style="margin: -3px 0 16px;">
    Explore my progress through the first four units.
  </p>

  <div class="bd-units">
    <a class="bd-unit" href="{{site.baseurl}}/csalessons/unit1">
      <span class="bd-unit-number">UNIT 01</span>
      <div>
        <h4>Unit 1</h4>
        <p>Primitive types</p>
      </div>
      <span class="bd-unit-arrow">↗</span>
    </a>

    <a class="bd-unit" href="{{site.baseurl}}/csalessons/unit2">
      <span class="bd-unit-number">UNIT 02</span>
      <div>
        <h4>Unit 2</h4>
        <p>Using objects</p>
      </div>
      <span class="bd-unit-arrow">↗</span>
    </a>

    <a class="bd-unit" href="{{site.baseurl}}/csalessons/unit3">
      <span class="bd-unit-number">UNIT 03</span>
      <div>
        <h4>Unit 3</h4>
        <p>Boolean expressions</p>
      </div>
      <span class="bd-unit-arrow">↗</span>
    </a>

    <a class="bd-unit" href="{{site.baseurl}}/csalessons/unit4">
      <span class="bd-unit-number">UNIT 04</span>
      <div>
        <h4>Unit 4</h4>
        <p>Iteration</p>
      </div>
      <span class="bd-unit-arrow">↗</span>
    </a>
  </div>
</section>

<!-- SPRINT 2 -->

<section class="bd-section">
  <div class="bd-section-head">
    <div class="bd-index">02</div>
    <div>
      <h2 class="bd-section-title">Sprint 2 Retrospective</h2>
      <p class="bd-section-subtitle">
        Expanding the work through analytics, lesson creation,
        and better tools for teaching.
      </p>
    </div>
    <div class="bd-section-tag">IN PROGRESS</div>
  </div>

  <div class="bd-card">
    <div class="bd-card-top">
      <div class="bd-icon" aria-hidden="true">⌘</div>
      <div>
        <h3>Ground 1</h3>
        <p>Next steps, project updates, and continued development.</p>
        <a class="bd-action"
           href="https://github.com/6lue2/bridget2027/issues/9#issue-5966266971"
           target="_blank" rel="noopener noreferrer">
          View on GitHub <span class="bd-arrow">↗</span>
        </a>
      </div>
    </div>
  </div>

  <div class="bd-card">
    <div class="bd-card-top">
      <div class="bd-icon" aria-hidden="true">↗</div>
      <div>
        <h3>OCS Analytics &amp; Self Assessment</h3>
        <p>Progress tracking, data collection, and reflection.</p>
        <a class="bd-action bd-action-coral" href="{{site.baseurl}}/foundations/analyticsprogress">
          View Project <span class="bd-arrow">↗</span>
        </a>
      </div>
    </div>
  </div>

  <div class="bd-subhead">Creating Lessons <span>1.09 — 1.12</span></div>

  <p class="bd-section-subtitle" style="margin: -3px 0 16px;">
    Select a lesson to reveal its page link.
  </p>

  <div class="bd-lesson-grid">
    <details class="bd-lesson">
      <summary>CB Lesson 1.09</summary>
      <div class="bd-lesson-content">
        <a class="bd-action"
           href="https://pages.opencodingsociety.com/topics/view/csa/unit_01/1_9/?category=java">
          View Lesson <span class="bd-arrow">↗</span>
        </a>
      </div>
    </details>

    <details class="bd-lesson">
      <summary>CB Lesson 1.10</summary>
      <div class="bd-lesson-content">
        <a class="bd-action"
           href="https://pages.opencodingsociety.com/topics/view/csa/unit_01/1_10/?category=java">
          View Lesson <span class="bd-arrow">↗</span>
        </a>
      </div>
    </details>

    <details class="bd-lesson">
      <summary>CB Lesson 1.11</summary>
      <div class="bd-lesson-content">
        <a class="bd-action"
           href="https://pages.opencodingsociety.com/topics/view/csa/unit_01/1_11/?category=java">
          View Lesson <span class="bd-arrow">↗</span>
        </a>
      </div>
    </details>

    <details class="bd-lesson">
      <summary>CB Lesson 1.12</summary>
      <div class="bd-lesson-content">
        <a class="bd-action"
           href="https://pages.opencodingsociety.com/topics/view/csa/unit_01/1_12/?category=java">
          View Lesson <span class="bd-arrow">↗</span>
        </a>
      </div>
    </details>
  </div>

  <div class="bd-standard">
    <div class="bd-standard-copy">
      <div class="bd-icon" aria-hidden="true">✳</div>
      <div>
        <h3 style="margin:0;color:var(--cream);font-family:Georgia,'Times New Roman',serif;font-size:1.25rem;font-weight:500;">
          Lesson Standardization for Teaching
        </h3>
        <p style="margin:5px 0 0;color:var(--muted);font-size:.88rem;line-height:1.6;">
          Consistent lesson structures and OCS submission guidelines.
        </p>
      </div>
    </div>
    <a class="bd-action"
       href="https://pages.opencodingsociety.com/topics/view/csa/unit_04/submission-roles/?q=OCS+Roles"
       target="_blank" rel="noopener noreferrer">
      View OCS Roles <span class="bd-arrow">↗</span>
    </a>
  </div>
</section>

<footer class="bd-footer">
  <span>BRIDGET XIAO &nbsp; · &nbsp; PORTFOLIO</span>
  <span>BUILD. LEARN. REFINE.</span>
</footer>

</div>
