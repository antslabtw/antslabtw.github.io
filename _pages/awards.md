---
layout: archive
title: ""
permalink: /awards/
author_profile: true
---


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
    height: min(65vh, 680px);
    border-radius: 12px;
    overflow:hidden;
    box-shadow: 0 8px 24px rgba(0,0,0,.08);
    margin-bottom: 1.75rem;
    background:#f3f4f6;
  }
  .hs-slide{
    position:absolute; inset:0;
    opacity:0; transition:opacity .6s ease;
    display:none; /* 非 active 不顯示，避免重疊 */
  }
  .hs-slide.active{ opacity:1; display:block; }
  .hs-slide img{
    width:100%; height:100%; object-fit:cover; display:block;
  }
  .hs-slide{ z-index: 0; }    
  .hs-caption{ z-index: 1; }     
  .hs-nav{ z-index: 3; }
  .hs-dots{ z-index: 4; }  

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
    display:flex; gap:.4rem; align-items:center; z-index:2;
  }
  .hs-dot{
    width:10px; height:10px; border-radius:9999px;
    background: rgba(255,255,255,.7); cursor:pointer;
    border: 2px solid rgba(0,0,0,.1);
  }
  .hs-dot.active{ background:#fff; }

  .hs-nav{
    position:absolute; top:50%; transform:translateY(-50%);
    width:44px; height:44px; border-radius:50%;
    border:none; background:rgba(0,0,0,.35); color:#fff;
    display:flex; align-items:center; justify-content:center;
    cursor:pointer; z-index:2;
  }
  .hs-nav:hover{ background:rgba(0,0,0,.5); }
  .hs-nav svg{ width:20px; height:20px; }
  .hs-nav.prev{ left:10px; }
  .hs-nav.next{ right:10px; }

  /* ====== TIMELINE ====== */
  .timeline{
    position:relative;
    padding-left:0;
    margin-top: 1.5rem;
  }
  .timeline::before{
    content:"";
    position:absolute;
    left: 160px;
    top:0; bottom:0;
    width:2px; background: var(--line);
  }

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
  }
  .tl-year summary::-webkit-details-marker{ display:none; }
  .tl-year summary .meta{
    color: var(--muted); font-weight: 500; margin-left:.4rem; font-size:.95rem;
  }
  .tl-year[open] summary{ border-bottom:1px solid var(--card-border); }

  .tl-items{ padding: .5rem .75rem 1rem .75rem; }
  .tl-item{
    position:relative;
    display:grid; grid-template-columns: 160px 1fr; gap: 18px;
    padding: 14px 6px;
  }
  .tl-item:not(:last-child){ border-bottom:1px dashed var(--line); }

  .tl-item::before{
    content:"";
    position:absolute; left: 160px; top: 28px;
    transform: translate(-50%, -50%);
    width:12px; height:12px; border-radius:50%;
    background: var(--green); box-shadow: 0 0 0 3px #e8f7ec;
  }

  .tl-date{
    text-align:right; padding-right:18px;
    color:var(--muted);
    font-weight:700; white-space:nowrap;
  }
  .date-badge{
    display:inline-block; padding:2px 6px; border-radius:4px;
    background: var(--green); color:#fff; font-weight:700; font-size:12px;
  }

  .tl-card{
    background: var(--card-bg);
    border:1px solid var(--card-border);
    border-radius:10px;
    padding: 12px 14px;
  }
  .tl-card a{ color:#0ea5e9; text-decoration:none; }
  .tl-card a:hover{ text-decoration:underline; }

  @media (max-width: 720px){
    .timeline::before{ display:none; }
    .tl-item{ grid-template-columns: 1fr; }
    .tl-item::before{ display:none; }
    .tl-date{ text-align:left; padding:0 0 6px 0; }
  }
</style>

<!-- ========== SLIDER ========== -->
<div class="hero-slider" id="hero-slider" aria-label="Awards hero slider" data-interval="5000">
  <!-- slides -->
  <div class="hs-slide" data-index="0">
    <img src="/images/TANET_2025_excellent_paper_page.jpg" alt="TANET 2025 優秀論文獎">
    <div class="hs-caption">
      <div class="hs-title">視覺化系統事件日誌攻擊調查｜TANET 2025 優秀論文獎</div>
      <div class="hs-sub">114年｜指導：黃意婷｜學生：楊明翊</div>
    </div>
  </div>
  <div class="hs-slide active" data-index="1">
    <img src="/images/NTUST_bachlorcomp-1.png" alt="113學年度電機工程系最佳專題競賽 第五名">
    <div class="hs-caption">
      <div class="hs-title">電機系最佳專題競賽｜第五名</div>
      <div class="hs-sub">113學年度｜指導：黃意婷｜專題生：陳柔尹、蔡宗嶧、廖冠語</div>
    </div>
  </div>
  <div class="hs-slide" data-index="2">
    <img src="/images/NICS-1_tmp.jpg" alt="資安演練場域與攻防腳本徵件 佳作">
    <div class="hs-caption">
      <div class="hs-title">資安演練場域與攻防腳本徵件｜佳作</div>
      <div class="hs-sub">113年度｜指導：黃意婷｜學生：楊明翊、林妍汝、沈婉瑛、余仲恩、王新元</div>
    </div>
  </div>

  <!-- 左右按鈕 -->
  <button class="hs-nav prev" type="button" aria-label="Previous slide">
    <svg viewBox="0 0 20 20" fill="currentColor"><path d="M12.5 4l-6 6 6 6"/></svg>
  </button>
  <button class="hs-nav next" type="button" aria-label="Next slide">
    <svg viewBox="0 0 20 20" fill="currentColor"><path d="M7.5 4l6 6-6 6"/></svg>
  </button>

  <!-- dots（JS 會自動產生） -->
  <div class="hs-dots" id="hs-dots" role="tablist" aria-label="Slider dots"></div>
</div>

<!-- ========== TIMELINE（年份可收合，預設全展開） ========== -->
<div class="timeline">

  <!-- 2025 -->
  <details class="tl-year" open>
    <summary>2025</summary>
    <div class="tl-items">
      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Dec. 2025</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導專題生陳敬橋、黃文良、胡承學榮獲114學年度電機工程系最佳專題競賽第一名
        </div>
      </div>
      
      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Oct. 2025</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導碩士生楊明翊榮獲<a href="/images/TANET_2025_excellent_paper.pdf"> TANET 2025 臺灣網際網路研討會 優秀論文獎 </a>
        </div>
      </div>
      
      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Aug. 2025</span></div>
        <div class="tl-card">
          Congratulations! <a href="https://www.ee.ntust.edu.tw/p/406-1027-138440,r490.php">黃意婷老師榮獲113學年度教學優良獎</a>
        </div>
      </div>
      
      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jul. 2025</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導專題生黃文良錄取大專學生研究計畫
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
    <summary>2024</summary>
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

  <!-- 2023
  
  <details class="tl-year" open>
    <summary>2023</summary>
    <div class="tl-items">

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Jan. 2023</span></div>
        <div class="tl-card">
          Congratulations! Our paper has been selected to receive 
          <a href="https://jise.iis.sinica.edu.tw/pages/jise/index.html#Announcements" target="_blank" rel="noopener">the annual best paper award of 2022 by JISE</a>.
        </div>
      </div>

    </div>
  </details>
  
  -->

  <!-- 2022 -->
  <details class="tl-year" open>
    <summary>2022</summary>
    <div class="tl-items">

      <div class="tl-item">
        <div class="tl-date"><span class="date-badge">Dec. 2022</span></div>
        <div class="tl-card">
          Congratulations! 黃意婷老師指導碩士生陳羿琪錄取台電公司111學年度研究所獎學金甄選
        </div>
      </div>

    </div>
  </details>

</div>

<script>
(function(){
  const slider = document.getElementById('hero-slider');
  if (!slider) return;

  const slides = slider.querySelectorAll('.hs-slide');
  const dotsWrap = document.getElementById('hs-dots');
  const interval = parseInt(slider.getAttribute('data-interval') || '5000', 10);
  let idx = 0;
  let timerId = null;

  /* 動態產生 dots */
  if (dotsWrap) {
    slides.forEach(function(_, i){
      const b = document.createElement('button');
      b.className = 'hs-dot' + (i === 0 ? ' active' : '');
      b.setAttribute('aria-label', 'Slide ' + (i+1));
      b.dataset.go = i;
      dotsWrap.appendChild(b);
    });
  }
  let dots = dotsWrap ? dotsWrap.querySelectorAll('.hs-dot') : [];

  function activate(n){
    slides[idx].classList.remove('active');
    if (dots[idx]) dots[idx].classList.remove('active');
    idx = (n + slides.length) % slides.length;
    slides[idx].classList.add('active');
    if (dots[idx]) dots[idx].classList.add('active');
  }

  function next(){ activate(idx + 1); }
  function prev(){ activate(idx - 1); }

  function schedule(){
    clear();
    if (document.hidden) return;
    timerId = setTimeout(function(){ next(); schedule(); }, interval);
  }
  function clear(){
    if (timerId){ clearTimeout(timerId); timerId = null; }
  }

  /* 事件委派：點擊 dots */
  if (dotsWrap) {
    dotsWrap.addEventListener('click', function(e){
      const btn = e.target.closest('.hs-dot');
      if (!btn) return;
      const go = parseInt(btn.dataset.go, 10);
      activate(go);
      schedule();
    });
  }

  /* 左右按鈕 */
  const btnPrev = slider.querySelector('.hs-nav.prev');
  const btnNext = slider.querySelector('.hs-nav.next');
  if (btnPrev) btnPrev.addEventListener('click', function(){ prev(); schedule(); });
  if (btnNext) btnNext.addEventListener('click', function(){ next(); schedule(); });

  /* 滑鼠暫停 / 離開繼續 */
  slider.addEventListener('mouseenter', clear);
  slider.addEventListener('mouseleave', schedule);

  /* 分頁可見性切換 */
  document.addEventListener('visibilitychange', function(){
    if (document.hidden) { clear(); }
    else { schedule(); }
  });

  schedule();
})();
</script>


