---
layout: glassy
title: The Infinity Blog
permalink: /blog/
---

# 📝 The Infinity Blog

Welcome to the heart of our insights — where spiritual energy meets digital design.  
We share behind-the-scenes drops, app updates, and conscious tech philosophies.

<ul style="list-style: none; padding: 0;">
  {% for post in site.posts %}
    <li style="margin-bottom: 2rem; padding: 1.5rem; border-radius: 12px; background: rgba(255, 255, 255, 0.5); backdrop-filter: blur(8px); box-shadow: 0 4px 12px rgba(0,0,0,0.08);">
      <a href="{{ post.url }}" style="text-decoration: none; font-size: 1.25rem; color: #7a3e9d; font-weight: 600;">
        {{ post.title }}
      </a><br>
      <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }}</small><br><br>
      <p style="color: #444; margin: 0;">{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </li>
  {% endfor %}
</ul>
