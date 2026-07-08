<!DOCTYPE html>
<html lang="ur" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AH Calligraphy | عربی و اردو خطاطی کا فن</title>
<meta name="description" content="AH Calligraphy — عربی اور اردو خطاطی، حسبِ ضرورت نام، اسلامی آرٹ اور دنیا بھر میں ترسیل۔">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Nastaliq+Urdu:wght@400;600;700&family=Aref+Ruqaa:wght@400;700&family=Noto+Sans+Arabic:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --navy-deep:#071527;
    --navy:#0B2038;
    --navy-soft:#122c4a;
    --gold:#C9A227;
    --gold-light:#E8C766;
    --gold-dim:#8B7B4E;
    --cream:#F3ECD8;
    --cream-dim:#cfc6a9;
    --max-w:1180px;
  }

  *{margin:0;padding:0;box-sizing:border-box;}

  html{scroll-behavior:smooth;}

  body{
    background:var(--navy-deep);
    color:var(--cream);
    font-family:'Noto Nastaliq Urdu','Noto Sans Arabic',serif;
    line-height:2;
    overflow-x:hidden;
  }

  @media (prefers-reduced-motion: reduce){
    html{scroll-behavior:auto;}
    *{animation-duration:0.01ms !important; animation-iteration-count:1 !important; transition-duration:0.01ms !important;}
  }

  a{color:inherit;text-decoration:none;}
  ul{list-style:none;}
  img{max-width:100%;display:block;}
  section{position:relative;}

  ::selection{background:var(--gold);color:var(--navy-deep);}

  :focus-visible{
    outline:2px solid var(--gold-light);
    outline-offset:3px;
  }

  .wrap{max-width:var(--max-w);margin:0 auto;padding:0 28px;}

  .eyebrow{
    font-family:'Aref Ruqaa',serif;
    color:var(--gold);
    letter-spacing:2px;
    font-size:1.05rem;
    display:inline-block;
    margin-bottom:10px;
    position:relative;
    padding-inline-start:38px;
  }
  .eyebrow::before{
    content:"";
    position:absolute;
    right:0;
    top:50%;
    transform:translateY(-50%);
    width:28px;
    height:1px;
    background:var(--gold);
  }

  h1,h2,h3{font-family:'Aref Ruqaa',serif;font-weight:700;color:var(--cream);}

  /* ===== Islamic geometric pattern background ===== */
  .pattern-bg{
    position:absolute;
    inset:0;
    opacity:0.08;
    pointer-events:none;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='84' height='84' viewBox='0 0 84 84'%3E%3Cg fill='none' stroke='%23C9A227' stroke-width='1'%3E%3Cpath d='M42 2 L62 22 L42 42 L22 22 Z'/%3E%3Cpath d='M42 42 L62 62 L42 82 L22 62 Z'/%3E%3Cpath d='M2 42 L22 22 L42 42 L22 62 Z'/%3E%3Cpath d='M42 42 L62 22 L82 42 L62 62 Z'/%3E%3Ccircle cx='42' cy='42' r='6'/%3E%3C/g%3E%3C/svg%3E");
    background-size:84px 84px;
  }

  .divider{
    width:100%;
    height:22px;
    background-repeat:repeat-x;
    background-position:center;
    background-size:44px 22px;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='44' height='22' viewBox='0 0 44 22'%3E%3Cpath d='M0 22 L11 0 L22 22 L33 0 L44 22' fill='none' stroke='%23C9A227' stroke-width='1.2'/%3E%3C/svg%3E");
    opacity:.55;
  }

  /* ===== Header / Nav ===== */
  header{
    position:fixed;
    top:0;
    right:0;
    left:0;
    z-index:100;
    background:rgba(7,21,39,0.85);
    backdrop-filter:blur(10px);
    border-bottom:1px solid rgba(201,162,39,0.25);
    transition:background .3s ease;
  }
  .nav-inner{
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:14px 28px;
    max-width:var(--max-w);
    margin:0 auto;
  }
  .logo{
    font-family:'Aref Ruqaa',serif;
    font-size:1.6rem;
    color:var(--gold-light);
    letter-spacing:1px;
    display:flex;
    align-items:center;
    gap:10px;
  }
  .logo span.mark{
    display:inline-block;
    width:14px;height:14px;
    border:2px solid var(--gold);
    transform:rotate(45deg);
  }
  nav.links{display:flex;gap:34px;font-size:1.05rem;}
  nav.links a{
    position:relative;
    color:var(--cream-dim);
    transition:color .25s ease;
    padding:4px 2px;
  }
  nav.links a::after{
    content:"";
    position:absolute;
    bottom:-2px;right:0;left:0;
    height:1px;
    background:var(--gold);
    transform:scaleX(0);
    transform-origin:right;
    transition:transform .3s ease;
  }
  nav.links a:hover,
  nav.links a.active{color:var(--gold-light);}
  nav.links a:hover::after,
  nav.links a.active::after{transform:scaleX(1);}

  .burger{
    display:none;
    flex-direction:column;
    gap:5px;
    background:none;
    border:none;
    cursor:pointer;
    padding:8px;
  }
  .burger span{
    width:24px;height:2px;background:var(--gold);
    transition:transform .3s ease, opacity .3s ease;
  }

  /* ===== Hero ===== */
  .hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:140px 24px 80px;
    background:
      radial-gradient(ellipse at 50% 0%, rgba(201,162,39,0.14), transparent 60%),
      linear-gradient(180deg, var(--navy-deep) 0%, var(--navy) 55%, var(--navy-deep) 100%);
  }
  .hero-inner{position:relative;z-index:2;max-width:780px;}
  .hero .eyebrow{padding-inline-start:0;}
  .hero .eyebrow::before{display:none;}
  .hero h1{
    font-size:clamp(2.6rem, 7vw, 4.6rem);
    line-height:1.25;
    margin:6px 0 4px;
  }
  .hero h1 .en{
    display:block;
    font-family:'Aref Ruqaa',serif;
    font-size:clamp(1.6rem, 4vw, 2.4rem);
    color:var(--gold-light);
    letter-spacing:3px;
    margin-top:10px;
  }

  /* signature stroke */
  .stroke-wrap{margin:26px auto 22px;width:min(420px,80vw);}
  .stroke-wrap svg{width:100%;height:auto;overflow:visible;}
  .stroke-wrap path{
    fill:none;
    stroke:var(--gold);
    stroke-width:2.5;
    stroke-linecap:round;
    stroke-dasharray:900;
    stroke-dashoffset:900;
    animation:draw 2.4s ease-out .3s forwards;
  }
  @keyframes draw{to{stroke-dashoffset:0;}}

  .hero p.tagline{
    font-size:1.25rem;
    color:var(--cream-dim);
    max-width:560px;
    margin:0 auto 34px;
  }

  .btn-row{display:flex;gap:18px;justify-content:center;flex-wrap:wrap;}

  .btn{
    display:inline-flex;
    align-items:center;
    gap:10px;
    padding:14px 30px;
    border-radius:2px;
    font-size:1.05rem;
    font-family:'Noto Nastaliq Urdu',serif;
    transition:transform .25s ease, box-shadow .25s ease, background .25s ease;
    border:1px solid var(--gold);
  }
  .btn-primary{
    background:linear-gradient(135deg, var(--gold-light), var(--gold));
    color:var(--navy-deep);
    font-weight:700;
  }
  .btn-primary:hover{transform:translateY(-3px);box-shadow:0 10px 26px rgba(201,162,39,0.35);}
  .btn-outline{
    background:transparent;
    color:var(--gold-light);
  }
  .btn-outline:hover{background:rgba(201,162,39,0.12);transform:translateY(-3px);}
  .btn svg{width:20px;height:20px;flex-shrink:0;}

  /* ===== Reveal on scroll ===== */
  .reveal{opacity:0;transform:translateY(28px);transition:opacity .8s ease, transform .8s ease;}
  .reveal.show{opacity:1;transform:translateY(0);}

  /* ===== Section shell ===== */
  .section{padding:100px 0;}
  .section-head{text-align:center;max-width:640px;margin:0 auto 56px;}
  .section-head h2{font-size:clamp(2rem,4.5vw,2.8rem);}
  .section-head p{color:var(--cream-dim);font-size:1.08rem;margin-top:10px;}
  .section.alt{background:var(--navy);}

  /* ===== About strip ===== */
  .about{
    max-width:760px;
    margin:0 auto;
    text-align:center;
    padding:70px 24px 20px;
  }
  .about p{font-size:1.15rem;color:var(--cream-dim);}

  /* ===== Gallery ===== */
  .gallery-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:22px;
  }
  .art-card{
    position:relative;
    aspect-ratio:1/1;
    border:1px solid rgba(201,162,39,0.35);
    background:linear-gradient(155deg, var(--navy-soft), var(--navy-deep));
    overflow:hidden;
    cursor:pointer;
  }
  .art-card img{
    width:100%;height:100%;object-fit:cover;
    transition:transform .5s ease;
  }
  .art-card:hover img{transform:scale(1.08);}
  .art-card .placeholder{
    width:100%;height:100%;
    display:flex;align-items:center;justify-content:center;
    font-family:'Aref Ruqaa',serif;
    font-size:3rem;
    color:rgba(201,162,39,0.5);
  }
  .art-card .corner{
    position:absolute;width:16px;height:16px;
    border:1px solid var(--gold);
    opacity:.8;
  }
  .art-card .corner.tl{top:8px;right:8px;border-left:none;border-bottom:none;}
  .art-card .corner.br{bottom:8px;left:8px;border-right:none;border-top:none;}
  .art-card .cap{
    position:absolute;bottom:0;right:0;left:0;
    padding:10px 12px;
    background:linear-gradient(0deg, rgba(7,21,39,0.9), transparent);
    font-size:.95rem;
    color:var(--cream);
    opacity:0;
    transform:translateY(8px);
    transition:opacity .3s ease, transform .3s ease;
  }
  .art-card:hover .cap{opacity:1;transform:translateY(0);}

  .gallery-note{
    text-align:center;
    margin-top:34px;
    color:var(--cream-dim);
    font-size:.98rem;
  }

  /* Lightbox */
  .lightbox{
    position:fixed;inset:0;z-index:200;
    background:rgba(4,10,20,0.94);
    display:flex;align-items:center;justify-content:center;
    opacity:0;pointer-events:none;
    transition:opacity .3s ease;
    padding:24px;
  }
  .lightbox.open{opacity:1;pointer-events:auto;}
  .lightbox-inner{max-width:min(720px,92vw);text-align:center;}
  .lightbox img,.lightbox .placeholder{width:100%;border:1px solid var(--gold);}
  .lightbox .placeholder{
    aspect-ratio:1/1;background:var(--navy-soft);
    display:flex;align-items:center;justify-content:center;
    font-family:'Aref Ruqaa',serif;font-size:4rem;color:var(--gold-dim);
  }
  .lightbox-close{
    margin-top:18px;color:var(--gold-light);
    border:1px solid var(--gold);padding:8px 22px;
    display:inline-block;cursor:pointer;background:none;font-family:inherit;font-size:1rem;
  }

  /* ===== Services ===== */
  .services-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:24px;
  }
  .service-card{
    background:var(--navy-deep);
    border:1px solid rgba(201,162,39,0.28);
    padding:36px 26px;
    text-align:center;
    transition:transform .3s ease, border-color .3s ease;
  }
  .service-card:hover{transform:translateY(-6px);border-color:var(--gold);}
  .service-icon{
    width:56px;height:56px;margin:0 auto 20px;
    color:var(--gold);
  }
  .service-icon svg{width:100%;height:100%;}
  .service-card h3{font-size:1.35rem;margin-bottom:10px;color:var(--gold-light);}
  .service-card p{color:var(--cream-dim);font-size:.98rem;}

  /* ===== Order steps ===== */
  .steps{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:36px;
    counter-reset:step;
  }
  .step{position:relative;text-align:center;padding:0 12px;}
  .step .num{
    font-family:'Aref Ruqaa',serif;
    font-size:3.2rem;
    color:transparent;
    -webkit-text-stroke:1.4px var(--gold);
    margin-bottom:14px;
  }
  .step h3{font-size:1.25rem;color:var(--cream);margin-bottom:8px;}
  .step p{color:var(--cream-dim);font-size:.98rem;}
  .step:not(:last-child)::after{
    content:"";
    position:absolute;
    top:28px;
    left:-18px;
    width:36px;height:1px;
    background:linear-gradient(90deg,var(--gold),transparent);
    display:none;
  }
  @media(min-width:769px){
    .step:not(:last-child)::after{display:block;}
  }

  /* ===== Contact ===== */
  .contact-box{
    max-width:640px;margin:0 auto;
    text-align:center;
    background:linear-gradient(155deg, var(--navy-soft), var(--navy-deep));
    border:1px solid rgba(201,162,39,0.35);
    padding:60px 34px;
    position:relative;
  }
  .contact-box::before,
  .contact-box::after{
    content:"";position:absolute;width:26px;height:26px;
    border:1px solid var(--gold);
  }
  .contact-box::before{top:14px;right:14px;border-left:none;border-bottom:none;}
  .contact-box::after{bottom:14px;left:14px;border-right:none;border-top:none;}
  .contact-box p.msg{color:var(--cream-dim);margin-bottom:30px;font-size:1.1rem;}
  .social-row{
    display:flex;justify-content:center;gap:20px;margin-top:36px;
  }
  .social-row a{
    width:48px;height:48px;
    border:1px solid var(--gold);
    display:flex;align-items:center;justify-content:center;
    color:var(--gold-light);
    transition:background .25s ease, transform .25s ease;
  }
  .social-row a:hover{background:rgba(201,162,39,0.15);transform:translateY(-4px);}
  .social-row svg{width:22px;height:22px;}

  /* ===== Footer ===== */
  footer{
    padding:34px 24px;
    text-align:center;
    color:var(--gold-dim);
    font-size:.92rem;
    border-top:1px solid rgba(201,162,39,0.2);
  }
  footer a{color:var(--gold-light);}
  footer a:hover{text-decoration:underline;}

  /* ===== WhatsApp floating button ===== */
  .float-wa{
    position:fixed;
    bottom:24px;left:24px;
    z-index:150;
    width:58px;height:58px;
    background:var(--gold);
    color:var(--navy-deep);
    border-radius:50%;
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 8px 22px rgba(0,0,0,0.4);
    transition:transform .25s ease;
  }
  .float-wa:hover{transform:scale(1.08);}
  .float-wa svg{width:28px;height:28px;}

  /* ===== Responsive ===== */
  @media(max-width:900px){
    .gallery-grid{grid-template-columns:repeat(2,1fr);}
    .services-grid{grid-template-columns:repeat(2,1fr);}
    .steps{grid-template-columns:1fr;gap:44px;}
  }
  @media(max-width:768px){
    nav.links{
      position:fixed;
      top:64px;right:0;left:0;
      background:rgba(7,21,39,0.98);
      flex-direction:column;
      align-items:center;
      padding:26px 0;
      gap:22px;
      border-bottom:1px solid rgba(201,162,39,0.25);
      transform:translateY(-130%);
      opacity:0;
      transition:transform .35s ease, opacity .3s ease;
    }
    nav.links.open{transform:translateY(0);opacity:1;}
    .burger{display:flex;}
    .section{padding:70px 0;}
  }
  @media(max-width:560px){
    .gallery-grid{grid-template-columns:repeat(2,1fr);gap:14px;}
    .services-grid{grid-template-columns:1fr;}
    .hero{padding-top:120px;}
  }
</style>
</head>
<body>

<header>
  <div class="nav-inner">
    <a href="#home" class="logo"><span class="mark"></span> AH Calligraphy</a>
    <nav class="links" id="navLinks">
      <a href="#home" class="nav-link active">ہوم</a>
      <a href="#gallery" class="nav-link">گیلری</a>
      <a href="#services" class="nav-link">سروسز</a>
      <a href="#contact" class="nav-link">رابطہ</a>
    </nav>
    <button class="burger" id="burger" aria-label="مینو کھولیں" aria-expanded="false">
      <span></span><span></span><span></span>
    </button>
  </div>
</header>

<!-- ===================== HERO / HOME ===================== -->
<section class="hero" id="home">
  <div class="pattern-bg"></div>
  <div class="hero-inner">
    <span class="eyebrow">فنِ خطاطی</span>
    <h1>حروف کی روح، قلم کی زبان
      <span class="en">AH Calligraphy</span>
    </h1>

    <div class="stroke-wrap" aria-hidden="true">
      <svg viewBox="0 0 400 60">
        <path d="M10 30 C 80 5, 140 55, 200 30 S 320 5, 390 30"/>
      </svg>
    </div>

    <p class="tagline">عربی اور اردو خطاطی — ہر لفظ ایک تصویر، ہر تحریر ایک فن پارہ۔ آپ کے الفاظ کو دستِ ہنر سے فن میں ڈھالتے ہیں۔</p>

    <div class="btn-row">
      <a class="btn btn-primary" href="https://wa.me/966566454430?text=السلام عليكم، مجھے اپنی خطاطی کے بارے میں معلومات چاہئیں" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.6 6.32A7.85 7.85 0 0 0 12.02 4c-4.35 0-7.9 3.53-7.9 7.88 0 1.39.37 2.74 1.06 3.94L4 20l4.3-1.13a7.93 7.93 0 0 0 3.72.94h.01c4.35 0 7.9-3.53 7.9-7.88a7.8 7.8 0 0 0-2.33-5.6zm-5.58 12.1h-.01a6.6 6.6 0 0 1-3.36-.92l-.24-.14-2.5.65.67-2.43-.16-.25a6.53 6.53 0 0 1-1.01-3.48c0-3.62 2.96-6.57 6.62-6.57 1.77 0 3.43.69 4.68 1.94a6.5 6.5 0 0 1 1.94 4.64c0 3.62-2.96 6.56-6.63 6.56zm3.63-4.92c-.2-.1-1.17-.58-1.35-.64-.18-.07-.32-.1-.45.1-.13.2-.51.64-.63.77-.12.13-.23.15-.43.05-.2-.1-.85-.31-1.62-1-.6-.53-1-1.19-1.12-1.39-.12-.2-.01-.31.09-.4.09-.09.2-.24.3-.36.1-.12.13-.2.2-.34.07-.13.03-.25-.02-.35-.05-.1-.45-1.08-.61-1.48-.16-.39-.33-.34-.45-.34h-.38c-.13 0-.35.05-.53.25-.18.2-.7.68-.7 1.66 0 .98.72 1.93.82 2.06.1.13 1.4 2.14 3.4 3 .48.2.85.33 1.14.42.48.15.91.13 1.26.08.38-.06 1.17-.48 1.34-.94.16-.46.16-.86.11-.94-.05-.09-.18-.14-.38-.24z"/></svg>
        واٹس ایپ پر رابطہ کریں
      </a>
      <a class="btn btn-outline" href="#gallery">گیلری دیکھیں</a>
    </div>
  </div>
</section>

<div class="divider"></div>

<!-- ===================== ABOUT ===================== -->
<section class="about reveal">
  <p>AH Calligraphy ایک منفرد آرٹ پیج ہے جو عربی اور اردو خطاطی کے ذریعے حروف کو زندہ فن میں بدلتا ہے۔ ہر تحریر ہاتھ سے، محبت اور مہارت کے ساتھ تخلیق کی جاتی ہے — چاہے وہ آپ کا نام ہو یا کوئی مقدس آیت۔</p>
</section>

<!-- ===================== GALLERY ===================== -->
<section class="section" id="gallery">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="eyebrow">فن پارے</span>
      <h2>گیلری</h2>
      <p>ہمارے تخلیق کردہ کچھ نمونہ فن پارے — جلد ہی مزید تصاویر شامل کی جائیں گی۔</p>
    </div>

    <!--
      ==== تصاویر شامل کرنے کی ہدایت ====
      نیچے ہر .art-card کے اندر <div class="placeholder">...</div> کو
      <img src="آپ کی-تصویر-کا-پتہ.jpg" alt="تفصیل"> سے تبدیل کریں۔
      مثال:
      <div class="art-card" onclick="openLightbox(this)">
        <img src="images/artwork-1.jpg" alt="حسبِ ضرورت نام کی خطاطی">
        ...
      </div>
    -->
    <div class="gallery-grid">
      <div class="art-card reveal" onclick="openLightbox(this)" tabindex="0">
        <span class="corner tl"></span><span class="corner br"></span>
        <div class="placeholder">ا</div>
        <div class="cap">حسبِ ضرورت نام</div>
      </div>
      <div class="art-card reveal" onclick="openLightbox(this)" tabindex="0">
        <span class="corner tl"></span><span class="corner br"></span>
        <div class="placeholder">ب</div>
        <div class="cap">اسلامی آرٹ</div>
      </div>
      <div class="art-card reveal" onclick="openLightbox(this)" tabindex="0">
        <span class="corner tl"></span><span class="corner br"></span>
        <div class="placeholder">ج</div>
        <div class="cap">فریمڈ فن پارہ</div>
      </div>
      <div class="art-card reveal" onclick="openLightbox(this)" tabindex="0">
        <span class="corner tl"></span><span class="corner br"></span>
        <div class="placeholder">د</div>
        <div class="cap">اسمائے حسنیٰ</div>
      </div>
      <div class="art-card reveal" onclick="openLightbox(this)" tabindex="0">
        <span class="corner tl"></span><span class="corner br"></span>
        <div class="placeholder">ھ</div>
        <div class="cap">آیتِ قرآنی</div>
      </div>
      <div class="art-card reveal" onclick="openLightbox(this)" tabindex="0">
        <span class="corner tl"></span><span class="corner br"></span>
        <div class="placeholder">و</div>
        <div class="cap">جدید خطاطی</div>
      </div>
    </div>

    <p class="gallery-note">تصاویر شامل کرنے کے لیے کوڈ میں موجود ہدایات ملاحظہ کریں (art-card کمنٹ)۔</p>
  </div>
</section>

<div class="divider"></div>

<!-- ===================== SERVICES ===================== -->
<section class="section alt" id="services">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="eyebrow">ہماری خدمات</span>
      <h2>سروسز</h2>
      <p>ہر فن پارہ آپ کی پسند اور ضرورت کے مطابق تیار کیا جاتا ہے۔</p>
    </div>

    <div class="services-grid">
      <div class="service-card reveal">
        <div class="service-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M4 20l4-1 11-11-3-3L5 16l-1 4z"/><path d="M14 6l3 3"/></svg>
        </div>
        <h3>کسٹم ڈیزائن</h3>
        <p>آپ کا نام یا پسندیدہ جملہ منفرد خطاطی کے انداز میں تخلیق کیا جاتا ہے۔</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M12 3l3 6 6 1-4.5 4 1 6-5.5-3-5.5 3 1-6L3 10l6-1z"/></svg>
        </div>
        <h3>اسلامی آرٹ</h3>
        <p>قرآنی آیات، اسمائے حسنیٰ اور اسلامی طرز کے فن پاروں کی تخلیق۔</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="4" y="4" width="16" height="16"/><rect x="7.5" y="7.5" width="9" height="9"/></svg>
        </div>
        <h3>فریمنگ</h3>
        <p>آپ کے آرٹ ورک کو خوبصورت فریم میں محفوظ کیا جاتا ہے، دیوار کی زینت کے لیے تیار۔</p>
      </div>
      <div class="service-card reveal">
        <div class="service-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="12" cy="12" r="9"/><path d="M3 12h18M12 3c2.5 2.5 3.5 6 3.5 9s-1 6.5-3.5 9c-2.5-2.5-3.5-6-3.5-9s1-6.5 3.5-9z"/></svg>
        </div>
        <h3>عالمی ترسیل</h3>
        <p>دنیا بھر میں محفوظ اور تیز ترسیل کی سہولت فراہم کی جاتی ہے۔</p>
      </div>
    </div>
  </div>
</section>

<!-- ===================== ORDER STEPS ===================== -->
<section class="section" id="order">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="eyebrow">آسان طریقہ</span>
      <h2>آرڈر کیسے کریں</h2>
      <p>صرف تین مراحل میں اپنا خصوصی فن پارہ حاصل کریں۔</p>
    </div>
    <div class="steps">
      <div class="step reveal">
        <div class="num">١</div>
        <h3>رابطہ کریں</h3>
        <p>واٹس ایپ پر اپنا آئیڈیا، نام یا جملہ ہمیں بتائیں۔</p>
      </div>
      <div class="step reveal">
        <div class="num">٢</div>
        <h3>ڈیزائن کی منظوری</h3>
        <p>ہم نمونہ ڈیزائن تیار کر کے آپ کو دکھائیں گے اور آپ کی رائے شامل کریں گے۔</p>
      </div>
      <div class="step reveal">
        <div class="num">٣</div>
        <h3>تیاری اور ترسیل</h3>
        <p>حتمی فن پارہ تیار کر کے، فریم کے ساتھ یا بغیر، آپ تک محفوظ طریقے سے پہنچایا جائے گا۔</p>
      </div>
    </div>
  </div>
</section>

<div class="divider"></div>

<!-- ===================== CONTACT ===================== -->
<section class="section alt" id="contact">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="eyebrow">رابطہ</span>
      <h2>آئیے بات کرتے ہیں</h2>
    </div>

    <div class="contact-box reveal">
      <p class="msg">اپنی خطاطی کے آرڈر یا کسی بھی سوال کے لیے براہِ راست واٹس ایپ پر پیغام بھیجیں — ہم جلد جواب دیں گے۔</p>

      <a class="btn btn-primary" href="https://wa.me/966566454430?text=السلام عليكم، مجھے AH Calligraphy سے آرڈر کے بارے میں بات کرنی ہے" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.6 6.32A7.85 7.85 0 0 0 12.02 4c-4.35 0-7.9 3.53-7.9 7.88 0 1.39.37 2.74 1.06 3.94L4 20l4.3-1.13a7.93 7.93 0 0 0 3.72.94h.01c4.35 0 7.9-3.53 7.9-7.88a7.8 7.8 0 0 0-2.33-5.6zm-5.58 12.1h-.01a6.6 6.6 0 0 1-3.36-.92l-.24-.14-2.5.65.67-2.43-.16-.25a6.53 6.53 0 0 1-1.01-3.48c0-3.62 2.96-6.57 6.62-6.57 1.77 0 3.43.69 4.68 1.94a6.5 6.5 0 0 1 1.94 4.64c0 3.62-2.96 6.56-6.63 6.56z"/></svg>
        +966 56 645 4430
      </a>

      <div class="social-row">
        <a href="https://www.facebook.com/profile.php?id=61585383685038&mibextid=ZbWKwL" target="_blank" rel="noopener" aria-label="فیس بک پیج">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M13.5 21v-8h2.7l.4-3.1h-3.1V8c0-.9.25-1.5 1.55-1.5H16.7V3.7C16.4 3.66 15.4 3.57 14.2 3.57c-2.4 0-4.05 1.47-4.05 4.17V9.9H7.5V13h2.65v8h3.35z"/></svg>
        </a>
        <a href="https://wa.me/966566454430" target="_blank" rel="noopener" aria-label="واٹس ایپ">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.6 6.32A7.85 7.85 0 0 0 12.02 4c-4.35 0-7.9 3.53-7.9 7.88 0 1.39.37 2.74 1.06 3.94L4 20l4.3-1.13a7.93 7.93 0 0 0 3.72.94h.01c4.35 0 7.9-3.53 7.9-7.88a7.8 7.8 0 0 0-2.33-5.6zm-5.58 12.1h-.01a6.6 6.6 0 0 1-3.36-.92l-.24-.14-2.5.65.67-2.43-.16-.25a6.53 6.53 0 0 1-1.01-3.48c0-3.62 2.96-6.57 6.62-6.57 1.77 0 3.43.69 4.68 1.94a6.5 6.5 0 0 1 1.94 4.64c0 3.62-2.96 6.56-6.63 6.56z"/></svg>
        </a>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="divider" style="margin-bottom:22px;"></div>
  <p>&copy; <span id="year"></span> AH Calligraphy — تمام حقوق محفوظ ہیں | <a href="https://www.facebook.com/profile.php?id=61585383685038&mibextid=ZbWKwL" target="_blank" rel="noopener">فیس بک پیج ملاحظہ کریں</a></p>
</footer>

<a class="float-wa" href="https://wa.me/966566454430" target="_blank" rel="noopener" aria-label="واٹس ایپ پر رابطہ کریں">
  <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.6 6.32A7.85 7.85 0 0 0 12.02 4c-4.35 0-7.9 3.53-7.9 7.88 0 1.39.37 2.74 1.06 3.94L4 20l4.3-1.13a7.93 7.93 0 0 0 3.72.94h.01c4.35 0 7.9-3.53 7.9-7.88a7.8 7.8 0 0 0-2.33-5.6zm-5.58 12.1h-.01a6.6 6.6 0 0 1-3.36-.92l-.24-.14-2.5.65.67-2.43-.16-.25a6.53 6.53 0 0 1-1.01-3.48c0-3.62 2.96-6.57 6.62-6.57 1.77 0 3.43.69 4.68 1.94a6.5 6.5 0 0 1 1.94 4.64c0 3.62-2.96 6.56-6.63 6.56z"/></svg>
</a>

<!-- Lightbox -->
<div class="lightbox" id="lightbox">
  <div class="lightbox-inner">
    <div class="placeholder" id="lightboxContent">ا</div>
    <button class="lightbox-close" onclick="closeLightbox()">بند کریں</button>
  </div>
</div>

<script>
  // current year
  document.getElementById('year').textContent = new Date().getFullYear();

  // mobile nav toggle
  const burger = document.getElementById('burger');
  const navLinks = document.getElementById('navLinks');
  burger.addEventListener('click', () => {
    const open = navLinks.classList.toggle('open');
    burger.setAttribute('aria-expanded', open);
  });
  document.querySelectorAll('.nav-link').forEach(link => {
    link.addEventListener('click', () => {
      navLinks.classList.remove('open');
      burger.setAttribute('aria-expanded', 'false');
    });
  });

  // active link on scroll
  const sections = document.querySelectorAll('section[id]');
  const navItems = document.querySelectorAll('.nav-link');
  const setActive = () => {
    let current = 'home';
    sections.forEach(sec => {
      const top = sec.offsetTop - 120;
      if (window.scrollY >= top) current = sec.id;
    });
    navItems.forEach(a => {
      a.classList.toggle('active', a.getAttribute('href') === '#' + current);
    });
  };
  window.addEventListener('scroll', setActive);
  setActive();

  // scroll reveal
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) {
        e.target.classList.add('show');
        io.unobserve(e.target);
      }
    });
  }, { threshold: 0.15 });
  document.querySelectorAll('.reveal').forEach(el => io.observe(el));

  // lightbox
  function openLightbox(card) {
    const img = card.querySelector('img');
    const box = document.getElementById('lightboxContent');
    if (img) {
      box.outerHTML = `<img id="lightboxContent" src="${img.src}" alt="${img.alt}">`;
    } else {
      box.textContent = card.querySelector('.placeholder').textContent;
    }
    document.getElementById('lightbox').classList.add('open');
  }
  function closeLightbox() {
    document.getElementById('lightbox').classList.remove('open');
  }
  document.getElementById('lightbox').addEventListener('click', (e) => {
    if (e.target.id === 'lightbox') closeLightbox();
  });
  document.addEventListener('keydown', (e) => {
    if (e.key === 'Escape') closeLightbox();
  });
</script>

</body>
</html>
