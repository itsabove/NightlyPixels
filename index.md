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

  <!-- ========================================== -->
  <!-- COLUMN 1: MAIN POSTS FEED (LEFT)           -->
  <!-- ========================================== -->
  <div class="left-column">

    <!-- ==================== POST 1 START ==================== -->
    <div class="post-entry">
      
      <!-- Post Card (Thumbnail + Summary) -->
      <div class="post-card">
        <a href="/article/whats-special-about-zelda" class="post-card-image">
          <img src="https://nightlypixel.imgix.net/nightlypixel/001.png" alt="Zelda fomo" />
        </a>
        <div class="post-card-text">
          <p style="font-size: 15px; font-weight: normal; margin: 0 0 4px 0;">
            <a href="https://nightlypixel.com/pages/Features.html" style="color: #1FBCF0; text-decoration: none;">Features</a>
          </p>
          <p style="font-size: 20px; font-weight: 900; margin: 0 0 8px 0; line-height: 1.2;">
            <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" style="color: #5E787D; text-decoration: none;">Resonance: A Plague Tale Legacy Review</a>
          </p>   
          <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">November 11, 2026</p>
          <p style="margin: 0;">Plague Tale wasn't for me, but a game without rats? That's something I can get into.</p>
        </div>
      </div>

      <br>

      <!-- Author Info & Divider -->
      <div class="post-author">
        <div style="display: flex; align-items: center; gap: 15px;">
          <img src="https://6af7a66789893ca61a9aff38.imgix.net/writer.png" alt="Jose Balderas" style="width: 50px; height: auto; display: block; flex-shrink: 0;" />
          <div>
            <p style="margin: 0;"><b>Jose Balderas</b></p>
            <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">GT: II Above II</p>
          </div>    
        </div> 
        <hr>
      </div>

    </div>
    <!-- ==================== POST 1 END ====================== -->


    <!-- ==================== POST 2 START ==================== -->
    <div class="post-entry">
      
      <!-- Post Card (Thumbnail + Summary) -->
      <div class="post-card">
        <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" class="post-card-image">
          <img src="https://6af7a66789893ca61a9aff38.imgix.net/r02.png" alt="Resonance: A Plague Tale Legacy" />
        </a>
        <div class="post-card-text">
          <p style="font-size: 15px; font-weight: normal; margin: 0 0 4px 0;">
            <a href="https://nightlypixel.com/pages/Reviews.html" style="color: #1FBCF0; text-decoration: none;">Reviews</a>
          </p>
          <p style="font-size: 20px; font-weight: 900; margin: 0 0 8px 0; line-height: 1.2;">
            <a href="https://nightlypixel.com/2026/11/12/resonance-review.html" style="color: #5E787D; text-decoration: none;">Resonance: A Plague Tale Legacy Review</a>
          </p>   
          <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">November 11, 2026</p>
          <p style="margin: 0;">Plague Tale wasn't for me, but a game without rats? That's something I can get into.</p>
        </div>
      </div>

      <br>

      <!-- Author Info & Divider -->
      <div class="post-author">
        <div style="display: flex; align-items: center; gap: 15px;">
          <img src="https://6af7a66789893ca61a9aff38.imgix.net/writer.png" alt="Jose Balderas" style="width: 50px; height: auto; display: block; flex-shrink: 0;" />
          <div>
            <p style="margin: 0;"><b>Jose Balderas</b></p>
            <p style="font-size: 10px; font-weight: 200; margin: 0 0 8px 0; line-height: 1.2;">GT: II Above II</p>
          </div>    
        </div> 
        <hr>
      </div>

    </div>
    <!-- ==================== POST 2 END ====================== -->



    <!-- ==================== POST 3 START ==================== -->
    <!-- NOTE: Paste Post 3 right below this line, BEFORE the closing </div> of the left-column -->

  </div> 
  <!-- END OF COLUMN 1 (LEFT) -->


  <!-- ========================================== -->
  <!-- COLUMN 2: SIDEBAR / TABLE OF CONTENTS      -->
  <!-- ========================================== -->
  <div class="right-column">
    <h4>Table of contents</h4>
    <p style="margin: 0 0 8px 0;">
      <a href="/2026/11/12/resonance-review.html" style="color: #363636;">Resonance: A Plague Tale Legacy</a>
    </p>
    <!-- NOTE: Add new sidebar links right below here -->
    <p style="margin: 0 0 8px 0;">
      <a href="LINK-TO-SECOND-POST" style="color: #363636;">Second Post Title</a>
    </p>
  </div>
  <!-- END OF COLUMN 2 (RIGHT) -->

</div>
