---
layout: academic
title: Academic profile
permalink: /
redirect_from:
  - /about/
  - /about.html
---

<section class="hero" aria-labelledby="about-me">
  <div class="wrap hero-inner">
    <div class="profile">
      <p class="field">System identification &amp; control theory</p>
      <h1 id="about-me">{{ site.author.name }}</h1>
      <p class="biography">I received my PhD in Computer and Information Engineering from The Chinese University of Hong Kong, Shenzhen, under the supervision of Prof. Tianshi Chen. I will be joining LMU as a postdoctoral researcher.</p>
      <ul class="profile-links" aria-label="Contact and academic profiles">
        <li><a href="mailto:{{ site.author.email }}"><span class="icon icon-email" aria-hidden="true"></span>Email</a></li>
        <li><a href="{{ site.author.googlescholar | escape }}"><span class="icon icon-scholar" aria-hidden="true"></span>Google Scholar</a></li>
        <li><a href="{{ site.author.orcid }}"><span class="icon icon-orcid" aria-hidden="true"></span>ORCID</a></li>
        <li><a href="{{ site.author.github }}"><span class="icon icon-github" aria-hidden="true"></span>GitHub</a></li>
      </ul>
    </div>
    <figure class="portrait">
      <div class="portrait-stage">
        <img src="{{ site.author.avatar | prepend: '/images/' | relative_url }}" alt="Portrait of Xiaozhu Fang" width="823" height="770" fetchpriority="high">
      </div>
      <figcaption><span class="location-mark" aria-hidden="true"></span>{{ site.author.location }}</figcaption>
    </figure>
  </div>
</section>

<div class="wrap home-body">
  <div class="research-spread">
    <section class="research" aria-labelledby="research-interests">
      <h2 id="research-interests">Research interests</h2>
      <ul class="interests">
        <li>System identification in the time and frequency domains</li>
        <li>Gaussian processes, regularization, and reproducing kernel Hilbert spaces (RKHS)</li>
        <li>Fourier analysis and functional analysis for system theory</li>
      </ul>
    </section>
    <aside class="thesis" aria-labelledby="thesis-title">
      <p class="thesis-label">Doctoral thesis</p>
      <h2 id="thesis-title"><a href="https://irepository.cuhk.edu.cn/handle/3EPUXD0A/102941?mode=full">On Fourier Analysis for Kernel-Based System Identification</a></h2>
      <p class="thesis-meta">The Chinese University of Hong Kong, Shenzhen · 2026</p>
    </aside>
  </div>

  <section class="selected ruled-section" aria-labelledby="selected-title">
    <div class="section-title"><h2 id="selected-title">Selected publications</h2><a class="text-link" href="{{ '/publications/' | relative_url }}">All publications</a></div>
    {% assign featured = site.data.papers | where: 'selected', true | sort: 'year' | reverse %}
    <ul class="paper-list">
      {% for paper in featured %}{% include paper-row.html paper=paper %}{% endfor %}
    </ul>
  </section>

  <section class="education ruled-section" aria-labelledby="education">
    <h2 id="education">Education</h2>
    <dl class="education-list">
      <div><dt>May 2026</dt><dd><strong>PhD in Computer and Information Engineering</strong><span>The Chinese University of Hong Kong, Shenzhen</span></dd></div>
      <div><dt>May 2020</dt><dd><strong>MS in Mechanical Engineering</strong><span>University of Michigan, Ann Arbor</span></dd></div>
      <div><dt>May 2020</dt><dd><strong>MS in Electrical and Computer Engineering</strong><span>University of Michigan, Ann Arbor</span></dd></div>
      <div><dt>July 2018</dt><dd><strong>BS in Mechanical Engineering</strong><span>Shanghai Jiao Tong University, China · UM–SJTU Joint Institute</span></dd></div>
      <div><dt>Fall 2017</dt><dd><strong>Exchange semester</strong><span>Technical University of Munich, Germany</span></dd></div>
    </dl>
  </section>
</div>
