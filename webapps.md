---
title: "**Web Applications**"
layout: post
---

<nav>
  <a href="https://joshmartinecon.github.io/">Home</a> | 
  <a href="https://nbviewer.org/github/joshmartinecon/quarto-cv/blob/main/joshmartin_cv.pdf" target="_blank" rel="noopener noreferrer">CV</a> | 
  <a href="https://joshmartinecon.github.io/research.html">Research</a> | 
  <a href="https://joshmartinecon.github.io/teaching.html">Teaching</a>
  <a href="https://joshmartinecon.github.io/webapps.html">WebApps</a>
</nav>

---

<style>
/* ---- accordion (same behavior as the publications page) ---- */
button.accordion-button {
background-color: #f1f1f1;
color: black;
cursor: pointer;
padding: 14px;
width: 100%;
border: none;
text-align: left;
outline: none;
font-size: 19px;
font-weight: bold;
transition: 0.4s;
border-radius: 5px;
margin: 10px 0;
}
button.accordion-button.active, button.accordion-button:hover {
background-color: #ccc;
}
button.accordion-button:before {
content: "+ ";
font-size: 24px;
color: blue;
line-height: 24px;
float: left;
margin-right: 8px;
}
button.accordion-button.active:before {
content: "- ";
}

/* ---- panel contents ---- */
.app-panel {
display: none;
background-color: #f9f9f9;
padding: 16px 18px;
border-radius: 5px;
font-size: 18px;
line-height: 1.6;
}
.app-panel p { margin: 0 0 12px 0; }
.app-updated {
color: #666;
font-size: 16px;
font-style: italic;
}

/* ---- link buttons ---- */
.app-links { margin-top: 14px; }
.app-links a {
display: inline-block;
padding: 9px 20px;
margin-right: 10px;
border-radius: 5px;
font-size: 16px;
font-weight: bold;
text-decoration: none;
border: 1px solid #2b5797;
}
.app-links a.primary { background-color: #2b5797; color: #fff; }
.app-links a.primary:hover { background-color: #1d3c69; }
.app-links a.secondary { background-color: #fff; color: #2b5797; }
.app-links a.secondary:hover { background-color: #e8eefa; }

.intro { font-size: 18px; line-height: 1.6; }
</style>

<script>
function toggleAccordion(element) {
var content = element.nextElementSibling;
if (content.style.display === 'none' || content.style.display === '') {
content.style.display = 'block';
element.classList.add("active");
} else {
content.style.display = 'none';
element.classList.remove("active");
}
}
</script>

<p class="intro">Interactive tools that I build and maintain. Click any app for details.</p>

<button class="accordion-button" onclick="toggleAccordion(this)">Economics Journal Rankings</button>
<div class="app-panel">
<p>A searchable table of economics journals ranked by a composite score that averages twelve RePEc citation-based rankings onto a common scale, matched against ABDC quality grades.</p>
<p class="app-updated">Last updated: May 2026</p>
<div class="app-links">
<a class="primary" href="https://joshua-c-martin.shinyapps.io/EconJournalRankings/" target="_blank" rel="noopener noreferrer">Open app</a>
<a class="secondary" href="https://github.com/joshmartinecon/econ-journal-rankings" target="_blank" rel="noopener noreferrer">Source code</a>
</div>
</div>

<button class="accordion-button" onclick="toggleAccordion(this)">WNBA Ratings &amp; Optimal Rotations</button>
<div class="app-panel">
<p>Player ratings on a 60&ndash;99 scale built from playing-time-weighted efficiency metrics, paired with a model of how many minutes each player should be getting, so you can see which teams are closest to their best possible rotation.</p>
<p class="app-updated">Refreshed daily during the season</p>
<div class="app-links">
<a class="primary" href="https://joshua-c-martin.shinyapps.io/wnba-ratings/" target="_blank" rel="noopener noreferrer">Open app</a>
<a class="secondary" href="https://github.com/joshmartinecon/wnba-ratings" target="_blank" rel="noopener noreferrer">Source code</a>
</div>
</div>

<button class="accordion-button" onclick="toggleAccordion(this)">NFL Fantasy Draft Assistant</button>
<div class="app-panel">
<p>A live draft board that re-values every remaining player after each pick, combining value over replacement at his position with how many roster spots you still have open at that position.</p>
<p class="app-updated">Last updated: September 2026</p>
<div class="app-links">
<a class="primary" href="https://joshua-c-martin.shinyapps.io/fantasy-football-drafter/" target="_blank" rel="noopener noreferrer">Open app</a>
<a class="secondary" href="https://github.com/joshmartinecon/fantasy-football-drafter" target="_blank" rel="noopener noreferrer">Source code</a>
</div>
</div>
