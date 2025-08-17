---
layout: archive
title: "Conferences"
permalink: /conferences/
author_profile: true
---

<script>
  const link = document.getElementById("download-link");
  link.addEventListener("click", function(e) {
    fetch(link.href, { method: "HEAD" }).then(resp => {
      if (!resp.ok) {
        e.preventDefault();
        window.location.href = "/404.html";
      }
    });
  });
</script>


{% include base_path %}


## Conferences
<div class="coming-soon" style="
     border: 2px dashed #ccc;
     background-color: #fff8e1;
     padding: 20px;
     text-align: center;
     border-radius: 10px;
     margin-bottom: 20px;
     font-weight: bold;
     font-size: 1.2em;
     color: #555;">
  🚀 Coming Soon!
</div>

<!-- 
## Workshop
<div class="coming-soon" style="
     border: 2px dashed #ccc;
     background-color: #fff8e1;
     padding: 20px;
     text-align: center;
     border-radius: 10px;
     margin-bottom: 20px;
     font-weight: bold;
     font-size: 1.2em;
     color: #555;">
  🚀 Coming Soon!
</div>
-->

## Summer School
{% for post in site.conferences reversed %}
<div class="conference-box" style="
     border: 1px solid #ccc;
     padding: 12px;
     margin-bottom: 12px;
     border-radius: 8px;
     background-color: #f9f9f9;">
  
  <h3 style="margin: 0 0 6px 0;">{{ post.title }}</h3>
  
  {% if post.start_date and post.end_date %}
  <p style="margin: 0;"><strong>Dates:</strong> {{ post.start_date | date: "%b %-d, %Y" }} – {{ post.end_date | date: "%b %-d, %Y" }}</p>
  {% elsif post.start_date %}
  <p style="margin: 0;"><strong>Date:</strong> {{ post.start_date | date: "%b %-d, %Y" }}</p>
  {% endif %}
  
  {% if post.venue %}
  <p style="margin: 0;"><strong>Venue:</strong> {{ post.venue }}</p>
  {% endif %}
  
  {% if post.location %}
  <p style="margin: 0;"><strong>Location:</strong> {{ post.location }}</p>
  {% endif %}
  
  {% if post.certificate %}
  <p style="margin:6px 0;">
    <a href="{{ '/files/' | append: post.certificate }}"
        style="display:inline-block; padding:6px 12px; background-color:#007acc; color:white; text-decoration:none; border-radius:6px; font-weight:bold; font-size:0.9em;">
    📄 Download Certificate (PDF)
    </a>
  </p>
  {% endif %}
  
</div>
{% endfor %}