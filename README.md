# smdigital.github.io<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Muhammad Sumair — Performance Marketer</title>
<meta name="description" content="Muhammad Sumair — Performance Marketer from Karachi. Meta Ads, Google Ads, YouTube Ads. Real campaigns. Real results."/>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Clash+Display:wght@400;500;600;700&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
:root{
  --bg:#080808;
  --bg2:#0f0f0f;
  --bg3:#161616;
  --card:#111111;
  --border:#1e1e1e;
  --border2:#2a2a2a;
  --text:#f0f0f0;
  --text2:#888888;
  --text3:#444444;
  --accent:#00d4ff;
  --accent2:#0099bb;
  --accent-dim:rgba(0,212,255,0.08);
  --accent-glow:rgba(0,212,255,0.18);
  --white:#ffffff;
  --ff-display:'Bebas Neue',sans-serif;
  --ff-head:'DM Sans',sans-serif;
  --ff-body:'DM Sans',sans-serif;
  --ease:cubic-bezier(.16,1,.3,1);
  --ease2:cubic-bezier(.4,0,.2,1);
}
html{scroll-behavior:smooth;}
body{font-family:var(--ff-body);background:var(--bg);color:var(--text);line-height:1.6;overflow-x:hidden;cursor:default;}
::selection{background:var(--accent);color:#000;}
::-webkit-scrollbar{width:3px;}
::-webkit-scrollbar-track{background:var(--bg);}
::-webkit-scrollbar-thumb{background:var(--accent);border-radius:2px;}

/* NOISE TEXTURE OVERLAY */
body::before{
  content:'';position:fixed;inset:0;z-index:0;pointer-events:none;
  background-image:url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
  opacity:.4;
}

/* ── NAV ────────────────────────────────── */
nav{
  position:fixed;top:0;left:0;right:0;z-index:100;
  padding:0 5%;height:64px;
  display:flex;align-items:center;justify-content:space-between;
  transition:all .4s var(--ease);
}
nav.scrolled{
  background:rgba(8,8,8,0.92);
  backdrop-filter:blur(24px);
  border-bottom:1px solid var(--border);
}
.nav-logo{
  font-family:var(--ff-display);
  font-size:1.4rem;letter-spacing:.08em;
  color:var(--text);text-decoration:none;
  display:flex;align-items:center;gap:.2rem;
}
.nav-logo span{color:var(--accent);}
.nav-links{display:flex;gap:2.5rem;list-style:none;}
.nav-links a{
  font-size:.8rem;font-weight:500;
  color:var(--text2);text-decoration:none;
  letter-spacing:.08em;text-transform:uppercase;
  transition:color .2s;
}
.nav-links a:hover{color:var(--accent);}
.nav-cta{
  font-size:.8rem;font-weight:600;
  color:#000;background:var(--accent);
  text-decoration:none;
  padding:.45rem 1.2rem;border-radius:4px;
  letter-spacing:.04em;
  transition:all .2s;
}
.nav-cta:hover{background:#00eeff;transform:translateY(-1px);}
.hamburger{display:none;flex-direction:column;gap:5px;cursor:pointer;padding:4px;}
.hamburger span{display:block;width:22px;height:1.5px;background:var(--text2);transition:.3s;}
.mob-menu{
  display:none;position:fixed;top:64px;left:0;right:0;
  background:rgba(8,8,8,0.98);backdrop-filter:blur(20px);
  border-bottom:1px solid var(--border);
  padding:1.5rem 5%;z-index:99;
}
.mob-menu.open{display:block;}
.mob-menu a{
  display:block;padding:.75rem 0;
  font-size:.9rem;font-weight:500;
  color:var(--text2);text-decoration:none;
  border-bottom:1px solid var(--border);
  text-transform:uppercase;letter-spacing:.06em;
  transition:color .2s;
}
.mob-menu a:last-child{border-bottom:none;}
.mob-menu a:hover{color:var(--accent);}

/* ── HERO ───────────────────────────────── */
#home{
  min-height:100vh;
  padding:100px 5% 60px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:3rem;
  align-items:center;
  max-width:1200px;
  margin:0 auto;
  position:relative;
}
.hero-left{position:relative;z-index:1;}
.hero-badge{
  display:inline-flex;align-items:center;gap:.5rem;
  background:var(--accent-dim);border:1px solid rgba(0,212,255,0.15);
  color:var(--accent);font-size:.7rem;font-weight:600;
  padding:.3rem .9rem;border-radius:100px;
  margin-bottom:1.75rem;letter-spacing:.1em;text-transform:uppercase;
  animation:fadeUp .6s var(--ease) both;
}
.hero-badge::before{content:'';width:5px;height:5px;background:var(--accent);border-radius:50%;animation:blink 2s infinite;}
@keyframes blink{0%,100%{opacity:1}50%{opacity:.2}}
.hero-name{
  font-family:var(--ff-display);
  font-size:clamp(4rem,7vw,7rem);
  line-height:.95;letter-spacing:.02em;
  color:var(--text);
  margin-bottom:1.5rem;
  animation:fadeUp .6s .1s var(--ease) both;
}
.hero-name span{
  display:block;color:var(--accent);
  -webkit-text-stroke:2px var(--accent);
  color:transparent;
}
.hero-desc{
  font-size:1rem;font-weight:300;
  color:var(--text2);line-height:1.8;
  max-width:420px;margin-bottom:2.5rem;
  animation:fadeUp .6s .2s var(--ease) both;
}
.hero-desc strong{color:var(--text);font-weight:500;}
.hero-btns{
  display:flex;gap:.75rem;flex-wrap:wrap;
  animation:fadeUp .6s .3s var(--ease) both;
}
.btn-primary{
  background:var(--accent);color:#000;
  padding:.7rem 1.75rem;border-radius:4px;
  font-size:.875rem;font-weight:700;
  text-decoration:none;letter-spacing:.02em;
  transition:all .2s;
}
.btn-primary:hover{background:#00eeff;transform:translateY(-2px);box-shadow:0 8px 24px rgba(0,212,255,0.3);}
.btn-outline{
  background:transparent;color:var(--text);
  padding:.7rem 1.75rem;border-radius:4px;
  font-size:.875rem;font-weight:600;
  text-decoration:none;
  border:1px solid var(--border2);
  transition:all .2s;
}
.btn-outline:hover{border-color:var(--accent);color:var(--accent);}

/* HERO RIGHT */
.hero-right{
  position:relative;z-index:1;
  display:flex;flex-direction:column;gap:1rem;
  animation:fadeUp .6s .2s var(--ease) both;
}
.hero-tagline-box{
  background:var(--accent);
  border-radius:12px;
  padding:1.75rem 2rem;
}
.hero-tagline-box p{
  font-family:var(--ff-display);
  font-size:clamp(1.1rem,2vw,1.4rem);
  letter-spacing:.04em;color:#000;
  line-height:1.3;
}
.hero-tagline-box span{
  display:block;font-family:var(--ff-body);
  font-size:.7rem;font-weight:600;
  color:rgba(0,0,0,0.5);letter-spacing:.12em;
  text-transform:uppercase;margin-top:.75rem;
}
.hero-stats-row{display:grid;grid-template-columns:1fr 1fr;gap:1rem;}
.hero-stat-box{
  background:var(--card);border:1px solid var(--border);
  border-radius:12px;padding:1.5rem;
  transition:border-color .2s;
}
.hero-stat-box:hover{border-color:var(--accent);}
.hero-stat-box:first-child{background:var(--bg3);}
.stat-big{
  font-family:var(--ff-display);
  font-size:2.75rem;letter-spacing:.02em;
  color:var(--text);display:block;line-height:1;
}
.stat-big span{color:var(--accent);}
.stat-lbl{font-size:.7rem;color:var(--text3);letter-spacing:.1em;text-transform:uppercase;margin-top:.35rem;display:block;}
.hero-stack-box{
  background:var(--card);border:1px solid var(--border);
  border-radius:12px;padding:1.25rem 1.5rem;
}
.stack-label{font-size:.65rem;color:var(--text3);letter-spacing:.12em;text-transform:uppercase;margin-bottom:.75rem;display:block;}
.stack-chips{display:flex;flex-wrap:wrap;gap:.4rem;}
.stack-chip{
  font-size:.72rem;font-weight:500;
  color:var(--accent);
  background:var(--accent-dim);
  border:1px solid rgba(0,212,255,0.15);
  padding:.25rem .65rem;border-radius:100px;
}

/* ── MARQUEE ────────────────────────────── */
.marquee-section{
  border-top:1px solid var(--border);
  border-bottom:1px solid var(--border);
  overflow:hidden;background:var(--bg2);
  padding:1.25rem 0;
}
.marquee-track{display:flex;gap:3rem;width:max-content;animation:marquee 30s linear infinite;}
.marquee-track:hover{animation-play-state:paused;}
.marquee-item{
  font-size:.72rem;font-weight:600;
  color:var(--text3);letter-spacing:.12em;
  text-transform:uppercase;white-space:nowrap;
  display:flex;align-items:center;gap:1rem;
}
.marquee-dot{color:var(--accent);font-size:.5rem;}
@keyframes marquee{from{transform:translateX(0)}to{transform:translateX(-50%)}}

/* ── SECTIONS ───────────────────────────── */
section{padding:100px 5%;}
.sec-inner{max-width:1200px;margin:0 auto;}
.eyebrow{
  font-size:.68rem;font-weight:700;
  color:var(--accent);letter-spacing:.18em;
  text-transform:uppercase;display:block;margin-bottom:.6rem;
}
.sec-title{
  font-family:var(--ff-display);
  font-size:clamp(2.5rem,5vw,4.5rem);
  letter-spacing:.02em;color:var(--text);
  line-height:1;margin-bottom:1rem;
}
.sec-title span{color:var(--accent);}
.sec-sub{font-size:.95rem;color:var(--text2);max-width:480px;line-height:1.8;}
.reveal{opacity:0;transform:translateY(28px);transition:opacity .7s var(--ease),transform .7s var(--ease);}
.reveal.visible{opacity:1;transform:translateY(0);}

/* ── SERVICES ───────────────────────────── */
#services{background:var(--bg);}
.services-top{
  display:flex;align-items:flex-end;justify-content:space-between;
  margin-bottom:3.5rem;flex-wrap:wrap;gap:1.5rem;
}
.services-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:1px;
  background:var(--border);
  border:1px solid var(--border);
  border-radius:16px;
  overflow:hidden;
}
.svc-card{
  background:var(--bg);
  padding:2.25rem 2rem;
  position:relative;
  overflow:hidden;
  transition:background .3s;
}
.svc-card::after{
  content:'';position:absolute;
  top:0;left:0;right:0;height:2px;
  background:linear-gradient(90deg,var(--accent),transparent);
  transform:scaleX(0);transform-origin:left;
  transition:transform .4s var(--ease);
}
.svc-card:hover{background:var(--bg2);}
.svc-card:hover::after{transform:scaleX(1);}
.svc-icon-wrap{
  width:44px;height:44px;
  background:var(--accent-dim);
  border:1px solid rgba(0,212,255,0.15);
  border-radius:10px;
  display:flex;align-items:center;justify-content:center;
  font-size:1.2rem;margin-bottom:1.25rem;
  transition:background .3s,border-color .3s;
}
.svc-card:hover .svc-icon-wrap{background:var(--accent-glow);border-color:rgba(0,212,255,0.3);}
.svc-num{
  font-family:var(--ff-display);
  font-size:.7rem;letter-spacing:.12em;
  color:var(--text3);margin-bottom:.5rem;display:block;
}
.svc-card h3{
  font-size:1.05rem;font-weight:700;
  color:var(--text);margin-bottom:.6rem;line-height:1.3;
}
.svc-card p{font-size:.85rem;color:var(--text2);line-height:1.7;}
.svc-arrow{
  display:block;margin-top:1.25rem;
  font-size:.78rem;font-weight:600;
  color:var(--accent);letter-spacing:.04em;
  opacity:0;transform:translateX(-8px);
  transition:all .3s var(--ease);
}
.svc-card:hover .svc-arrow{opacity:1;transform:translateX(0);}

/* ── SKILLS ─────────────────────────────── */
#skills{background:var(--bg2);}
.skills-layout{
  display:grid;grid-template-columns:1fr 1.2fr;
  gap:5rem;align-items:start;
}
.chips-wrap{display:flex;flex-wrap:wrap;gap:.5rem;margin-top:2rem;}
.chip{
  font-size:.78rem;font-weight:500;
  color:var(--text2);
  background:transparent;
  border:1px solid var(--border2);
  padding:.4rem .9rem;border-radius:4px;
  transition:all .2s;cursor:default;
}
.chip:hover{border-color:var(--accent);color:var(--accent);background:var(--accent-dim);}
.chip.active{
  background:var(--accent);color:#000;
  border-color:var(--accent);font-weight:700;
}
.bars-wrap{display:flex;flex-direction:column;gap:1.5rem;margin-top:2rem;}
.bar-item{}
.bar-top{display:flex;justify-content:space-between;margin-bottom:.5rem;}
.bar-name{font-size:.85rem;font-weight:500;color:var(--text);}
.bar-pct{font-size:.8rem;font-weight:700;color:var(--accent);}
.bar-track{height:2px;background:var(--border2);border-radius:2px;overflow:hidden;}
.bar-fill{
  height:100%;
  background:linear-gradient(90deg,var(--accent),#00ffee);
  border-radius:2px;
  transform:scaleX(0);transform-origin:left;
  transition:transform 1.2s var(--ease);
}

/* ── WORK ───────────────────────────────── */
#work{background:var(--bg);}
.work-header{margin-bottom:3rem;}
.work-grid{
  display:grid;grid-template-columns:1fr 1fr;
  gap:1rem;
}
.work-card{
  border-radius:14px;padding:2rem 2.25rem;
  position:relative;overflow:hidden;
  border:1px solid var(--border);
  transition:border-color .3s,transform .3s;
  background:var(--card);
}
.work-card:hover{border-color:var(--accent);transform:translateY(-4px);}
.work-card.dark{background:var(--bg3);}
.work-card.accent{background:var(--accent);border-color:var(--accent);}
.work-card.accent h3,.work-card.accent p,.work-card.accent .work-tag,.work-card.accent .work-link{color:#000;}
.work-card.accent .work-tag{background:rgba(0,0,0,0.15);color:#000;}
.work-card-top{display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:1.25rem;}
.work-tag{
  font-size:.65rem;font-weight:700;
  color:var(--accent);background:var(--accent-dim);
  border:1px solid rgba(0,212,255,0.15);
  padding:.2rem .65rem;border-radius:100px;
  letter-spacing:.1em;text-transform:uppercase;
}
.work-emoji{font-size:1.75rem;opacity:.8;}
.work-card h3{
  font-size:1.1rem;font-weight:700;
  color:var(--text);margin-bottom:.6rem;line-height:1.3;
}
.work-card p{font-size:.85rem;color:var(--text2);line-height:1.7;margin-bottom:1.25rem;}
.work-link{
  font-size:.78rem;font-weight:600;
  color:var(--accent);letter-spacing:.02em;
}

/* ── CONTACT ────────────────────────────── */
#contact{background:var(--bg2);}
.contact-layout{
  display:grid;grid-template-columns:1fr 1.4fr;
  gap:5rem;align-items:start;
}
.contact-left h2{
  font-family:var(--ff-display);
  font-size:clamp(3rem,5vw,5rem);
  letter-spacing:.02em;color:var(--text);
  line-height:.95;margin-bottom:1.5rem;
}
.contact-left h2 span{color:var(--accent);}
.contact-left p{font-size:.95rem;color:var(--text2);line-height:1.8;}
.contact-rows{display:flex;flex-direction:column;gap:.75rem;}
.contact-row{
  display:flex;align-items:center;gap:1.25rem;
  background:var(--card);border:1px solid var(--border);
  border-radius:10px;padding:1.1rem 1.4rem;
  text-decoration:none;
  transition:all .25s;
}
.contact-row:hover{border-color:var(--accent);transform:translateX(4px);}
.contact-row.highlighted{
  background:var(--accent);border-color:var(--accent);
}
.contact-row.highlighted .cr-label,.contact-row.highlighted .cr-value{color:#000;}
.cr-icon-box{
  width:36px;height:36px;flex-shrink:0;
  background:var(--accent-dim);border-radius:8px;
  display:flex;align-items:center;justify-content:center;
  font-size:1rem;
  transition:background .2s;
}
.contact-row.highlighted .cr-icon-box{background:rgba(0,0,0,0.15);}
.cr-text{}
.cr-label{
  font-size:.62rem;font-weight:700;
  color:var(--text3);letter-spacing:.12em;
  text-transform:uppercase;display:block;
}
.cr-value{font-size:.88rem;font-weight:500;color:var(--text);}

/* ── FOOTER ─────────────────────────────── */
footer{
  background:var(--bg);
  border-top:1px solid var(--border);
  padding:2rem 5%;
}
.footer-inner{
  max-width:1200px;margin:0 auto;
  display:flex;align-items:center;
  justify-content:space-between;flex-wrap:wrap;gap:1rem;
}
.footer-logo{
  font-family:var(--ff-display);
  font-size:1.1rem;letter-spacing:.08em;color:var(--text);
}
.footer-logo span{color:var(--accent);}
.footer-copy{font-size:.75rem;color:var(--text3);}
.footer-right{font-size:.75rem;color:var(--text3);letter-spacing:.06em;text-transform:uppercase;}

/* ── ANIMATIONS ─────────────────────────── */
@keyframes fadeUp{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}

/* ── RESPONSIVE ─────────────────────────── */
@media(max-width:960px){
  #home{grid-template-columns:1fr;padding-top:120px;}
  .hero-right{margin-top:2rem;}
  .hero-stats-row{grid-template-columns:1fr 1fr;}
  .services-grid{grid-template-columns:1fr 1fr;}
  .skills-layout{grid-template-columns:1fr;gap:3rem;}
  .work-grid{grid-template-columns:1fr;}
  .contact-layout{grid-template-columns:1fr;gap:2.5rem;}
  .nav-links,.nav-cta{display:none;}
  .hamburger{display:flex;}
}
@media(max-width:580px){
  section{padding:70px 4%;}
  .services-grid{grid-template-columns:1fr;}
  .hero-stats-row{grid-template-columns:1fr 1fr;}
  .hero-name{font-size:clamp(3.5rem,12vw,5rem);}
}
</style>
</head>
<body>

<!-- NAV -->
<nav id="navbar">
  <a href="#home" class="nav-logo">SM<span>.</span></a>
  <ul class="nav-links">
    <li><a href="#services">Services</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#work">Work</a></li>
    <li><a href="#contact">Let's Talk</a></li>
  </ul>
  <a href="#contact" class="nav-cta">Let's Talk</a>
  <div class="hamburger" onclick="toggleMenu()"><span></span><span></span><span></span></div>
</nav>
<div class="mob-menu" id="mobMenu">
  <a href="#services" onclick="closeMenu()">Services</a>
  <a href="#skills" onclick="closeMenu()">Skills</a>
  <a href="#work" onclick="closeMenu()">Work</a>
  <a href="#contact" onclick="closeMenu()">Let's Talk</a>
</div>

<!-- HERO -->
<div id="home">
  <!-- LEFT -->
  <div class="hero-left">
    <div class="hero-badge">Available for clients · Karachi, Pakistan</div>
    <h1 class="hero-name">
      Muhammad
      <span>Sumair</span>
    </h1>
    <p class="hero-desc">
      Based in Karachi. I run <strong>Meta Ads, Google Ads and YouTube Ads</strong> for businesses that are done spending money on campaigns that go nowhere.
    </p>
    <div class="hero-btns">
      <a href="#work" class="btn-primary">See My Work</a>
      <a href="#contact" class="btn-outline">Work With Me</a>
    </div>
  </div>

  <!-- RIGHT -->
  <div class="hero-right">
    <div class="hero-tagline-box">
      <p>"I don't sell ads. I build revenue engines."</p>
      <span>SM Digital · Performance Marketing</span>
    </div>
    <div class="hero-stats-row">
      <div class="hero-stat-box">
        <span class="stat-big">8<span>+</span></span>
        <span class="stat-lbl">Skills in stack</span>
      </div>
      <div class="hero-stat-box">
        <span class="stat-big">8</span>
        <span class="stat-lbl">Core services</span>
      </div>
    </div>
    <div class="hero-stack-box">
      <span class="stack-label">Full Stack</span>
      <div class="stack-chips">
        <span class="stack-chip">Meta Ads</span>
        <span class="stack-chip">Google Ads</span>
        <span class="stack-chip">YouTube Ads</span>
        <span class="stack-chip">Lead Gen</span>
        <span class="stack-chip">FB Analytics</span>
      </div>
    </div>
  </div>
</div>

<!-- MARQUEE -->
<div class="marquee-section">
  <div class="marquee-track">
    <div class="marquee-item">Meta Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Google Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">YouTube Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Facebook Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Lead Generation <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Ad Copywriting <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Retargeting <span class="marquee-dot">●</span></div>
    <div class="marquee-item">ROAS Optimization <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Campaign Analytics <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Audience Targeting <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Meta Pixel <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Page Management <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Meta Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Google Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">YouTube Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Facebook Ads <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Lead Generation <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Ad Copywriting <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Retargeting <span class="marquee-dot">●</span></div>
    <div class="marquee-item">ROAS Optimization <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Campaign Analytics <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Audience Targeting <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Meta Pixel <span class="marquee-dot">●</span></div>
    <div class="marquee-item">Page Management <span class="marquee-dot">●</span></div>
  </div>
</div>

<!-- SERVICES -->
<section id="services">
  <div class="sec-inner">
    <div class="services-top reveal">
      <div>
        <span class="eyebrow">What I Do</span>
        <h2 class="sec-title">Services</h2>
      </div>
      <p class="sec-sub">I don't offer everything. I focus on what I'm actually good at — and that focus is what gets results.</p>
    </div>
    <div class="services-grid reveal">

      <div class="svc-card">
        <div class="svc-icon-wrap">🎯</div>
        <span class="svc-num">01</span>
        <h3>Meta Ads</h3>
        <p>Facebook and Instagram campaigns built properly — cold traffic, retargeting, and conversion layers. Strategy, copy, targeting, and daily optimization. Not just boosting posts.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">🔍</div>
        <span class="svc-num">02</span>
        <h3>Google Ads</h3>
        <p>Search campaigns that put your business in front of people actively looking for what you sell. Keyword strategy, ad copy, and conversion tracking from day one.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">▶️</div>
        <span class="svc-num">03</span>
        <h3>YouTube Ads</h3>
        <p>Video campaigns that build awareness and drive action. Skippable, non-skippable, and bumper ad formats matched to your goal and your audience.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">✍️</div>
        <span class="svc-num">04</span>
        <h3>Ad Copywriting</h3>
        <p>Hooks that stop the scroll, body copy that holds attention, and CTAs that push people to act. Written specifically for your customer — not a generic template.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">📲</div>
        <span class="svc-num">05</span>
        <h3>Lead Generation</h3>
        <p>Lead form campaigns on Meta that bring in people who actually want to hear from you. Qualified leads with real intent — not just clicks from the curious.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">📊</div>
        <span class="svc-num">06</span>
        <h3>Campaign Analytics</h3>
        <p>I track ROAS, CPR, CTR, CPM and frequency weekly. When something works I scale it. When it doesn't I fix it. No guessing, no autopilot.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">📱</div>
        <span class="svc-num">07</span>
        <h3>Page Management</h3>
        <p>Your social pages stay active, consistent, and professional. Captions, hashtags, scheduling, and engagement — handled so you don't have to think about it.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

      <div class="svc-card">
        <div class="svc-icon-wrap">🎨</div>
        <span class="svc-num">08</span>
        <h3>Content Creation</h3>
        <p>Carousels, branded images, and reel graphics designed for each platform and built to match your brand identity — ready to post or run as ads.</p>
        <span class="svc-arrow">→ Get started</span>
      </div>

    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="sec-inner">
    <div class="skills-layout">
      <div class="reveal">
        <span class="eyebrow">Toolkit</span>
        <h2 class="sec-title">Skills &<br><span>Tools</span></h2>
        <p class="sec-sub">Paid ads across three platforms, copy that converts, and the data to back every decision.</p>
        <div class="chips-wrap">
          <span class="chip active">Meta Ads Manager</span>
          <span class="chip active">Google Ads</span>
          <span class="chip active">YouTube Ads</span>
          <span class="chip">Facebook Ads</span>
          <span class="chip">Instagram Ads</span>
          <span class="chip">Meta Pixel</span>
          <span class="chip">Custom Audiences</span>
          <span class="chip">Lookalike Audiences</span>
          <span class="chip">Retargeting</span>
          <span class="chip">Ad Copywriting</span>
          <span class="chip">Campaign Structure</span>
          <span class="chip">ROAS Optimization</span>
          <span class="chip">Lead Generation</span>
          <span class="chip">Page Management</span>
          <span class="chip">Audience Targeting</span>
          <span class="chip">A/B Testing</span>
          <span class="chip">Content Creation</span>
        </div>
      </div>
      <div class="reveal">
        <span class="eyebrow">Proficiency</span>
        <h2 class="sec-title" style="font-size:2rem;">Core<br><span>Strengths</span></h2>
        <div class="bars-wrap">
          <div class="bar-item">
            <div class="bar-top"><span class="bar-name">Meta Ads Strategy</span><span class="bar-pct">90%</span></div>
            <div class="bar-track"><div class="bar-fill" data-w="0.9"></div></div>
          </div>
          <div class="bar-item">
            <div class="bar-top"><span class="bar-name">Ad Copywriting</span><span class="bar-pct">90%</span></div>
            <div class="bar-track"><div class="bar-fill" data-w="0.9"></div></div>
          </div>
          <div class="bar-item">
            <div class="bar-top"><span class="bar-name">Google Ads</span><span class="bar-pct">90%</span></div>
            <div class="bar-track"><div class="bar-fill" data-w="0.9"></div></div>
          </div>
          <div class="bar-item">
            <div class="bar-top"><span class="bar-name">YouTube Ads</span><span class="bar-pct">90%</span></div>
            <div class="bar-track"><div class="bar-fill" data-w="0.9"></div></div>
          </div>
          <div class="bar-item">
            <div class="bar-top"><span class="bar-name">Audience Targeting</span><span class="bar-pct">90%</span></div>
            <div class="bar-track"><div class="bar-fill" data-w="0.9"></div></div>
          </div>
          <div class="bar-item">
            <div class="bar-top"><span class="bar-name">Campaign Optimization</span><span class="bar-pct">90%</span></div>
            <div class="bar-track"><div class="bar-fill" data-w="0.9"></div></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- WORK -->
<section id="work">
  <div class="sec-inner">
    <div class="work-header reveal">
      <span class="eyebrow">Experience & Projects</span>
      <h2 class="sec-title">Work I've Done</h2>
    </div>
    <div class="work-grid reveal">

      <div class="work-card dark">
        <div class="work-card-top">
          <span class="work-tag">Meta Ads</span>
          <span class="work-emoji">🎯</span>
        </div>
        <h3>Meta Ads Funnel — Clothing E-commerce Brand</h3>
        <p>Set up a 3-layer campaign — cold traffic at the top, retargeting in the middle, conversion at the bottom. Wrote all the ad copy, built the audiences, mapped the budget across each layer.</p>
        <span class="work-link">→ Full Funnel Strategy</span>
      </div>

      <div class="work-card">
        <div class="work-card-top">
          <span class="work-tag">Social Media</span>
          <span class="work-emoji">📱</span>
        </div>
        <h3>Social Media Buildout — Local Service Business</h3>
        <p>Started from zero. Set up Instagram and Facebook pages, wrote the bio, built a 30-day content calendar, and wrote every caption with platform-specific hashtags.</p>
        <span class="work-link">→ Full Content System</span>
      </div>

      <div class="work-card">
        <div class="work-card-top">
          <span class="work-tag">Copywriting</span>
          <span class="work-emoji">✍️</span>
        </div>
        <h3>Ad Copy Portfolio — 3 Different Niches</h3>
        <p>Wrote 9 Meta Ad scripts across e-commerce, clothing, and food. Each one has a hook, problem, offer, social proof line, and CTA using PAS and AIDA frameworks.</p>
        <span class="work-link">→ Copywriting Samples</span>
      </div>

      <div class="work-card accent">
        <div class="work-card-top">
          <span class="work-tag">Personal Brand</span>
          <span class="work-emoji">🚀</span>
        </div>
        <h3>SM Digital — Built From Zero</h3>
        <p>Built my entire brand from scratch. Identity across 5 platforms, 90-day content calendar, this website, and a professional CV. Documented the whole process publicly.</p>
        <span class="work-link">→ linkedin.com/in/muhammad-sumair-896410378</span>
      </div>

    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="sec-inner">
    <div class="contact-layout">
      <div class="reveal">
        <span class="eyebrow">Get In Touch</span>
        <h2 class="contact-left" style="font-family:var(--ff-display);font-size:clamp(3rem,5vw,5rem);letter-spacing:.02em;color:var(--text);line-height:.95;margin-bottom:1.5rem;">
          Let's Build<br><span style="color:var(--accent);">Something.</span>
        </h2>
        <p style="font-size:.95rem;color:var(--text2);line-height:1.8;">Open to freelance projects, long-term clients, and collaborations. If your ads aren't converting — let's fix that.</p>
      </div>
      <div class="contact-rows reveal">
        <a class="contact-row highlighted" href="https://linkedin.com/in/muhammad-sumair-896410378" target="_blank">
          <div class="cr-icon-box">💼</div>
          <div class="cr-text">
            <span class="cr-label">LinkedIn</span>
            <span class="cr-value">muhammad-sumair-896410378</span>
          </div>
        </a>
        <a class="contact-row" href="https://wa.me/923310310587" target="_blank">
          <div class="cr-icon-box">📲</div>
          <div class="cr-text">
            <span class="cr-label">WhatsApp</span>
            <span class="cr-value">+92 331 0310587</span>
          </div>
        </a>
        <a class="contact-row" href="mailto:sumairmarketer10@gmail.com">
          <div class="cr-icon-box">✉️</div>
          <div class="cr-text">
            <span class="cr-label">Email</span>
            <span class="cr-value">sumairmarketer10@gmail.com</span>
          </div>
        </a>
        <a class="contact-row" href="https://www.instagram.com/smdigital.co?igsh=MTd5azN1ZzBmYThhNQ==" target="_blank">
          <div class="cr-icon-box">📸</div>
          <div class="cr-text">
            <span class="cr-label">Instagram</span>
            <span class="cr-value">@smdigital.co</span>
          </div>
        </a>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-logo">SM<span>.</span></div>
    <span class="footer-copy">© 2026 Muhammad Sumair. All rights reserved.</span>
    <span class="footer-right">Performance Marketer · Karachi</span>
  </div>
</footer>

<script>
window.addEventListener('scroll',()=>{
  document.getElementById('navbar').classList.toggle('scrolled',window.scrollY>20);
});
function toggleMenu(){document.getElementById('mobMenu').classList.toggle('open');}
function closeMenu(){document.getElementById('mobMenu').classList.remove('open');}

const revealObs=new IntersectionObserver((entries)=>{
  entries.forEach((e,i)=>{
    if(e.isIntersecting){
      setTimeout(()=>e.target.classList.add('visible'),i*80);
      revealObs.unobserve(e.target);
    }
  });
},{threshold:0.08});
document.querySelectorAll('.reveal').forEach(el=>revealObs.observe(el));

const barObs=new IntersectionObserver((entries)=>{
  entries.forEach(e=>{
    if(e.isIntersecting){
      e.target.querySelectorAll('.bar-fill').forEach((bar,i)=>{
        setTimeout(()=>{bar.style.transform=`scaleX(${bar.getAttribute('data-w')||0.9})`;},i*100);
      });
      barObs.unobserve(e.target);
    }
  });
},{threshold:0.2});
document.querySelectorAll('.bars-wrap').forEach(el=>barObs.observe(el));

const sections=document.querySelectorAll('section[id],div[id]');
window.addEventListener('scroll',()=>{
  let cur='';
  sections.forEach(s=>{if(window.scrollY>=s.offsetTop-100)cur=s.getAttribute('id');});
  document.querySelectorAll('.nav-links a').forEach(a=>{
    a.style.color=a.getAttribute('href')==='#'+cur?'var(--accent)':'';
  });
});
</script>
</body>
</html>
