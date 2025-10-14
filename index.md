---
layout: default
title: "Home"
permalink: /
---

<div class="profile">
  <img class="photo" src="/assets/img/avatar.jpg" alt="Portrait of Philippine Burdeau">
  <div class="identity">
    <h1>Philippine Burdeau</h1>
    <p>I am a <strong><span id="phdYearInline">PhD student</span></strong> working with <a href="https://eao.stanford.edu/" target="_blank" rel="noopener">Prof. Adam Brandt</a> at Stanford. I am originally from France.</p>
    <div class="social">
      <!-- Google Scholar -->
      <a class="icon" href="https://scholar.google.com/citations?user=sJb11sYAAAAJ&hl=fr" aria-label="Google Scholar" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M3 7l9-4 9 4-9 4-9-4z" />
          <path d="M21 10l-9 4-9-4" />
          <path d="M12 14v7" />
        </svg>
      </a>
      <!-- LinkedIn -->
      <a class="icon" href="https://www.linkedin.com/in/philippine-burdeau/" aria-label="LinkedIn" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <rect x="2" y="9" width="4" height="12" rx="1"/>
          <path d="M9 9h4v2a4 4 0 0 1 8 0v10h-4V12a2 2 0 0 0-4 0v9H9z"/>
          <circle cx="4" cy="5" r="2"/>
        </svg>
      </a>
      <!-- GitHub -->
      <a class="icon" href="https://github.com/pburdeau" aria-label="GitHub" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.9a3.4 3.4 0 0 0-.9-2.6c3 0 6-1.5 6-6a4.6 4.6 0 0 0-1.3-3.2 4.2 4.2 0 0 0-.1-3.2S17.8 2.7 15 4a12.1 12.1 0 0 0-6 0C6.3 2.7 3.3 2.3 3.3 2.3a4.2 4.2 0 0 0-.1 3.2A4.6 4.6 0 0 0 1.9 8c0 4.4 3 6 6 6a3.4 3.4 0 0 0-.9 2.6V22"/>
        </svg>
      </a>
      <!-- Email -->
      <a class="icon" href="mailto:pburdeau@stanford.edu" aria-label="Email">
        <svg viewBox="0 0 24 24" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <rect x="3" y="5" width="18" height="14" rx="2"/>
          <path d="M3 7l9 6 9-6"/>
        </svg>
      </a>
    </div>
  </div>

  <div class="spot">
    <img src="/assets/img/spotlight.jpg" alt="Research or personal spotlight image">
    <small>Replace with a research figure, a Boston–Stanford collage, or a map crop—this is where color lives.</small>
  </div>
</div>

<h2 class="section-title">Summary</h2>
<p>I am <span id="age">27</span> years old and a <strong><span id="phdYearText">4th‑year PhD student</span></strong> in Energy Resources Engineering (since 2022), working with Prof. Adam Brandt in the <a href="https://eao.stanford.edu/" target="_blank" rel="noopener">Environmental Assessment & Optimization</a> group. Before Stanford, I studied applied mathematics and physics at <em>École Polytechnique</em> (France) and completed an MSc in <em>Politics & Policy Analysis</em> at <em>Bocconi University</em>.</p>

<h2 class="section-title">Work nooks</h2>
<p>I like quiet corners with books and daylight. A few regulars:</p>

<div class="nooks">
  <figure class="nook">
    <img src="/assets/img/athenaeum.jpg" alt="Reading room at the Boston Athenæum">
    <figcaption>
      Boston Athenæum
      <small>oak tables, whisper‑quiet; perfect for long reads</small>
    </figcaption>
  </figure>
  <figure class="nook">
    <img src="/assets/img/green-library.jpg" alt="Cecil H. Green Library (Bing Wing), Stanford">
    <figcaption>
      Green Library (Stanford)
      <small>campus calm; a good place to think in full sentences</small>
    </figcaption>
  </figure>
  <figure class="nook">
    <img src="/assets/img/third-place.jpg" alt="Another favorite quiet workspace">
    <figcaption>
      A third place
      <small>changes with the week—quiet, bright, close to coffee</small>
    </figcaption>
  </figure>
</div>

<script>
(function(){
  const now = new Date();
  const birth = new Date('1998-02-26T00:00:00');
  let age = now.getFullYear() - birth.getFullYear();
  const mdiff = now.getMonth() - birth.getMonth();
  if (mdiff < 0 || (mdiff === 0 && now.getDate() < birth.getDate())) age--;
  const ageEl = document.getElementById('age'); if (ageEl) ageEl.textContent = age;

  // PhD year since 2022; roll to next academic year on Sep 1
  const y = now.getFullYear();
  const afterSep = now.getMonth() >= 8;
  let yearNum = (y - 2022) + (afterSep ? 1 : 0);
  if (yearNum < 1) yearNum = 1;
  const ord = (n)=>{
    if (n % 10 == 1 && n % 100 != 11) return n + 'st';
    if (n % 10 == 2 && n % 100 != 12) return n + 'nd';
    if (n % 10 == 3 && n % 100 != 13) return n + 'rd';
    return n + 'th';
  };
  const text = ord(yearNum) + '‑year PhD student';
  const t1 = document.getElementById('phdYearInline');
  const t2 = document.getElementById('phdYearText');
  if (t1) t1.textContent = text;
  if (t2) t2.textContent = text;
})();
</script>