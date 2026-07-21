---
layout: default
title: CV
description: "Resume and CV overview."
---

<section class="page-hero narrow-hero">
  <p class="eyebrow">CV / Resume</p>
  <h1>CV</h1>
  <p>{{ site.data.profile.resume.intro }}</p>
</section>

<section class="section resume-section" aria-labelledby="experience-title">
  <div class="section-heading">
    <p class="eyebrow">Experience</p>
    <h2 id="experience-title">Experience</h2>
  </div>
  <div class="resume-list">
    {% for item in site.data.profile.resume.experience %}
      <article class="resume-item">
        <div>
          <h3>{{ item.role }}</h3>
          <p>{{ item.org }}</p>
        </div>
        <time>{{ item.dates }}</time>
        <p>{{ item.text }}</p>
      </article>
    {% endfor %}
  </div>
</section>

<section class="section resume-section" aria-labelledby="education-title">
  <div class="section-heading">
    <p class="eyebrow">Education</p>
    <h2 id="education-title">Education</h2>
  </div>
  <div class="resume-list">
    {% for item in site.data.profile.resume.education %}
      <article class="resume-item">
        <div>
          <h3>{{ item.degree }}</h3>
          <p>{{ item.school }}</p>
        </div>
        <time>{{ item.dates }}</time>
        <p>{{ item.text }}</p>
      </article>
    {% endfor %}
  </div>
</section>

<section class="section skills-section" aria-labelledby="skills-title">
  <div class="section-heading">
    <p class="eyebrow">Skills</p>
    <h2 id="skills-title">Skills</h2>
  </div>
  <div class="tag-row large-tags">
    {% for skill in site.data.profile.resume.skills %}
      <span>{{ skill }}</span>
    {% endfor %}
  </div>
</section>
