---
layout: default
title: "Nightly Pixel"
full_width: true
body_class: wide-post
---

<!-- Hero Section for Latest Post -->

{% assign latest_post = site.posts.first %}
<div class="hero-banner" style="position: relative; margin-bottom: 30px; width: 100%; height: 250px; overflow: hidden;">
  <a href="{{ latest_post.url | relative_url }}" title="Read {{ latest_post.title }}" style="display: block; width: 100%; height: 100%; text-decoration: none;">
    
    <img src="https://6af7a66789893ca61a9aff38.imgix.net/008.png" 
         alt="Hero Banner" 
         style="width: 100%; height: 100%; object-fit: cover; object-position: center 20%; display: block;">

    <!-- Custom Text Overlay -->
    <div style="position: absolute; inset: 0; background: linear-gradient(to top, rgba(0,0,0,0.75) 0%, rgba(0,0,0,0.15) 60%, transparent 100%); display: flex; flex-direction: column; justify-content: flex-end; padding: 20px; box-sizing: border-box;">
      <h2 style="color: #ffffff; margin: 0; font-size: 24px; line-height: 1.2; text-shadow: 1px 1px 3px rgba(0,0,0,0.8);">No Rats? Sounds Like A Game For Me</h2>
    </div>

  </a>
</div>

<!-- Rest of your normal index content follows below -->

<div class="two-columns-left-wide">
  <!-- COLUMN 1: Automatic Post Feed (Limited to 5) -->
  <div>
    {% for post in site.posts limit:5 %}
      <div class="post-card">
        <a href="{{ post.url | relative_url }}" class="post-card-image">
          <img src="{{ post.image }}" alt="{{ post.title }}" />
        </a>
        <div class="post-card-text">
          <p style="font-size: 15px; font-weight: normal; margin: 0 0 4px 0;">
            <a href="{{ '/pages/' | append: post.category | append: '.html' | relative_url }}" style="color: #1FBCF0; text-decoration: none;">
              {{ post.category }}
            </a>
          </p>
          <p style="font-size: 20px; font-weight: 900; margin: 0 0 8px 0; line-height: 1.2;">
            <a href="{{ post.url | relative_url }}" style="color: #5E787D; text-decoration: none;">
              {{ post.title }}
            </a>
          </p>   
          <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">
            {{ post.date | date: "%B %-d, %Y" }}
          </p>
          <p style="margin: 0;">{{ post.description }}</p>
        </div>
      </div>    
      
      <br>
      
      <!-- Row 2: Author Image & Info -->
      <div>
        <div style="display: flex; align-items: center; gap: 15px;">
          <img src="{{ post.author_image | default: 'https://imgix.net' }}" alt="{{ post.author | default: 'Jose Balderas' }}" style="width: 50px; height: auto; display: block; flex-shrink: 0;" />
          <div>
            <p style="margin: 0;"><b>{{ post.author | default: "Jose Balderas" }}</b></p>
            <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">
              {{ post.gamertag | default: "GT: II Above II" }}
            </p>
          </div>    
        </div> 
        <hr>
      </div>
    {% endfor %}
  </div>

  <!-- COLUMN 2: Automatic Table of Contents (Limited to 5) -->
  <div>
    <h4>Table of contents</h4>
    {% for post in site.posts limit:5 %}
      <p style="margin: 0 0 6px 0;">
        <a href="{{ post.url | relative_url }}" style="color: #363636;">{{ post.title }}</a>
      </p>
    {% endfor %}
  </div>
</div>

