---
layout: archive
title: 
permalink: /fake_research/
author_profile: true
---
<!-- Malware Analysis Paragraph-->
<span style="color:#AB9278;font-weight:700;font-size:38px"> Malware Analysis </span>


<div style="display: flex; align-items: flex-start; gap: 20px;">
  <div style="width: 15%; min-width: 12.5rem;">
    <img id="thumbnail" src="/images/Malware_Analysis.png" alt="Malware Analysis"
         style="width: 100%; height: auto; max-width: 150px; cursor: pointer;">
  </div>

  <div style="width: 72%;">
    <h4 class="m_8a5d1357 mantine-Title-root"
        style="--title-fw:var(--mantine-h4-font-weight); --title-lh:var(--mantine-h4-line-height); --title-fz:var(--mantine-h4-font-size);"
        data-order="4">
      Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring
    </h4>
    <p class="mantine-focus-auto m_b6d8b162 mantine-Text-root">
      Po-Kai Chen, Bo-Wei Tsai, Shao Kuan Wei, Chien-Yao Wang, Jia-Ching Wang, and Yi-Ting Huang
    </p>
    <p class="mantine-focus-auto m_b6d8b162 mantine-Text-root">
      To appear in Proceedings of the Annual Meeting of the Association for Computational Linguistics (ACL), 2025.
    </p>
  </div>
</div>

<!-- Modal for enlarged image -->
<div id="imageModal"
     style="display: none; position: fixed; z-index: 999; padding-top: 60px; left: 0; top: 0; width: 100vw; height: 100vh; overflow: auto; background-color: rgba(0,0,0,0.8);">
  <span id="closeModal"
        style="position: absolute; top: 30px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;">&times;</span>
  <img id="modalImage" style="margin: auto; display: block; max-width: 90%; max-height: 80%;">
</div>

<script>
  const modal = document.getElementById("imageModal");
  const modalImg = document.getElementById("modalImage");
  const thumbnail = document.getElementById("thumbnail");
  const closeModal = document.getElementById("closeModal");

  thumbnail.onclick = function () {
    modal.style.display = "block";
    modalImg.src = this.src;
  }

  closeModal.onclick = function () {
    modal.style.display = "none";
  }

  window.onclick = function (event) {
    if (event.target === modal) {
      modal.style.display = "none";
    }
  }
</script>

