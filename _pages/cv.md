---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<head>
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
  <link rel="stylesheet" href="/assets/css/cv.css">

</head>



<section class="cv-section">
  <h2>💼 Work Experience</h2>

  <div class="cv-box">
    <h3>Software Engineer</h3>
    <p><strong>Duration:</strong> 2024 - Present</p>
    <p><strong>Company:</strong> IT-Systems s.r.l.</p>
    <p><strong>Role / Responsibilities:</strong> Develop and optimize HPC solutions on GPU architectures, implement linear algebra algorithms, and support scientific computing workflows.</p>
    <p><strong>Type:</strong> Full Time</p>
  </div>

  <div class="cv-box">
    <h3>Software Engineer</h3>
    <p><strong>Duration:</strong> 2022 - 2024</p>
    <p><strong>Company:</strong> IT-Systems s.r.l.</p>
    <p><strong>Role / Responsibilities:</strong> Full-stack web development projects and independent cybersecurity tasks.</p>
    <p><strong>Type:</strong> Part Time</p>
  </div>

  <div class="cv-box">
    <h3>Teaching Tutor</h3>
    <p><strong>Duration:</strong> 2022 - 2023</p>
    <p><strong>Company:</strong> Tor Vergata University</p>
    <p><strong>Role / Responsibilities:</strong> Conducted lessons, guided hands-on exercises, and provided lab support to students.</p>
    <p><strong>Type:</strong> Part Time</p>
  </div>
</section>

<section class="cv-section">
  <h2>🎓 Education</h2>

  <div class="cv-box">
    <h3>Ph.D. in Computer Science, Control and GeoInformation</h3>
    <p><strong>University:</strong> Tor Vergata University, Rome</p>
    <p><strong>Duration:</strong> 2024 - In Progress</p>
  </div>

  <div class="cv-box">
    <h3>M.S. in System and Software Engineering</h3>
    <p><strong>University:</strong> Tor Vergata University, Rome</p>
    <p><strong>Mark:</strong> 110/110 cum laude</p>
    <p><strong>Duration:</strong> 2022 - 2024</p>
    <p>
      <strong>Thesis:</strong> “Mixed-precision algorithms for linear systems on GPU accelerators”  
    </p>
    <p style="margin:6px 0;">
      <a href="{{ '/files/msc_thesis.pdf' | relative_url }}"
          style="display:inline-block; padding:6px 12px; background-color:#007acc; color:white; text-decoration:none; border-radius:6px; font-weight:bold; font-size:0.9em;">
      📄 Download Thesis (PDF)
      </a>
    </p>
  </div>

  <div class="cv-box">
    <h3>B.S. in Computer Engineering</h3>
    <p><strong>University:</strong> Tor Vergata University, Rome</p>
    <p><strong>Mark:</strong> 110/110 cum laude</p>
    <p><strong>Duration:</strong> 2019 - 2021</p>
  </div>
</section>