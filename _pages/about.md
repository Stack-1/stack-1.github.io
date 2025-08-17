---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

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



# General Information

I am a **PhD student** at the [Department of Civil and Computer Engineering](https://dicii.uniroma2.it/) (DICII) at the [University of Rome “Tor Vergata”](https://web.uniroma2.it/).

My research focuses on **High-Performance Computing (HPC)** and **scientific computing**, with a strong emphasis on designing and implementing **numerical methods and algorithms for solving linear systems on GPU accelerators**.

I am particularly engaged in developing and optimizing **parallel numerical linear algebra techniques**. My main research interests include:

- Iterative methods for sparse and dense linear systems  
- Krylov subspace algorithms and advanced preconditioning strategies  
- GPU-accelerated Sparse Matrix–Vector Multiplication (SpMV) kernels  
- High-throughput solvers for large-scale scientific simulations  

---

# Current Porjects
This is a collection of the projects I'm currently working on:
- HPC cluster emulation in order to use MPI on single board chipsets
- ACM TACO paper result reproducibility of [gHyPart](https://github.com/HiPeac-TorVergata/gHyPart_TACO) according to the [HiPEAC](https://www.hipeac.net/news/7068/students-hone-your-research-skills-at-hipeac-2025/)
- Testing parallel sparse BLAS routines on [PSBLAS](https://github.com/sfilippone/psblas3/tree/test_dev)
- Binary sparse matri-vector multiplication (SpMV) on GPU

---


<div class="cv-section" style="display: flex; gap: 2em; flex-wrap: wrap;">

  <div class="cv-box" style="flex: 1; min-width: 300px;">
    <h3>University Office</h3>
    <p>
      Department of Civil and Computer Engineering <br>
      University of Rome “Tor Vergata” <br>
      Information Engineering Building <br>
      1st Floor, Building D <br>
      Via del Politecnico 1, 00133 Rome, Italy
    </p>
  </div>

  <div class="cv-box" style="flex: 1; min-width: 300px;">
    <h3>Company Office</h3>
    <p>
      IT-Systems s.r.l.<br>
      Campo Romano Shopping Center <br>
      2nd Floor <br>
      Via Frascineto 8, 00133 Rome, Italy
    </p>
  </div>

</div>