---
layout: archive
title: 
permalink: /fake_research/
author_profile: true
---

<!-- 第一個區塊 -->
<div style="display: flex; align-items: flex-start; gap: 20px; flex-wrap: wrap; background:#FDF8F5; padding: 20px; margin-bottom: 20px;">
  <div style="width: 40%; min-width: 300px; display: flex; align-items: center; justify-content: center;">
    <img id="thumbnail1" src="/images/Malware_Analysis.png"
         alt="Malware Analysis"
         style="width: 100%; height: auto; cursor: pointer; max-width: 100%; border-radius: 8px;">
  </div>
  <div style="flex: 1; min-width: 250px; background:#FDF8F5; padding: 20px; border-radius: 12px;">
    <h2 style="font-weight: bold;">
      Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring
    </h2>
    <p>Po-Kai Chen, Bo-Wei Tsai, Shao Kuan Wei, Chien-Yao Wang, Jia-Ching Wang, and Yi-Ting Huang</p>
    <p>To appear in Proceedings of the Annual Meeting of the Association for Computational Linguistics (ACL), 2025.</p>
    <div style="display: flex; gap: 12px; margin-top: 10px;">
      <!-- PDF 按鈕 -->
      <a href="https://example.com/your-paper.pdf" target="_blank"
         style="display: inline-block; background: #f4eeff; padding: 10px 16px; border-radius: 12px;">
        <img src="https://cdn-icons-png.flaticon.com/512/337/337946.png" alt="PDF" width="24">
      </a>
      <!-- Dataset 按鈕 -->
      <a href="https://example.com/your-dataset" target="_blank"
         style="display: inline-block; background: #f4eeff; padding: 10px 16px; border-radius: 12px;">
        <img src="https://cdn-icons-png.flaticon.com/512/4228/4228783.png" alt="Dataset" width="24">
      </a>
      <!-- Website 按鈕 -->
      <a href="https://example.com/project-site" target="_blank"
         style="display: inline-block; background: #f4eeff; padding: 10px 16px; border-radius: 12px;">
        <img width="30" height="30" src="https://img.icons8.com/external-wanicon-lineal-color-wanicon/30/external-link-user-interface-wanicon-lineal-color-wanicon.png" alt="LINK"/>
      </a>
    </div>
  </div>
</div>

<!-- 第二個區塊 -->
<div style="display: flex; align-items: flex-start; gap: 20px; flex-wrap: wrap; background:#FDF8F5; padding: 20px;">
  <div style="width: 25%; min-width: 300px;">
    <img id="thumbnail2" src="/images/Malware_Analysis.png"
         alt="Malware Analysis 2"
         style="width: 100%; height: auto; cursor: pointer;">
  </div>
  <div style="flex: 1; min-width: 250px; background:#FDF8F5; padding: 20px; border-radius: 12px;">
    <h2 style="font-weight: bold;">
      Another Research Title Placeholder
    </h2>
    <p>Author A, Author B, Author C</p>
    <p>To appear in IEEE Transactions on Example Research, 2025.</p>
    <div style="display: flex; gap: 12px; margin-top: 10px;">
      <!-- PDF 按鈕 -->
      <a href="https://example.com/your-paper.pdf" target="_blank"
         style="display: inline-block; background: #f4eeff; padding: 10px 16px; border-radius: 12px;">
        <img src="https://cdn-icons-png.flaticon.com/512/337/337946.png" alt="PDF" width="24">
      </a>
      <!-- Dataset 按鈕 -->
      <a href="https://example.com/your-dataset" target="_blank"
         style="display: inline-block; background: #f4eeff; padding: 10px 16px; border-radius: 12px;">
        <img src="https://cdn-icons-png.flaticon.com/512/4228/4228783.png" alt="Dataset" width="24">
      </a>
      <!-- Website 按鈕 -->
      <a href="https://example.com/project-site" target="_blank"
         style="display: inline-block; background: #f4eeff; padding: 10px 16px; border-radius: 12px;">
        <img width="30" height="30" src="https://img.icons8.com/external-wanicon-lineal-color-wanicon/30/external-link-user-interface-wanicon-lineal-color-wanicon.png" alt="LINK"/>
      </a>
    </div>
  </div>
</div>


<div id="modal1" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.8); z-index:9999; justify-content:center; align-items:center;">
  <span onclick="document.getElementById('modal1').style.display='none'"
        style="position:absolute; top:20px; right:30px; font-size:36px; color:white; cursor:pointer;">&times;</span>
  <img id="modalImage1" style="max-width:90%; max-height:90%; border-radius:10px;">
</div>

<script>
  document.getElementById("thumbnail1").onclick = function () {
    document.getElementById("modalImage1").src = this.src;
    document.getElementById("modal1").style.display = "flex";
  };
</script>
