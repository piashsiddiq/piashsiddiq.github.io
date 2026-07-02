---
title: "ECA"
permalink: /eca/
layout: default
author_profile: false
classes: wide
---

<div class="wrap" markdown="1">

<style>
  /* ====== Layout (same as Education/Skills) ====== */
  .page-grid{display:grid;grid-template-columns:260px 1fr;gap:28px;align-items:start;}
  @media(max-width:900px){.page-grid{grid-template-columns:1fr;}}

  /* ====== Author card ====== */
  .author-card{position:sticky;top:90px;border:1px solid #e5e7eb;border-radius:14px;padding:16px;background:#fff;}
  @media(max-width:900px){.author-card{position:static;}}
  .author-avatar{width:110px;height:110px;border-radius:999px;object-fit:cover;display:block;margin:0 auto 10px;}
  .author-name{text-align:center;font-weight:800;margin:0;}
  .author-bio{text-align:center;color:#6b7280;margin:6px 0 12px;font-size:.95rem;}
  .author-links{list-style:none;padding:0;margin:0;}
  .author-links li{margin:8px 0;}
  .author-links a{display:inline-flex;gap:8px;align-items:center;text-decoration:none;}

  /* ====== Page header card ====== */
  .eca-hero{
    border:1px solid #e5e7eb;
    border-radius:16px;
    padding:18px 18px;
    background: linear-gradient(180deg, rgba(243,244,246,.7), rgba(255,255,255,1));
    margin-bottom: 18px;
    position: relative;
    overflow: hidden;
  }
  .eca-hero:before{
    content:"";
    position:absolute;
    inset:-80px -120px auto auto;
    width:260px;height:260px;
    background: radial-gradient(circle, rgba(59,130,246,.18), rgba(59,130,246,0));
    filter: blur(2px);
    transform: rotate(18deg);
  }
  .eca-hero h2{margin:0 0 6px 0; position:relative;}
  .eca-hero p{margin:0;color:#6b7280; position:relative;}

  /* ====== Section card ====== */
  .eca-card{
    border:1px solid #e5e7eb;
    border-radius:16px;
    padding:16px 16px;
    background:#fff;
    margin: 16px 0;
  }
  .eca-title{
    display:flex;
    align-items:center;
    gap:10px;
    margin:0 0 10px 0;
  }
  .eca-title i{opacity:.9;}
  .muted{ color:#6b7280; }

  /* ====== Uncertain-info note (please confirm) ====== */
  .confirm-note{
    display:inline-block;
    border:1px dashed #f59e0b;
    background:#fffbeb;
    color:#b45309;
    border-radius:8px;
    padding:4px 9px;
    font-size:.82rem;
    font-weight:600;
  }

  /* ====== Fun badges ====== */
  .badges{display:flex;flex-wrap:wrap;gap:10px;margin:12px 0 0 0;}
  .badge{
    display:inline-flex;align-items:center;gap:8px;
    padding:8px 10px;border:1px solid #e5e7eb;border-radius:999px;
    background:#fff;color:#111827;font-size:.92rem;
  }

  /* ====== Gallery grid ====== */
  .gallery{
    display:grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap:12px;
  }
  @media(max-width:1100px){ .gallery{grid-template-columns: repeat(3, minmax(0, 1fr));} }
  @media(max-width:760px){  .gallery{grid-template-columns: repeat(2, minmax(0, 1fr));} }
  @media(max-width:420px){  .gallery{grid-template-columns: 1fr;} }

  .thumb{
    border:1px solid #e5e7eb;
    border-radius:14px;
    overflow:hidden;
    background:#fff;
    box-shadow: 0 10px 25px rgba(0,0,0,.06);
    position:relative;
  }
  .thumb:after{
    content:"";
    position:absolute;inset:0;
    background: linear-gradient(180deg, rgba(0,0,0,0), rgba(0,0,0,.22));
    opacity:0;
    transition:opacity .25s ease;
    pointer-events:none;
  }
  .thumb:hover:after{opacity:1;}
  .thumb img{
    width:100%;
    height:210px;
    object-fit:cover;
    display:block;
    transition: transform .25s ease;
  }
  .thumb:hover img{ transform: scale(1.03); }

  /* ====== Placeholder tile (for photos not yet added) ====== */
  .thumb-placeholder{
    border:2px dashed #cbd5e1;
    border-radius:14px;
    height:210px;
    background:#f8fafc;
    color:#94a3b8;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    gap:6px;
    font-size:.82rem;
    text-align:center;
    padding:10px;
  }
  .thumb-placeholder i{ font-size:26px; }

  /* ====== Lightbox ====== */
  .lb{
    position:fixed; inset:0;
    background:rgba(0,0,0,.85);
    display:none;
    align-items:center;
    justify-content:center;
    z-index:9999;
    padding:24px;
  }
  .lb.is-open{ display:flex; }

  .lb__img{
    max-width:min(1200px, 94vw);
    max-height:88vh;
    border-radius:14px;
    box-shadow:0 18px 50px rgba(0,0,0,.45);
    background:#111;
    object-fit:contain;
  }

  .lb__btn{
    position:absolute;
    top:18px;
    right:18px;
    width:42px;height:42px;
    border:0;
    border-radius:999px;
    background:rgba(255,255,255,.12);
    color:#fff;
    font-size:22px;
    cursor:pointer;
    display:flex;
    align-items:center;
    justify-content:center;
  }
  .lb__btn:hover{ background:rgba(255,255,255,.2); }

  .lb__nav{
    position:absolute;
    top:50%;
    transform:translateY(-50%);
    width:46px;height:46px;
    border:0;
    border-radius:999px;
    background:rgba(255,255,255,.12);
    color:#fff;
    font-size:28px;
    cursor:pointer;
    display:flex;
    align-items:center;
    justify-content:center;
  }
  .lb__nav:hover{ background:rgba(255,255,255,.2); }
  .lb__prev{ left:18px; }
  .lb__next{ right:18px; }

  @media (max-width:700px){
    .lb{ padding:14px; }
    .lb__prev{ left:10px; }
    .lb__next{ right:10px; }
  }

  /* ====== Subtle scroll reveal (fun) ====== */
  .reveal{opacity:0;transform:translateY(10px);transition:opacity .55s ease, transform .55s ease;}
  .reveal.is-in{opacity:1;transform:none;}
</style>

<div class="page-grid">

<!-- LEFT: Author profile (manual, same style as other pages) -->
<aside class="author-card">
  <img class="author-avatar" src="/assets/images/profile.jpg" alt="Abu Bakkar Siddiq">
  <p class="author-name">Abu Bakkar Siddiq</p>
  <p class="author-bio">MS Student, UT Dallas</p>
  <ul class="author-links">
    <li><a href="mailto:piashsiddiq@gmail.com"><i class="fas fa-envelope"></i>Email</a></li>
    <li><a href="https://github.com/piashsiddiq" target="_blank" rel="noopener"><i class="fab fa-github"></i>GitHub</a></li>
    <li><a href="https://www.linkedin.com/in/abu-siddiq-bakkar/" target="_blank" rel="noopener"><i class="fab fa-linkedin"></i>LinkedIn</a></li>
  </ul>
</aside>

<!-- RIGHT: Page content -->
<main markdown="1">

<div class="eca-hero reveal">
  <h2 class="eca-title"><i class="fas fa-people-group"></i> Extracurricular Activities</h2>
  <p>Human rights &amp; social welfare work, volunteering, professional student organizations, and sports activities beyond academics.</p>

  <div class="badges">
    <span class="badge"><i class="fas fa-scale-balanced"></i> Human Rights</span>
    <span class="badge"><i class="fas fa-hand-holding-heart"></i> Volunteering</span>
    <span class="badge"><i class="fas fa-people-group"></i> Professional Orgs</span>
    <span class="badge"><i class="fas fa-futbol"></i> Sports</span>
  </div>
</div>

<!-- ============ HUMAN RIGHTS & SOCIAL WELFARE ============ -->
<div class="eca-card reveal" markdown="1">
  <h3 class="eca-title"><i class="fas fa-scale-balanced"></i> Legal Aid Center Foundation — Human Rights &amp; Social Welfare</h3>
  <p class="muted" style="margin-top:0;">
    Served as <strong>Social Welfare Secretary</strong> (Feni South Region, Bangladesh) with the
    <strong>Legal Aid Center Foundation</strong> — a human rights and legal aid organization in
    Bangladesh, registered under the Societies Registration Act, 1860 (also registered as
    Ain Shohaota Kendra Foundation).
    <span class="confirm-note">⚠️ Please confirm exact years of service</span>
  </p>

  <!--
    TO ADD A PHOTO: replace one of the <div class="thumb-placeholder"> blocks below with:
    <a class="thumb" href="/assets/images/eca/legal-aid/1.jpg" data-lightbox="eca">
      <img src="/assets/images/eca/legal-aid/1.jpg" alt="Legal Aid Center activity">
    </a>
    (Just upload your image file to /assets/images/eca/legal-aid/ using that filename.)
  -->
  <div class="gallery">
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/legal-aid/1.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/legal-aid/2.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/legal-aid/3.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/legal-aid/4.jpg</div>
  </div>
</div>

<!-- ============ VOLUNTEERING ============ -->
<div class="eca-card reveal" markdown="1">
  <h3 class="eca-title"><i class="fas fa-hand-holding-heart"></i> Volunteering</h3>

  <p class="muted" style="margin-top:0;">
    <strong>MUNA</strong> — Muslim Ummah of North America &middot; Volunteer, 2025 &ndash; Present
  </p>
  <p class="muted" style="margin-top:0;">
    <strong>NAHAR</strong> — North American Humanitarian Aid &amp; Relief &middot; Volunteer, 2025 &ndash; Present
  </p>

  <!--
    TO ADD A PHOTO: replace a <div class="thumb-placeholder"> block below with:
    <a class="thumb" href="/assets/images/eca/volunteering/1.jpg" data-lightbox="eca">
      <img src="/assets/images/eca/volunteering/1.jpg" alt="Volunteering activity">
    </a>
  -->
  <div class="gallery">
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/volunteering/1.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/volunteering/2.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/volunteering/3.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/volunteering/4.jpg</div>
  </div>
</div>

<!-- ============ PROFESSIONAL STUDENT ORGANIZATIONS ============ -->
<div class="eca-card reveal" markdown="1">
  <h3 class="eca-title"><i class="fas fa-people-group"></i> Professional Student Organizations — UT Dallas</h3>

  <p class="muted" style="margin-top:0;">
    <strong>BALC</strong> — Business Analytics Leadership Committee, UT Dallas &middot; Active Member, 2025 &ndash; Present
  </p>
  <p class="muted" style="margin-top:0;">
    <strong>TAC</strong> — The Accounting Club, UT Dallas &middot; Active Member, 2025 &ndash; Present
  </p>

  <!--
    TO ADD A PHOTO: replace a <div class="thumb-placeholder"> block below with:
    <a class="thumb" href="/assets/images/eca/utd-orgs/1.jpg" data-lightbox="eca">
      <img src="/assets/images/eca/utd-orgs/1.jpg" alt="BALC or TAC activity">
    </a>
  -->
  <div class="gallery">
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/utd-orgs/1.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/utd-orgs/2.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/utd-orgs/3.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/utd-orgs/4.jpg</div>
  </div>
</div>

<!-- ============ SPORTS (Football & Cricket combined) ============ -->
<div class="eca-card reveal" markdown="1">
  <h3 class="eca-title"><i class="fas fa-futbol"></i> Sports — Football &amp; Cricket</h3>
  <p class="muted" style="margin-top:0;">
    I actively participate in football and cricket, including inter-institutional
    and community-level matches. I will keep adding photos here over time.
  </p>

  <!--
    TO ADD A PHOTO: replace a <div class="thumb-placeholder"> block below with:
    <a class="thumb" href="/assets/images/eca/sports/1.jpg" data-lightbox="eca">
      <img src="/assets/images/eca/sports/1.jpg" alt="Football or cricket activity">
    </a>
    (Football and cricket photos can both go in this same /assets/images/eca/sports/ folder.)
  -->
  <div class="gallery">
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/sports/1.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/sports/2.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/sports/3.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/sports/4.jpg</div>
    <div class="thumb-placeholder"><i class="fas fa-camera"></i>Add photo<br>/assets/images/eca/sports/5.jpg</div>
  </div>
</div>

<!-- Lightbox overlay (one per page) -->
<div class="lb" id="lightbox" aria-hidden="true">
  <button class="lb__btn" type="button" id="lbClose" aria-label="Close">✕</button>
  <button class="lb__nav lb__prev" type="button" id="lbPrev" aria-label="Previous">‹</button>
  <img class="lb__img" id="lbImg" alt="Expanded image">
  <button class="lb__nav lb__next" type="button" id="lbNext" aria-label="Next">›</button>
</div>

<script>
(function(){
  // ---- lightbox ----
  const lb = document.getElementById('lightbox');
  const lbImg = document.getElementById('lbImg');
  const btnClose = document.getElementById('lbClose');
  const btnPrev = document.getElementById('lbPrev');
  const btnNext = document.getElementById('lbNext');

  const links = Array.from(document.querySelectorAll('a[data-lightbox="eca"]'));
  let idx = -1;

  function openAt(i){
    if(!links.length) return;
    idx = (i + links.length) % links.length;
    const href = links[idx].getAttribute('href');
    lbImg.src = href;
    lb.classList.add('is-open');
    lb.setAttribute('aria-hidden','false');
    document.body.style.overflow = 'hidden';
  }
  function close(){
    lb.classList.remove('is-open');
    lb.setAttribute('aria-hidden','true');
    lbImg.src = '';
    document.body.style.overflow = '';
  }
  function next(){ openAt(idx + 1); }
  function prev(){ openAt(idx - 1); }

  links.forEach((a, i) => {
    a.addEventListener('click', (e) => {
      e.preventDefault();
      openAt(i);
    });
  });

  lb.addEventListener('click', (e) => {
    if(e.target === lb) close();
  });

  btnClose.addEventListener('click', close);
  btnNext.addEventListener('click', next);
  btnPrev.addEventListener('click', prev);

  document.addEventListener('keydown', (e) => {
    if(!lb.classList.contains('is-open')) return;
    if(e.key === 'Escape') close();
    if(e.key === 'ArrowRight') next();
    if(e.key === 'ArrowLeft') prev();
  });

  // ---- subtle scroll reveal ----
  const obs = new IntersectionObserver((entries) => {
    entries.forEach(en => {
      if(en.isIntersecting) en.target.classList.add('is-in');
    });
  }, { threshold: 0.08 });
  document.querySelectorAll('.reveal').forEach(el => obs.observe(el));
})();
</script>

</main>
</div>
</div>
