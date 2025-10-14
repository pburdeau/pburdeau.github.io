---
layout: default
title: "Home"
permalink: /
---

<div class="profile">
  <img class="photo" src="/assets/img/avatar.jpg" alt="Portrait of Philippine Burdeau">
  <div class="identity">
    <h1>Philippine Burdeau</h1>
    <p><span id="phdYear">PhD student</span> working with <a href="https://eao.stanford.edu/" target="_blank" rel="noopener">Prof. Adam Brandt</a> at Stanford.</p>
    <div class="social">
      <!-- Scholar -->
      <a class="icon oxblood" href="https://scholar.google.com/citations?user=sJb11sYAAAAJ&hl=fr" aria-label="Google Scholar" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M4 19.5V6.8a2 2 0 0 1 2-2h12"/>
          <path d="M6 18.5a2 2 0 0 1 2-2h12v3H8a2 2 0 0 1-2-2Z"/>
          <path d="M6 6.5h12v8H8a2 2 0 0 1-2-2V6.5Z"/>
        </svg>
      </a>

      <!-- LinkedIn -->
      <a class="icon sage" href="https://www.linkedin.com/in/philippine-burdeau/" aria-label="LinkedIn" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/>
          <rect x="2" y="9" width="4" height="12" rx="1"/>
          <circle cx="4" cy="5" r="2"/>
        </svg>
      </a>

      <!-- GitHub -->
      <a class="icon charcoal" href="https://github.com/pburdeau" aria-label="GitHub" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.9a3.4 3.4 0 0 0-.9-2.6c3 0 6-1.5 6-6a4.6 4.6 0 0 0-1.3-3.2 4.2 4.2 0 0 0-.1-3.2S17.8 2.7 15 4a12.1 12.1 0 0 0-6 0C6.3 2.7 3.3 2.3 3.3 2.3a4.2 4.2 0 0 0-.1 3.2A4.6 4.6 0 0 0 1.9 8c0 4.4 3 6 6 6a3.4 3.4 0 0 0-.9 2.6V22"/>
        </svg>
      </a>

      <!-- Email -->
      <a class="icon brass" href="mailto:pburdeau@stanford.edu" aria-label="Email">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M4 6h16a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2z"/>
          <path d="m22 8-10 6L2 8"/>
        </svg>
      </a>
    </div>

  </div>

  <div class="spot">
    <img src="/assets/img/spotlight.jpg" alt="Personified image placeholder">
    <small>Swap this with a personified image: a map crop, notebook scan, or hand‑drawn motif.</small>
  </div>
</div>

<h2 class="section-title">Summary</h2>
<p>I'm <span id="age">27</span> and a <strong><span id="phdYearInline">4th‑year</span></strong> PhD student in Energy Resources Engineering (since 2022), working with Prof. Adam Brandt in the <a href="https://eao.stanford.edu/" target="_blank" rel="noopener">Environmental Assessment & Optimization</a> group. Before Stanford, I studied applied math and physics at <em>École Polytechnique</em> and completed an MSc in <em>Politics & Policy Analysis</em> at <em>Bocconi University</em>.</p>

<h2 class="section-title">Key Topics</h2>
<ul class="big-bullets">
  <li>Intermittency (HMMs), detection‑aware estimation</li>
  <li>Produced gas composition: kriging + non‑linear modeling</li>
  <li>Reproducible pipelines; maps and visualization</li>
</ul>

<script>
(function(){
  const now = new Date();
  const birth = new Date('1998-02-26T00:00:00');
  let age = now.getFullYear() - birth.getFullYear();
  const mdiff = now.getMonth() - birth.getMonth();
  if (mdiff < 0 || (mdiff === 0 && now.getDate() < birth.getDate())) age--;
  document.getElementById('age').textContent = age;

  // PhD year since 2022; roll to next academic year on Sep 1
  const y = now.getFullYear();
  const afterSep = now.getMonth() >= 8; // 0-based months
  let yearNum = (y - 2022) + (afterSep ? 1 : 0);
  if (yearNum < 1) yearNum = 1;
  const ord = (n)=>{
    if (n % 10 == 1 && n % 100 != 11) return n + 'st';
    if (n % 10 == 2 && n % 100 != 12) return n + 'nd';
    if (n % 10 == 3 && n % 100 != 13) return n + 'rd';
    return n + 'th';
  };
  const text = ord(yearNum) + '‑year';
  const el1 = document.getElementById('phdYear');
  const el2 = document.getElementById('phdYearInline');
  if (el1) el1.textContent = text + ' PhD student';
  if (el2) el2.textContent = text;
})();
</script>