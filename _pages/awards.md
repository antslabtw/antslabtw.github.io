---
layout: archive
title: ""
permalink: /awards/
author_profile: true
---

<!-- 留這一行空白，避免 <style> 被當成程式碼 -->

<style>
  :root{
    --green:#5CB85C;
    --text:#111827;
    --muted:#6b7280;
    --line:#e5e7eb;
    --card-bg:#ffffff;
    --card-border:#e5e7eb;
  }

  /* ====== SLIDER ====== */
  .hero-slider{
    position:relative;
    width:100%;
    height: min(55vh, 520px);
    border-radius: 12px;
    overflow:hidden;
    box-shadow: 0 8px 24px rgba(0,0,0,.08);
    margin-bottom: 1.75rem;
    background:#f3f4f6;
  }
  .hs-slide{
    position:absolute; inset:0;
    opacity:0; transition:opacity .6s ease;
  }
  .hs-slide.active{ opacity:1; }
  .hs-slide img{
    width:100%; height:100%; object-fit:cover; display:block;
  }
  .hs-caption{
    position:absolute; left:0; right:0; bottom:0;
    padding: .9rem 1.1rem;
    color:#fff;
    background: linear-gradient(0deg, rgba(0,0,0,.55), rgba(0,0,0,0));
  }
  .hs-title{ font-weight:700; font-size:1.05rem; }
  .hs-sub{ font-size:.9rem; opacity:.9; }

  .hs-dots{
    position:absolute; bottom:10px; left:50%; transform:translateX(-50%);
    display:flex; gap:.4rem; align-items:center;
  }
  .hs-dot{
    width:10px; height:10px; border-radius:9999px;
    background: rgba(255,255,255,.7); cursor:pointer;
    border: 2px solid rgba(0,0,0,.1);
  }
  .hs-dot.active{ background:#fff; }

  /* ====== TIMELINE ====== */
  .timeline{
    position:relative;
    padding-left:0;
    margin-top: 1.5rem;
  }
  /* 中央垂直線（在日期與內容之間） */
  .timeline::before{
    content:"";
    position:absolute;
    left: 160px; /* 與日期欄寬對齊 */
    top:0; bottom:0;
    width:2px; background: var(--line);
  }

  /* 年份收合區塊 */
  .tl-year{
    margin: 1rem 0 1.2rem 0;
    border:1px solid var(--card-border);
    border-radius:10px;
    background:#fff;
    overflow:hidden;
  }
  .tl-year summary{
    list-style:none; cursor:pointer;
    padding: .8rem 1rem;
    font-weight:700; color:var(--text);
    background:#f9fafb;
    position:relative;
  }
  .tl-year summary::-webkit-details-marker{ display:none; }
  .tl-year summary .meta{
    color: var(--muted); font-weight: 500; margin-left:.4rem; font-size:.95rem;
  }
  .tl-year[open] summary{ border-bottom:1px solid var(--card-border); }

  /* 條目 */
  .tl-items{ padding: .5rem .75rem 1rem .75rem; }
  .tl-item{
    position:relative;
    display:grid; grid-template-columns: 160px 1fr; gap: 18px;
    padding: 14px 6px;
  }
  .tl-item:not(:last-child){ border-bottom:1px dashed var(--line); }

  /* 節點（圓點） */
  .tl-item::before{
    content:"";
    position:absolute; left: 160px; top: 28px;
    transform: translate(-50%, -50%);
    width:12px; height:12px; border-radius:50%;
    background: var(--green); box-shadow: 0 0 0 3px #e8f7ec;
  }

  /* 日期徽章 */
  .tl-date{
    text-align:right; padding-right:18px;
    color:var(--muted);
    font-weight:700; white-space:nowrap;
  }
  .date-badge{
    display:inline-block; padding:2px 6px; border-radius:4px;
    background: var(--green); color:#fff; font-weight:700; font-size:12px;
  }

  /* 內容卡片 */
  .tl-card{
    background: var(--card-bg);
    border:1px solid var(--card-border);
    border-radius:10px;
    padding: 12px 14px;
  }
  .tl-card a{ color:#0ea5e9; text-decoration:none; }
  .tl-card a:hover{ text-decoration:underline; }

  /* 行動版調整 */
  @media (max-width: 720px){
    .timeline::before{ display:none; }
    .tl-item{ grid-template-columns: 1fr; }
    .tl-item::before{ display:none; }
    .tl-date{ text-align:left; padding:0 0 6px 0; }
  }
</style>

<!-- ========== SLIDER ========== -->
<div class="hero-slider" id="hero-slider" aria-label="Awards hero slider">
  <div class="hs-slide active" data-index="0">
    <img src="/images/NTUST_bachlorcomp-1.png" alt="ACL 2025 acceptance">
    <div class="hs-caption">
      <div class="hs-title">電機系最佳專題競賽｜第五名</div>
      <div class="hs-sub">113學年度｜指導：黃意婷｜專題生：陳柔尹、蔡宗嶧、廖冠語</div>
    </div>
  </div>
  <div class="hs-slide" data-index="1">
    <img src="/images/NICS-1_tmp.jpg" alt="Honorable Mention — Cyber Range & Attack/Defense Scripts Challenge">
    <div class="hs-caption">
      <div class="hs-title">資安演練場域與攻防腳本徵件｜佳作</div>
      <div class="hs-sub">113年度｜指導：黃意婷｜學生：楊明翊、林妍汝、沈婉瑛、余仲恩、王新元</div>
    </div>
  </div>
</div>

<!-- ========== TIMELINE（年份可收合，預設全展開） ========== -->
<div class="timeline">

  <!-- 2025 -->
  <details class="tl-year" open>
    <summary>
      <!-- 小箭頭 icon（可提示可展開/收起） -->
      <svg class="chev" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
        <path d="M6 6l8 4-8 4V6z"/>
      </svg>
      2025 
    </summary>
    <div class="tl-items">

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jul. 2025</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導專題生黃文良錄取大專學生研究計畫
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jun. 2025</span></div>
        <div class="tl-card">
          Congratulations! Our paper "<i>Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring</i>" has been accepted in ACL2025.
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jun. 2025</span></div>
        <div class="tl-card">
          Congratulations! Our paper "<i>A Cascade Approach for APT Campaign Attribution in System Event Logs: Technique Hunting and Subgraph Matching</i>" has been accepted in ICC2025.
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Feb. 2025</span></div>
        <div class="tl-card">
          黃意婷老師指導碩士生楊明翊、林妍汝、沈婉瑛、余仲恩、王新元榮獲
          <a href="/images/NICS.pdf">113年度建置資安演練場域及攻擊/防禦腳本徵件活動</a>佳作
        </div>
      </div>

    </div>
  </details>

  <!-- 2024 -->
  <details class="tl-year" open>
    <summary>
      <svg class="chev" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
        <path d="M6 6l8 4-8 4V6z"/>
      </svg>
      2024 
    </summary>
    <div class="tl-items">

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Dec. 2024</span></div>
        <div class="tl-card">
          黃意婷老師指導專題生陳柔尹、蔡宗嶧、廖冠語榮獲 
          <a href="/images/NTUST_bachlorcomp.pdf">113學年度電機工程系最佳專題競賽</a>第五名
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Oct. 2024</span></div>
        <div class="tl-card">
          Congratulations! Our paper has been selected to receive 
          <a href="/images/TANET.png">Best Paper Awards of TANET 2024</a>
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jul. 2024</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導專題生陳柔尹錄取大專學生研究計畫
        </div>
      </div>

    </div>
  </details>

  <!-- 2023 -->
  <details class="tl-year" open>
    <summary>
      <svg class="chev" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
        <path d="M6 6l8 4-8 4V6z"/>
      </svg>
      2023 
    </summary>
    <div class="tl-items">

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">May 2023</span></div>
        <div class="tl-card">
          Prof. Yi-Ting Huang will give a talk at Indo-Taiwan Workshop in Jammu, India. Come to say hi!
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jan. 2023</span></div>
        <div class="tl-card">
          Congratulations! Our paper has been selected to receive 
          <a href="https://jise.iis.sinica.edu.tw/pages/jise/index.html#Announcements" target="_blank" rel="noopener">the annual best paper award of 2022 by JISE</a>.
        </div>
      </div>

    </div>
  </details>

  <!-- 2022 -->
  <details class="tl-year" open>
    <summary>
      <svg class="chev" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
        <path d="M6 6l8 4-8 4V6z"/>
      </svg>
      2022 
    </summary>
    <div class="tl-items">

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Dec. 2022</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導碩士生陳羿琪錄取台電公司111學年度研究所獎學金甄選
        </div>
      </div>

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Sep. 2022</span></div>
        <div class="tl-card">
          Prof. Yi-Ting Huang will give a talk at 
          <a href="https://cyber.ithome.com.tw/2022/speaker-page/473" target="_blank" rel="noopener">CYBERSEC2022</a>. Come to say hi!
        </div>
      </div>

    </div>
  </details>

</div>

<script>
  // ===== Hero Slider：更健壯的自動播放（setTimeout 鏈結＋visibility 保護） =====
  (function(){
    const slider = document.getElementById('hero-slider');
    if(!slider) return;
    const slides = slider.querySelectorAll('.hs-slide');
    const dots = slider.querySelectorAll('.hs-dot');
    const interval = parseInt(slider.getAttribute('data-interval') || '5000', 10);
    let idx = 0;
    let timerId = null;

    function activate(n){
      slides[idx].classList.remove('active');
      dots[idx].classList.remove('active');
      idx = (n + slides.length) % slides.length;
      slides[idx].classList.add('active');
      dots[idx].classList.add('active');
    }

    function next(){ activate(idx + 1); }

    function schedule(){
      clear();
      // 若頁面不可見，先不排程，等回到可見時再啟動
      if (document.hidden) return;
      timerId = setTimeout(()=>{ next(); schedule(); }, interval);
    }

    function clear(){
      if (timerId){ clearTimeout(timerId); timerId = null; }
    }

    // 點擊圓點
    dots.forEach(d=>{
      d.addEventListener('click', ()=>{
        activate(parseInt(d.dataset.go,10));
        schedule();
      });
    });

    // 滑鼠暫停 / 離開繼續
    slider.addEventListener('mouseenter', clear);
    slider.addEventListener('mouseleave', schedule);

    // 切換分頁可見性時控制播放
    document.addEventListener('visibilitychange', ()=>{
      if (document.hidden) { clear(); }
      else { schedule(); }
    });

    // 首次排程
    schedule();
  })();
</script>
