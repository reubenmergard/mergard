---
layout: default
title: Home
---

<header class="site-header">
  <div class="site-title">Reuben Mergard</div>
</header>

<div class="home-layout">

  <main class="home-main">
    {% for post in site.posts limit:20 %}
      <div class="post-item">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <div class="post-meta">{{ post.date | date: "%d %b %Y" }}</div>
      </div>
    {% endfor %}
  </main>

  <div class="home-side">
    <div class="side-note">
      <p>Clarity is a design discipline.</p>
    </div>

    <div class="side-links">
      <a href="/about/">About</a><br>
      <a href="/now/">Now</a><br>
      <a href="/contact/">Contact</a>
    </div>
  </div>

</div>