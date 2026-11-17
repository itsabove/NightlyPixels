---
layout: default
---

<h1 align="center"><b>Reviews</b></h1>
<h4 align="center"><b>A critical look at the latest games</b></h4>
<br>

***

<div class="sidebar-box" style="text-align: center;">
  <h3 style="margin-top: 0; color: #5E787D; border-bottom: 2px solid #1FBCF0; padding-bottom: 6px;">Table of Contents</h3>
  <ul style="list-style: none; list-style-type: none; padding-left: 0; margin: 0;">
    {% assign count = 0 %}
    {% for post in articles %}
      {% assign tags_lower = post.tags | join: "," | downcase %}
      {% assign cats_lower = post.categories | join: "," | downcase %}
      {% if tags_lower contains "review" or cats_lower contains "review" %}
        <li style="list-style: none; background: none; padding-left: 0; margin-bottom: 12px; padding-bottom: 10px; border-bottom: 1px solid #eee;">
          <a href="{{ post.url | relative_url }}" style="color: #5E787D; font-weight: bold; text-decoration: none; display: block; line-height: 1.3;">
            {{ post.title }}
          </a>
        </li>
        {% assign count = count | plus: 1 %}
        {% if count == 10 %}{% break %}{% endif %}
      {% endif %}
    {% endfor %}
  </ul>
</div>
