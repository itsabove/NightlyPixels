---
layout: default
title: "Gallery"
full_width: true
body_class: wide-post
---

<h1 align="center"><b>Reviews</b></h1>
<h4 align="center"><b>A critical look at the latest games</b></h4>
<br>

<div class="two-columns-left-wide">

  <!-- ========================================== -->
  <!-- COLUMN 1: MAIN POSTS FEED (LEFT)           -->
  <!-- ========================================== -->
  <div class="left-column">

    
    <div class="image-grid-3">
     <img src="/assets/img/photo1.jpg" alt="Image 1">
     <img src="/assets/img/photo2.jpg" alt="Image 2">
     <img src="/assets/img/photo3.jpg" alt="Image 3">
    </div>
        </div>

      </div>

  </div>
  <!-- COLUMN 1 END -->


  <!-- ========================================== -->
  <!-- COLUMN 2: SIDEBAR / TABLE OF CONTENTS      -->
  <!-- ========================================== -->
  <div class="right-column">
    <div class="sidebar-box">
      <h3 style="margin-top: 0; color: #5E787D; border-bottom: 2px solid #1FBCF0; padding-bottom: 6px;">Table of Contents</h3>
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
  </div>
  <!-- COLUMN 2 END -->

</div>



    <div class="image-grid-3">
     <img src="/assets/img/photo1.jpg" alt="Image 1">
     <img src="/assets/img/photo2.jpg" alt="Image 2">
     <img src="/assets/img/photo3.jpg" alt="Image 3">
    </div>

