---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
/* Hide the layout-generated homepage title. The name appears only once in the left profile card. */
.page__title {
  display: none !important;
}

.profile-hero {
  border: 1px solid #d9e5ee;
  border-radius: 30px;
  padding: 38px 42px;
  margin: 0 0 28px 0;
  background:
    linear-gradient(135deg, rgba(245, 250, 253, .96) 0%, rgba(239, 247, 250, .96) 56%, rgba(250, 252, 247, .98) 100%),
    #ffffff;
  box-shadow: 0 14px 38px rgba(25, 55, 80, 0.09);
}
.profile-eyebrow {
  display: inline-flex;
  align-items: center;
  padding: 6px 12px;
  border: 1px solid #cfe1ec;
  border-radius: 999px;
  color: #285e78;
  background: rgba(255,255,255,.68);
  font-size: .82rem;
  font-weight: 650;
  margin-bottom: 16px;
}
.profile-statement {
  font-size: 1.06rem;
  line-height: 1.62;
  margin: 0 0 18px;
  color: #263f52;
  font-weight: 700;
  font-style: italic;
  max-width: 820px;
}
.profile-hero p {
  font-size: 1.06rem;
  color: #344f63;
  max-width: 820px;
  margin: 0 0 18px;
}
.profile-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 22px;
}
.profile-pill {
  display: inline-flex;
  padding: 7px 11px;
  border-radius: 999px;
  background: #ffffff;
  border: 1px solid #ccdde8;
  color: #244b62;
  font-size: .78rem;
  font-weight: 700;
}
.academic-section {
  margin-top: 30px;
  padding: 28px 32px;
  border: 1px solid #d9e5ee;
  border-radius: 24px;
  background: rgba(255,255,255,.9);
  box-shadow: 0 9px 24px rgba(25,55,80,.045);
}
.section-header {
  display: flex;
  justify-content: space-between;
  align-items: end;
  gap: 20px;
  border-bottom: 2px solid #e0ebf2;
  padding-bottom: 12px;
  margin-bottom: 18px;
}
.section-header h2 {
  font-size: 1.55rem;
  margin: 0;
  letter-spacing: -.015em;
  font-weight: 650;
  color: #173b57;
}
.section-kicker {
  font-size: .78rem;
  font-weight: 800;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: #7ca58d;
  white-space: nowrap;
}
.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 16px;
}
.info-card,
.service-card {
  border: 1px solid #e3ebf1;
  border-radius: 18px;
  padding: 18px 18px 16px;
  background: #ffffff;
  box-shadow: 0 8px 20px rgba(31,64,93,.04);
}
.info-card h3,
.service-card h3 {
  margin: 0 0 8px;
  font-size: 1.02rem;
  color: #173b57;
}
.info-card p,
.service-card p {
  margin: 0;
  color: #627386;
  font-size: .96rem;
  line-height: 1.58;
}
.timeline {
  border-left: 3px solid #d4e4ef;
  padding-left: 18px;
  margin-top: 10px;
}
.timeline-item {
  position: relative;
  margin: 0 0 24px;
  padding: 2px 0 2px;
}
.timeline-item::before {
  content: '';
  position: absolute;
  left: -27px;
  top: 7px;
  width: 13px;
  height: 13px;
  background: #526d7a;
  border-radius: 50%;
  box-shadow: 0 0 0 5px #edf6fa;
}
.timeline-item.current::before {
  background: #87510f;
  box-shadow: 0 0 0 5px #fff2d8;
}
.timeline-title-row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 14px;
  flex-wrap: wrap;
  margin-bottom: 8px;
}
.timeline-item strong {
  display: block;
  font-size: 1.05rem;
  color: #173b57;
}
.timeline-item.current strong {
  color: #87510f;
}
.current-badge {
  display: inline-flex;
  padding: 4px 9px;
  border-radius: 999px;
  background: #fff2d8;
  border: 1px solid #f0bf67;
  color: #87510f;
  font-size: .74rem;
  font-weight: 750;
  text-transform: uppercase;
  letter-spacing: .04em;
  box-shadow: 0 5px 12px rgba(190, 126, 34, .13);
}
.date-badge {
  display: inline-flex;
  padding: 4px 9px;
  border-radius: 999px;
  background: #eef5f8;
  border: 1px solid #d5e5ed;
  color: #526d7a;
  font-size: .74rem;
  font-weight: 700;
  letter-spacing: .02em;
}
.edu-details {
  display: grid;
  grid-template-columns: 120px minmax(0, 1fr);
  gap: 4px 12px;
  color: #627386;
  font-size: .95rem;
}
.edu-label {
  color: #426273;
  font-size: .82rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: .04em;
}
.pub-list {
  display: grid;
  gap: 14px;
}
.pub-highlight {
  display: block;
  color: inherit;
  text-decoration: none;
  border-left: 5px solid #6f9ab5;
  border-radius: 0 18px 18px 0;
  background: #fbfdff;
  padding: 16px 18px;
  border-top: 1px solid #e4edf3;
  border-right: 1px solid #e4edf3;
  border-bottom: 1px solid #e4edf3;
  transition: transform .18s ease, box-shadow .18s ease, background .18s ease;
  cursor: pointer;
}
.pub-highlight:hover {
  transform: translateY(-2px);
  background: #ffffff;
  box-shadow: 0 10px 24px rgba(35, 72, 105, .09);
}
.pub-highlight p {
  margin: 0 0 8px;
  line-height: 1.55;
}
.doi-text {
  color: #2d6f8e;
  font-size: .88rem;
  font-weight: 650;
}
.tag-row {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin-top: 8px;
}
.tag {
  font-size: .74rem;
  font-weight: 700;
  padding: 4px 8px;
  border-radius: 999px;
  background: #edf5fb;
  color: #2f5b78;
  border: 1px solid #d7e7f4;
}
.small-note {
  color: #627386;
  font-size: .92rem;
  margin-top: 12px;
}
.editorial-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 12px;
  margin-top: 10px;
}
.editorial-tag {
  display: block;
  padding: 14px 15px;
  border: 1px solid #d8e6ee;
  border-radius: 7px;
  background: linear-gradient(135deg, #fbfdff 0%, #f3f8fb 100%);
  color: inherit;
  text-decoration: none;
  transition: transform .18s ease, box-shadow .18s ease, border-color .18s ease;
}
.editorial-tag:hover {
  text-decoration: none;
  transform: translateY(-2px);
  border-color: #bcd4e3;
  box-shadow: 0 10px 22px rgba(35, 72, 105, .08);
}
.role-tag {
  display: inline-flex;
  padding: 4px 9px;
  border-radius: 7px;
  background: #eaf6f1;
  border: 1px solid #cde5d9;
  color: #356a51;
  font-size: .72rem;
  font-weight: 800;
  text-transform: none;
  letter-spacing: .01em;
  margin-bottom: 8px;
}
.editorial-period {
  display: block;
  color: #6a7f8f;
  font-size: .72rem;
  font-weight: 650;
  margin-bottom: 4px;
}
.editorial-journal {
  display: block;
  color: #173b57;
  font-size: .98rem;
  line-height: 1.36;
  margin-bottom: 4px;
  font-weight: 700;
}
.journal-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 8px 10px;
  margin-top: 14px;
}
.journal-item {
  padding: 9px 11px;
  border: 1px solid #e3ebf2;
  border-radius: 12px;
  background: #f9fbfd;
  color: #344f63;
  font-size: .9rem;
  line-height: 1.42;
}
.journal-rank {
  display: block;
  margin-top: 2px;
  color: #6a7f8f;
  font-size: .74rem;
  font-weight: 700;
  letter-spacing: .02em;
}
@media (max-width: 900px) {
  .profile-hero { padding: 30px 26px; }
  .academic-section { padding: 24px 22px; }
  .edu-details { grid-template-columns: 1fr; }
}
</style>

<div class="profile-hero">
  <div class="profile-eyebrow">Academic Homepage</div>
  <p class="profile-statement"><strong><em>PhD candidate working at the intersection of AI-assisted language learning, EFL writing, and learner psychology.</em></strong></p>
  <p>I am a PhD candidate in Applied Linguistics at the Department of Foreign Languages and Literatures, Tsinghua University. My research examines how modern technologies, including AI-assisted learning environments and digital writing tools, shape learners’ motivation, strategy use, engagement, and reflective development in English as a foreign language contexts.</p>
  <p>Before joining Tsinghua University, I completed an M.A. in Applied Linguistics in Foreign Languages at Beijing Language and Culture University and a B.A. in English Language and Literature at Sichuan International Studies University.</p>
  <div class="profile-meta">
    <span class="profile-pill">EFL Writing</span>
    <span class="profile-pill">AI-Assisted Language Learning</span>
    <span class="profile-pill">Self-Regulated Learning</span>
    <span class="profile-pill">Technology Acceptance</span>
    <span class="profile-pill">Research Synthesis</span>
  </div>
</div>

<div class="academic-section" id="research">
  <div class="section-header">
    <h2>Research Interests</h2>
    <div class="section-kicker">Areas of expertise</div>
  </div>
  <div class="card-grid">
    <div class="info-card">
      <h3>Technology-enhanced language learning</h3>
      <p>AI-assisted language learning, digital academic reading, automated writing feedback, pedagogical agents, and learner–technology interaction.</p>
    </div>
    <div class="info-card">
      <h3>Second language writing</h3>
      <p>EFL writing strategies, writing self-regulation, writing feedback, information seeking, and reflective strategy evaluation.</p>
    </div>
    <div class="info-card">
      <h3>Positive psychology in EFL learning</h3>
      <p>Learner motivation, enjoyment, academic buoyancy, engagement, grit, self-efficacy, and psychologically supportive learning environments.</p>
    </div>
    <div class="info-card">
      <h3>Research synthesis and methodology</h3>
      <p>Systematic review, bibliometric analysis, meta-analysis, structural equation modeling, mixed methods, and scale development.</p>
    </div>
  </div>
</div>

<div class="academic-section">
  <div class="section-header">
    <h2>Current Research Agenda</h2>
    <div class="section-kicker">Ongoing work</div>
  </div>
  <p>My current research agenda focuses on <strong>active second language learning in technology-mediated environments</strong>, especially in EFL writing. I am interested in how learners proactively seek resources, interact with feedback, evaluate learning strategies, and construct productive relationships with AI-supported tools.</p>
  <p>This line of work connects applied linguistics with educational psychology and human-computer interaction by asking how language learners become more agentic, reflective, and strategically adaptive in digital learning contexts.</p>
</div>

<div class="academic-section" id="education">
  <div class="section-header">
    <h2>Education</h2>
    <div class="section-kicker">Academic background</div>
  </div>
  <div class="timeline">
    <div class="timeline-item current">
      <div class="timeline-title-row">
        <strong>Tsinghua University</strong>
        <span class="current-badge">Current · 2025.09–Present</span>
      </div>
      <div class="edu-details">
        <div class="edu-label">Aff.</div>
        <div>Department of Foreign Languages and Literatures</div>
        <div class="edu-label">Status</div>
        <div>PhD Candidate in Applied Linguistics</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-title-row">
        <strong>Beijing Language and Culture University</strong>
        <span class="date-badge">2022.09–2025.06</span>
      </div>
      <div class="edu-details">
        <div class="edu-label">Degree</div>
        <div>M.A. in Literature</div>
        <div class="edu-label">Field</div>
        <div>Applied Linguistics in Foreign Languages</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-title-row">
        <strong>Sichuan International Studies University</strong>
        <span class="date-badge">2018.09–2022.06</span>
      </div>
      <div class="edu-details">
        <div class="edu-label">Degree</div>
        <div>B.A. in English Language and Literature</div>
      </div>
    </div>
  </div>
</div>

<div class="academic-section" id="publications">
  <div class="section-header">
    <h2>Selected Publications</h2>
    <div class="section-kicker">Journal articles</div>
  </div>
  <div class="pub-list">
    <div class="pub-highlight" role="link" tabindex="0" onclick="window.open('https://doi.org/10.1111/ijal.70092', '_blank')" onkeydown="if(event.key==='Enter'||event.key===' '){window.open('https://doi.org/10.1111/ijal.70092', '_blank')}">
      <p><strong>Lin, Y., &amp; Liu, M.</strong> (2026). From self-prepared writers to strategy effectiveness evaluators: Mediation of critical thinking during self-regulated EFL writing. <em>International Journal of Applied Linguistics</em>, 1–13.</p>
      <span class="doi-text">doi:10.1111/ijal.70092</span>
      <div class="tag-row"><span class="tag">EFL writing</span><span class="tag">Self-regulated learning</span><span class="tag">Critical thinking</span></div>
    </div>
    <div class="pub-highlight" role="link" tabindex="0" onclick="window.open('https://doi.org/10.1080/10447318.2024.2359222', '_blank')" onkeydown="if(event.key==='Enter'||event.key===' '){window.open('https://doi.org/10.1080/10447318.2024.2359222', '_blank')}">
      <p><strong>Lin, Y., &amp; Yu, Z.</strong> (2025). Learner perceptions of artificial intelligence-generated pedagogical agents in language learning videos: Embodiment effects on technology acceptance. <em>International Journal of Human-Computer Interaction</em>, 41(2), 1606–1627.</p>
      <span class="doi-text">doi:10.1080/10447318.2024.2359222</span>
      <div class="tag-row"><span class="tag">AI pedagogical agents</span><span class="tag">Embodiment</span><span class="tag">Technology acceptance</span></div>
    </div>
    <div class="pub-highlight" role="link" tabindex="0" onclick="window.open('https://doi.org/10.1057/s41599-024-03861-1', '_blank')" onkeydown="if(event.key==='Enter'||event.key===' '){window.open('https://doi.org/10.1057/s41599-024-03861-1', '_blank')}">
      <p><strong>Lin, Y., &amp; Yu, Z.</strong> (2025). Elucidating university students’ intentions to seek automated writing feedback from Grammarly: Toward perceptual and systemic predictors. <em>Humanities and Social Sciences Communications</em>, 12, 7.</p>
      <span class="doi-text">doi:10.1057/s41599-024-03861-1</span>
      <div class="tag-row"><span class="tag">Automated writing feedback</span><span class="tag">Grammarly</span><span class="tag">EFL learners</span></div>
    </div>
    <div class="pub-highlight" role="link" tabindex="0" onclick="window.open('https://doi.org/10.1186/s41239-023-00403-8', '_blank')" onkeydown="if(event.key==='Enter'||event.key===' '){window.open('https://doi.org/10.1186/s41239-023-00403-8', '_blank')}">
      <p><strong>Lin, Y., &amp; Yu, Z.</strong> (2023). Extending Technology Acceptance Model to higher-education students’ use of digital academic reading tools on computers. <em>International Journal of Educational Technology in Higher Education</em>, 20, 34.</p>
      <span class="doi-text">doi:10.1186/s41239-023-00403-8</span>
      <div class="tag-row"><span class="tag">Digital academic reading</span><span class="tag">Higher education</span><span class="tag">TAM</span></div>
    </div>
  </div>
  <p class="small-note">Click a publication card to open its DOI page. For a fuller list of journal articles, review papers, and conference presentations, please see the <a href="/publications/">Publications</a> page.</p>
</div>

<div class="academic-section" id="service">
  <div class="section-header">
    <h2>Academic Service</h2>
    <div class="section-kicker">Editorial & reviewing</div>
  </div>
  <div class="card-grid">
    <div class="service-card">
      <h3>Editorial service</h3>
      <div class="editorial-grid">
        <a class="editorial-tag" href="https://www.emeraldgrouppublishing.com/journal/qae" target="_blank" rel="noopener">
          <span class="role-tag">Editorial Advisory Board Member</span>
          <span class="editorial-period">June 2024–present</span>
          <span class="editorial-journal"><em>Quality Assurance in Education</em></span>
        </a>
        <a class="editorial-tag" href="https://www.wiserpub.com/journals/ser/" target="_blank" rel="noopener">
          <span class="role-tag">Editorial Board Member</span>
          <span class="editorial-period">May 2026–present</span>
          <span class="editorial-journal"><em>Social Education Research</em></span>
        </a>
      </div>
    </div>
    <div class="service-card">
      <h3>Reviewing expertise</h3>
      <p>Educational technology, applied linguistics, language education, human-computer interaction, educational psychology, higher education, and research synthesis.</p>
    </div>
  </div>
  <div class="service-card" style="margin-top:16px;">
    <h3>Invited reviewer for journals</h3>
    <div class="journal-grid">
      <div class="journal-item"><em>Computers &amp; Education</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>International Journal of STEM Education</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>System</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Computer Assisted Language Learning</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Language Teaching Research</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Language Learning &amp; Technology</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>International Journal of Human-Computer Interaction</em><span class="journal-rank">SSCI/SCI Q1</span></div>
      <div class="journal-item"><em>Interactive Learning Environments</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Education and Information Technologies</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Teaching and Teacher Education</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>European Journal of Psychology of Education</em><span class="journal-rank">SSCI Q2</span></div>
      <div class="journal-item"><em>IEEE Transactions on Learning Technologies</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Journal of Educational Computing Research</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>The Asia-Pacific Education Researcher</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Journal of Computer Assisted Learning</em><span class="journal-rank">SSCI Q1</span></div>
      <div class="journal-item"><em>Journal of Educational Research</em><span class="journal-rank">SSCI Q2</span></div>
      <div class="journal-item"><em>Behaviour &amp; Information Technology</em><span class="journal-rank">SSCI Q2</span></div>
      <div class="journal-item"><em>Universal Access in the Information Society</em><span class="journal-rank">SCI Q2</span></div>
      <div class="journal-item"><em>Learning and Motivation</em><span class="journal-rank">SSCI Q3</span></div>
      <div class="journal-item"><em>Humanities and Social Sciences Communications</em><span class="journal-rank">SSCI Q1 · AHCI</span></div>
    </div>
  </div>
</div>
