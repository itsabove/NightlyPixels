---
layout: default
title: "Nightly Pixel"
full_width: true
body_class: wide-post
---

<!-- Hero Section for Latest Post -->
{% assign latest_post = site.posts.first %}
<div class="hero-latest-post" style="border: 1px solid #ddd; padding: 20px; margin-bottom: 30px; background: #f9f9f9;">
  
  <!-- Custom Image: Change 'height: 250px' to your preferred size -->
  <img src="{{ '/assets/images/my-custom-hero.jpg' | relative_url }}" 
       alt="Latest Post Banner" 
       style="width: 100%; height: 250px; object-fit: cover; margin-bottom: 15px;">

  <h2>Latest Post: <a href="{{ latest_post.url | relative_url }}">{{ latest_post.title }}</a></h2>
  <p><small>Published on {{ latest_post.date | date: "%B %d, %Y" }}</small></p>
  <p>{{ latest_post.excerpt }}</p>
  <a href="{{ latest_post.url | relative_url }}" class="btn">Read More &rarr;</a>
</div>

<!-- Rest of your normal index content follows below -->

<div class="two-columns-left-wide">
  <div>
    <div style="display: flex; align-items: center; gap: 15px;">
  <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" style="flex-shrink: 0;">
    <img src="assets/images/res.png" alt="Description" style="width: 150px; height: auto; display: block;" />
  </a>
  <div>
    <p style="font-size: 15px; font-weight: normal; margin: 0 0 4px 0;">
      <a href="https://nightlypixel.com/pages/Reviews.html" style="color: #1FBCF0; text-decoration: none;">Reviews</a>
    </p>
    <p style="font-size: 20px; font-weight: 900; margin: 0 0 8px 0; line-height: 1.2;">
      <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" style="color: #5E787D; text-decoration: none;">Resonance: A Plague Tale Legacy Review</a>
    </p>   
     <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">November 11,2026</p>
    <p style="margin: 0;">Plague Tale wasn't for me, but a game without rats? That's something I can get into.</p>
  </div>
</div>
  </div>
  <div>
    <h4>Table of contents</h4>
    <a href="/2026/11/12/resonance-review.html" style="color: #363636;">Resonance: A Plague Tale Legacy</a>
  </div>
</div>


<div style="display: flex; align-items: center; gap: 15px;">
  <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" style="flex-shrink: 0;">
    <img src="assets/images/res.png" alt="Description" style="width: 150px; height: auto; display: block;" />
  </a>
  <div>
    <p style="font-size: 15px; font-weight: normal; margin: 0 0 4px 0;">
      <a href="https://nightlypixel.com/pages/Reviews.html" style="color: #1FBCF0; text-decoration: none;">Reviews</a>
    </p>
    <p style="font-size: 20px; font-weight: 900; margin: 0 0 8px 0; line-height: 1.2;">
      <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" style="color: #5E787D; text-decoration: none;">Resonance: A Plague Tale Legacy Review</a>
    </p>   
     <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">November 11,2026</p>
    <p style="margin: 0;">Plague Tale wasn't for me, but a game without rats? That's something I can get into.</p>
  </div>
</div>

