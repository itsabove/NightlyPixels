---
layout: default
title: "Nightly Pixel"
full_width: true
body_class: wide-post
---

<!-- Hero Section for Latest Post in a Subfolder -->
{% assign latest_post = site.posts.first %}
<div class="hero-banner" style="position: relative; margin-bottom: 30px; width: 100%; height: 300px; overflow: hidden;">
  <a href="/article/forever-ago-review.html" title="Read {{ latest_post.title }}" style="display: block; width: 100%; height: 100%; text-decoration: none;">
    
    <img src="/assets/images/post/forever-ago/FA_01.webp" 
         alt="Hero Banner" 
         style="width: 100%; height: 100%; object-fit: cover; object-position: center 50%; display: block;">

    <!-- Custom Text Overlay -->
    <div style="position: absolute; inset: 0; background: linear-gradient(to top, rgba(0,0,0,0.75) 0%, rgba(0,0,0,0.15) 60%, transparent 100%); display: flex; flex-direction: column; justify-content: flex-end; padding: 20px; box-sizing: border-box;">
      <h1 style="color: #ffffff; margin: 0; font-size: 24px; line-height: 1.2; text-shadow: 1px 1px 3px rgba(0,0,0,0.8);">Forever Ago Review</h1>
    </div>

  </a>
</div>
<!-- Rest of your normal index content follows below -->

<!-- ========================================== -->
<!-- Page Starts Under Here           -->
<!-- ========================================== -->

<div class="two-columns-left-wide">

  <!-- ========================================== -->
  <!-- COLUMN 1: MAIN POSTS FEED (LEFT)           -->
  <!-- ========================================== -->
  <div class="left-column">

    {% assign raw_articles = site.pages | where_exp: "item", "item.path contains 'article/'" | sort: "date" | reverse %}
    {% assign articles = "" | split: "" %}
    {% for item in raw_articles %}
      {% unless item.name == "index.html" or item.name == "index.md" %}
        {% assign articles = articles | push: item %}
      {% endunless %}
    {% endfor %}
    
    {% for post in articles limit: 10 %}
      <div class="post-entry">
        
        <!-- Post Card (Thumbnail + Summary) -->
        <div class="post-card">
          <a href="{{ post.url | relative_url }}" class="post-card-image">
            <img src="{{ post.image }}" alt="{{ post.image_alt | default: post.title }}" />
          </a>
          <div class="post-card-text">
            <p style="font-size: 15px; font-weight: normal; margin: 0 0 4px 0;">
              <a href="{{ post.category_url }}" style="color: #1aa499; text-decoration: none;">{{ post.category }}</a>
            </p>
            <p style="font-size: 20px; font-weight: 900; margin: 0 0 8px 0; line-height: 1.2;">
              <a href="{{ post.url | relative_url }}" style="color: #5E787D; text-decoration: none;">{{ post.title }}</a>
            </p>   
            <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">{{ post.date | date: "%B %-d, %Y" }}</p>
            <p style="margin: 0;">{{ post.summary }}</p>
          </div>
        </div>

        <br>

        <!-- Author Info & Divider -->
        <div class="post-author">
          <div style="display: flex; align-items: center; gap: 15px;">
            <img src="{{ post.author_image | default: 'https://imgix.net' }}" alt="{{ post.author | default: 'Jose Balderas' }}" style="width: 50px; height: auto; display: block; flex-shrink: 0;" />
            <div>
              <p style="margin: 0;"><b>{{ post.author | default: "Jose Balderas" }}</b></p>
              <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">{{ post.gamertag | default: "GT: II Above II" }}</p>
            </div>    
          </div> 
          <hr>
        </div>

      </div>
    {% endfor %}

  </div>
  <!-- COLUMN 1 END -->


  <!-- ========================================== -->
  <!-- COLUMN 2: SIDEBAR / TABLE OF CONTENTS      -->
  <!-- ========================================== -->
  <div class="right-column">
    <div class="sidebar-box">
      <h3 style="margin-top: 0; color: #5E787D; border-bottom: 2px solid #1aa499; padding-bottom: 6px;">Table of Contents</h3>
      <ul style="list-style: none; list-style-type: none; padding-left: 0; margin: 0;">
        {% for post in articles limit: 10 %}
          <li style="list-style: none; background: none; padding-left: 0; margin-bottom: 12px; padding-bottom: 10px; border-bottom: 1px solid #eee;">
            <a href="{{ post.url | relative_url }}" style="color: #5E787D; font-weight: bold; text-decoration: none; display: block; line-height: 1.3;">
              {{ post.title }}
            </a>
          </li>
        {% endfor %}
      </ul>
    </div>
     <h3 style="margin-top: 0; color: #5E787D; border-bottom: 2px solid #1aa499; padding-bottom: 6px;">List</h3>
       <li style="list-style: none; background: none; padding-left: 0; margin-bottom: 12px; padding-bottom: 10px; border-bottom: 1px solid #eee;">
            <a href="blank" style="color: #5E787D; font-weight: bold; text-decoration: none; display: block; line-height: 1.3;">List coming soon</a>
       </li>
  </div>
  <!-- COLUMN 2 END -->

</div>


