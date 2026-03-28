---
layout: default
title: Home
---

<div class="home-layout">
  <main class="home-main">

    <div class="site-bio">
      <p><a href="/" class="site-name">Reuben Mergard</a> knows a bit about branding, a smidge about making things, a lot about thinking about making things, and hardly anything about tax returns — except that his is probably late. Self-employed. Needs a better boss. Enjoys the arrangement of words. Editing less so. Spends a lot of time imagining things in the spatial-conceptual realm: energy flowing, forms assembling, light bending around invisible forces. Shoots medium format film. Obsessed with organisation as a hobby he never has time for. Thinks a lot about how creative people can do more with what they've got. Not much of a surfer, but you can't catch a wave before you get in the water. Not in the habit of writing about himself in the third person. For those who make.</p>
    </div>

    <div class="post-list">
      {% for post in site.posts limit:20 %}
      <div class="post-item">
        <div class="post-title-meta">
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="post-meta">{{ post.date | date: "%d %b %Y" }}</span>
        </div>
      </div>
      {% endfor %}
    </div>

  </main>

  <div class="home-side">
    <div class="side-links">
      <a href="/now/">Now</a><br>
      <a href="/contact/">Contact</a>
    </div>
  </div>
</div>
