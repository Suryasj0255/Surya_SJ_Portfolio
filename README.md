<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Surya S J — UI/UX Designer &amp; Product Designer</title>
<meta name="description" content="Portfolio of Surya S J — Award-winning UI/UX Designer with 3+ years of experience designing scalable design systems, enterprise SaaS dashboards, and intuitive digital products.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,500;0,9..144,600;1,9..144,400;1,9..144,500&family=Inter:wght@300;400;500;600;700&family=IBM+Plex+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#0A0A0A;
    --panel:#141414;
    --panel-hover:#1A1A1A;
    --ink:#F4F2EC;
    --muted:#8E8E86;
    --line:#262624;
    --cobalt:#5C7CFA;
    --cobalt-dim:#141828;
    --cobalt-border:rgba(92,124,250,0.28);
    --amber:#D9CBA3;
    --amber-dim:rgba(217,203,163,0.12);
    --display:'Fraunces', Georgia, serif;
    --body:'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    --mono:'IBM Plex Mono', monospace;
    --maxw:1220px;
  }
  *{box-sizing:border-box; margin:0; padding:0;}
  html{scroll-behavior:smooth; cursor:none;}
  body{
    background:var(--paper);
    color:var(--ink);
    font-family:var(--body);
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
    cursor:none;
  }
  body::after{
    content:""; position:fixed; inset:0; pointer-events:none; z-index:2; opacity:0.045; mix-blend-mode:overlay;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='120' height='120'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='2' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
  }
  a{color:inherit; text-decoration:none;}
  ::selection{background:var(--cobalt); color:#0A0A0A;}
  img{max-width:100%; display:block;}
  * { cursor:none; }

  #cursor-dot{
    position:fixed; top:0; left:0; width:8px; height:8px; border-radius:50%; background:var(--amber);
    pointer-events:none; z-index:9999; transform:translate(-50%,-50%); transition:opacity .2s ease;
    mix-blend-mode:difference;
  }
  #cursor-ring{
    position:fixed; top:0; left:0; width:34px; height:34px; border-radius:50%; border:1px solid var(--amber);
    pointer-events:none; z-index:9998; transform:translate(-50%,-50%); transition:width .2s ease, height .2s ease, opacity .2s ease;
    opacity:0.6;
  }

  .wrap{
    max-width:var(--maxw);
    margin:0 auto;
    padding:0 40px;
    position:relative;
    z-index:1;
  }

  a:focus-visible, button:focus-visible{outline:2px solid var(--amber); outline-offset:3px; border-radius:2px;}

  /* ---------- NAV ---------- */
  header.nav{
    position:sticky; top:0; z-index:50;
    background:rgba(10,10,10,0.88);
    backdrop-filter:blur(12px);
    border-bottom:1px solid var(--line);
  }
  .nav-inner{
    max-width:var(--maxw); margin:0 auto; padding:18px 40px;
    display:flex; align-items:center; justify-content:space-between;
  }
  .nav-mark{
    font-family:var(--display); font-weight:600; font-size:1.15rem; font-style:italic;
    letter-spacing:0.01em; display:flex; align-items:center; gap:8px;
  }
  .nav-mark .dot{width:7px; height:7px; border-radius:50%; background:var(--amber); display:inline-block; animation:pulse 2.4s ease-in-out infinite;}
  @keyframes pulse{0%,100%{opacity:1; transform:scale(1);} 50%{opacity:.3; transform:scale(0.85);}}
  nav.links{display:flex; gap:26px; font-size:0.72rem;}
  nav.links a{position:relative; padding:4px 0; color:var(--muted); font-weight:500; text-transform:uppercase; letter-spacing:0.12em;
    transition:color .2s ease;}
  nav.links a:hover{color:var(--ink);}
  .nav-actions{display:flex; align-items:center; gap:12px;}
  .nav-resume-btn{
    font-family:var(--mono); font-size:0.7rem; letter-spacing:0.06em; text-transform:uppercase;
    border:1px solid var(--line); padding:8px 16px; border-radius:100px; color:var(--amber);
    background:var(--panel);
    transition:border-color .2s ease, transform .15s ease, background .2s ease;
    white-space:nowrap;
    display:inline-flex; align-items:center; gap:6px;
  }
  .nav-resume-btn:hover{border-color:var(--amber); transform:translateY(-1px); background:var(--panel-hover);}
  .nav-cta{
    font-family:var(--mono); font-size:0.7rem; letter-spacing:0.06em; text-transform:uppercase;
    border:1px solid var(--ink); padding:8px 18px; border-radius:100px;
    transition:background .2s ease, color .2s ease, transform .15s ease;
    white-space:nowrap;
  }
  .nav-cta:hover{background:var(--ink); color:var(--paper); transform:translateY(-1px);}

  /* ---------- MARQUEE ---------- */
  .marquee{
    border-top:1px solid var(--line); border-bottom:1px solid var(--line); overflow:hidden; white-space:nowrap; padding:13px 0;
    background:var(--paper);
  }
  .marquee-track{display:inline-block; animation:scrollmq 36s linear infinite;}
  .marquee-track span{
    font-family:var(--display); font-style:italic; font-size:1.02rem; color:var(--muted); margin:0 24px; display:inline-block;
  }
  .marquee-track span em{color:var(--amber); font-style:normal; font-family:var(--mono); font-size:0.65rem; letter-spacing:0.1em; text-transform:uppercase; margin-right:8px;}
  @keyframes scrollmq{ from{transform:translateX(0);} to{transform:translateX(-50%);} }

  /* ---------- SECTION SPACING ---------- */
  section{
    padding:130px 0 110px;
    border-top:1px solid var(--line);
    position:relative;
    width:100%;
    clear:both;
  }
  section.hero{
    border-top:none;
    padding:95px 0 85px;
  }
  section#expertise{
    border-top:none;
  }
  .section-head{
    margin-bottom:52px;
    max-width:760px;
  }
  .section-head .eyebrow{
    margin-bottom:12px;
  }
  .section-head h2{
    font-family:var(--display);
    font-weight:500;
    font-size:clamp(1.95rem, 3.6vw, 3rem);
    letter-spacing:-0.025em;
    line-height:1.1;
    color:var(--ink);
    margin-bottom:8px;
  }
  .section-head .section-sub{
    font-size:0.95rem;
    color:var(--muted);
    line-height:1.55;
  }
  .reveal{
    opacity:0;
    transform:translateY(28px);
    transition:opacity .8s cubic-bezier(.2,.7,.2,1), transform .8s cubic-bezier(.2,.7,.2,1);
  }
  .reveal.in{
    opacity:1;
    transform:translateY(0);
  }

  /* ---------- HERO ---------- */
  .hero-grid{display:grid; grid-template-columns:1.12fr 0.88fr; gap:44px; align-items:center;}
  
  .hero-id{
    display:flex; align-items:center; gap:16px; margin-bottom:20px;
  }
  .hero-avatar-badge{
    width:64px; height:64px; border-radius:50%;
    background:linear-gradient(135deg, #2A2A26 0%, #151515 100%);
    border:2px solid var(--amber);
    position:relative; flex-shrink:0;
    box-shadow:0 0 0 4px rgba(217,203,163,0.14);
  }
  .hero-avatar-img{
    width:100%; height:100%; border-radius:50%;
    object-fit:cover; object-position:center 15%;
    display:block;
  }
  .avatar-status{
    position:absolute; bottom:0; right:0; width:14px; height:14px; border-radius:50%;
    background:#10B981; border:2.5px solid var(--paper);
    box-shadow:0 0 8px #10B981;
  }
  .hero-id-text{display:flex; flex-direction:column; gap:1px;}
  .hero-id-text strong{
    font-family:var(--display); font-weight:500; font-style:italic; font-size:1.1rem; letter-spacing:0.01em;
  }
  .hero-id-text span{font-size:0.75rem; color:var(--muted); font-family:var(--mono);}
  
  .eyebrow{
    font-family:var(--mono); font-size:0.72rem; letter-spacing:0.16em; text-transform:uppercase;
    color:var(--amber); display:flex; align-items:center; gap:10px; margin-bottom:16px;
  }
  .eyebrow::before{content:""; width:26px; height:1px; background:var(--amber);}
  
  h1.headline{
    font-family:var(--display); font-weight:500; font-style:normal;
    font-size:clamp(2.35rem, 4.6vw, 4rem);
    line-height:1.04; letter-spacing:-0.025em;
    margin-bottom:18px;
  }
  h1.headline .accent{color:var(--amber); font-style:italic;}
  .hero-sub{
    font-size:1.02rem; color:#BCBCB5; max-width:44ch; margin-bottom:28px; line-height:1.6;
  }

  .hero-actions{display:flex; gap:12px; flex-wrap:wrap; margin-bottom:30px;}
  .btn{
    display:inline-flex; align-items:center; gap:8px;
    font-family:var(--mono); font-weight:500; font-size:0.76rem; letter-spacing:0.05em; text-transform:uppercase;
    padding:13px 22px; border-radius:100px; transition:transform .18s ease, box-shadow .18s ease, background .2s ease, border-color .2s ease;
  }
  .btn-primary{background:var(--ink); color:var(--paper);}
  .btn-primary:hover{transform:translateY(-2px); box-shadow:0 10px 24px -6px rgba(217,203,163,0.35);}
  .btn-ghost{border:1px solid var(--line); color:var(--ink);}
  .btn-ghost:hover{transform:translateY(-2px); border-color:var(--amber); background:rgba(255,255,255,0.02);}
  
  .hero-meta{
    display:flex; gap:14px 18px; font-family:var(--mono); font-size:0.72rem; color:var(--muted); flex-wrap:wrap; letter-spacing:0.02em;
    padding-top:18px; border-top:1px solid var(--line); align-items:center;
  }
  .hero-meta span, .hero-meta a{
    display:inline-flex; align-items:center; gap:6px; color:var(--muted);
    transition:color .18s ease, transform .15s ease;
  }
  .hero-meta a:hover{
    color:var(--amber); transform:translateY(-1px);
  }
  .hero-meta a b{
    color:var(--ink); font-weight:600;
  }

  /* ---------- GAMIFIED HERO: DESIGN ARCADE & VIBE SANDBOX ---------- */
  .arcade-card{
    background:var(--panel); border:1px solid var(--line); border-radius:12px;
    box-shadow:0 35px 70px -25px rgba(0,0,0,0.9);
    padding:22px; position:relative; overflow:hidden;
  }
  .arcade-header{
    display:flex; align-items:center; justify-content:space-between; margin-bottom:14px;
    padding-bottom:12px; border-bottom:1px solid var(--line);
  }
  .arcade-title-group{display:flex; align-items:center; gap:8px;}
  .arcade-live-dot{
    width:8px; height:8px; border-radius:50%; background:#10B981;
    box-shadow:0 0 10px #10B981; animation:pulse 2s infinite;
  }
  .arcade-title{font-family:var(--mono); font-size:0.75rem; font-weight:600; color:var(--amber); letter-spacing:0.06em; text-transform:uppercase;}
  
  /* GAMIFIED STATS BAR */
  .arcade-stats{
    display:flex; align-items:center; gap:12px; font-family:var(--mono); font-size:0.68rem; color:var(--muted);
  }
  .stat-badge{
    background:rgba(255,255,255,0.04); border:1px solid var(--line); padding:3px 8px; border-radius:100px;
    color:var(--ink); font-weight:600;
  }
  .stat-badge b{color:var(--amber);}

  /* ARCADE MODE TABS */
  .arcade-nav{
    display:flex; gap:6px; margin-bottom:16px; background:rgba(0,0,0,0.3); padding:4px; border-radius:8px;
    border:1px solid rgba(255,255,255,0.03);
  }
  .arcade-tab-btn{
    flex:1; font-family:var(--mono); font-size:0.65rem; letter-spacing:0.04em; text-transform:uppercase;
    background:transparent; border:none; color:var(--muted); padding:6px 8px; border-radius:6px;
    cursor:pointer; transition:all .18s ease; text-align:center;
  }
  .arcade-tab-btn.active{
    background:var(--amber-dim); color:var(--amber); font-weight:600; box-shadow:0 2px 8px rgba(0,0,0,0.4);
  }

  /* GAME ARENA VIEWPORT */
  .arcade-viewport{
    min-height:200px; position:relative; background:rgba(0,0,0,0.45); border:1px solid var(--line);
    border-radius:8px; padding:16px; overflow:hidden; display:flex; flex-direction:column; justify-content:center;
  }
  .game-panel{display:none; width:100%;}
  .game-panel.active{display:block; animation:fadeIn .2s ease forwards;}

  /* GAME 1: CATCH THE SPARK (CLICKING TARGETS) */
  #game-arena{
    position:relative; width:100%; height:190px; border-radius:6px; overflow:hidden;
    background:radial-gradient(circle at center, rgba(92,124,250,0.06) 0%, transparent 70%);
  }
  .arena-overlay{
    position:absolute; inset:0; display:flex; flex-direction:column; align-items:center; justify-content:center;
    text-align:center; z-index:10; background:rgba(10,10,10,0.7); backdrop-filter:blur(4px);
  }
  .arena-overlay h4{font-family:var(--display); font-size:1.15rem; font-style:italic; margin-bottom:4px;}
  .arena-overlay p{font-size:0.75rem; color:var(--muted); margin-bottom:14px; max-width:28ch;}
  .play-start-btn{
    font-family:var(--mono); font-size:0.72rem; text-transform:uppercase; letter-spacing:0.08em;
    background:var(--amber); color:#0A0A0A; border:none; padding:8px 20px; border-radius:100px;
    font-weight:700; cursor:pointer; box-shadow:0 0 20px rgba(217,203,163,0.4);
    transition:transform .15s ease, box-shadow .15s ease;
  }
  .play-start-btn:hover{transform:scale(1.05); box-shadow:0 0 25px rgba(217,203,163,0.7);}

  .spark-target{
    position:absolute; width:34px; height:34px; border-radius:50%;
    display:flex; align-items:center; justify-content:center; font-size:1.1rem;
    cursor:pointer; user-select:none; animation:floatOrb 3s ease-in-out infinite alternate;
    box-shadow:0 0 16px currentColor; transition:transform .1s ease;
  }
  .spark-target:hover{transform:scale(1.25);}
  @keyframes floatOrb{0%{transform:translateY(0px) rotate(0deg);} 100%{transform:translateY(-14px) rotate(15deg);}}

  .game-hud{
    position:absolute; top:8px; left:10px; right:10px; display:flex; justify-content:space-between;
    font-family:var(--mono); font-size:0.68rem; color:var(--muted); z-index:5; pointer-events:none;
  }
  .game-hud b{color:var(--ink);}

  /* GAME 2: OPTICAL PIXEL BALANCE */
  .balance-game-wrap{text-align:center; padding:10px 0;}
  .balance-stage{
    width:100%; height:80px; border:1px dashed var(--line); border-radius:6px; position:relative;
    margin:12px 0 16px; background:rgba(255,255,255,0.01); display:flex; align-items:center; justify-content:center;
  }
  .target-zone{
    width:48px; height:48px; border:1.5px solid var(--line); border-radius:8px;
    position:absolute; left:50%; transform:translateX(-50%); display:flex; align-items:center; justify-content:center;
    transition:border-color .2s ease, box-shadow .2s ease;
  }
  .target-zone.locked{border-color:#10B981; box-shadow:0 0 18px rgba(16,185,129,0.5);}
  .movable-orb{
    width:32px; height:32px; border-radius:6px; background:var(--cobalt); position:absolute;
    box-shadow:0 4px 12px rgba(92,124,250,0.4); display:flex; align-items:center; justify-content:center;
    font-size:0.8rem; color:#fff; transition:left .05s linear;
  }
  .balance-slider-row{display:flex; align-items:center; gap:12px; justify-content:center;}
  .balance-slider{
    width:70%; accent-color:var(--amber); cursor:pointer; height:4px;
  }
  .balance-feedback{
    font-family:var(--mono); font-size:0.72rem; color:var(--amber); margin-top:8px; min-height:18px;
  }

  /* GAME 3: SUPERCHARGED LIKE MACHINE */
  .like-machine-wrap{
    text-align:center; padding:12px 0; position:relative;
  }
  .like-machine-btn{
    display:inline-flex; align-items:center; gap:10px;
    background:linear-gradient(135deg, #F43F5E 0%, #E11D48 100%);
    color:#FFFFFF; border:none; padding:14px 28px; border-radius:100px;
    font-family:var(--body); font-size:0.95rem; font-weight:700; cursor:pointer;
    box-shadow:0 10px 30px -5px rgba(244,63,94,0.6); position:relative; overflow:hidden;
    transition:transform .12s ease, box-shadow .12s ease;
  }
  .like-machine-btn:hover{transform:scale(1.06); box-shadow:0 14px 36px -4px rgba(244,63,94,0.8);}
  .like-machine-btn:active{transform:scale(0.96);}
  .like-combo-badge{
    font-family:var(--mono); font-size:0.7rem; color:var(--amber); margin-top:14px;
    display:flex; align-items:center; justify-content:center; gap:6px;
  }
  .achievement-pill{
    display:inline-block; font-family:var(--mono); font-size:0.65rem; color:#10B981;
    background:rgba(16,185,129,0.1); border:1px solid rgba(16,185,129,0.25);
    padding:4px 10px; border-radius:100px; margin-top:8px;
  }

  /* FLOATING PARTICLE HEARTS/STARS */
  .floating-sparkle{
    position:absolute; pointer-events:none; z-index:100;
    font-size:1.3rem; animation:floatAway 1.2s cubic-bezier(0.2, 0.8, 0.2, 1) forwards;
  }
  @keyframes floatAway{
    0%{opacity:1; transform:translate(0, 0) scale(0.6) rotate(0deg);}
    100%{opacity:0; transform:translate(var(--dx), var(--dy)) scale(1.4) rotate(var(--dr));}
  }

  .arcade-footer{
    display:flex; justify-content:space-between; align-items:center; margin-top:14px;
    padding-top:12px; border-top:1px solid var(--line); font-family:var(--mono); font-size:0.65rem; color:var(--muted);
  }

  /* ---------- CORE EXPERTISE & TOOLS (SECTION 2) ---------- */
  .token-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
    border-radius:8px;
    overflow:hidden;
  }
  .token-card{
    background:var(--paper);
    padding:40px 32px;
    transition:background .25s ease;
  }
  .token-card:hover{background:var(--panel);}
  .token-card .swatch{
    width:10px;
    height:10px;
    border-radius:50%;
    margin-bottom:20px;
  }
  .token-card:nth-child(1) .swatch{background:var(--amber);}
  .token-card:nth-child(2) .swatch{background:var(--cobalt);}
  .token-card:nth-child(3) .swatch{background:var(--ink);}
  .token-card h3{
    font-family:var(--display);
    font-weight:500;
    font-size:1.25rem;
    margin-bottom:18px;
    font-style:italic;
  }
  .pill-row{display:flex; flex-wrap:wrap; gap:8px;}
  .pill{
    font-family:var(--mono);
    font-size:0.68rem;
    color:var(--muted);
    background:transparent;
    border:1px solid var(--line);
    padding:6px 12px;
    border-radius:100px;
    transition:border-color .15s ease, color .15s ease;
  }
  .token-card:hover .pill{
    border-color:rgba(255,255,255,0.14);
    color:#E0DED7;
  }

  /* ---------- SELECTED WORK (SECTION 3) ---------- */
  .work-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
    border-radius:8px;
    overflow:hidden;
    margin-bottom:48px;
  }
  .work-card{
    background:var(--paper);
    overflow:hidden;
    display:flex;
    flex-direction:column;
    position:relative;
    transition:background .25s ease;
  }
  .work-card:hover{background:var(--panel);}
  .work-thumb{
    aspect-ratio:4/3.3;
    overflow:hidden;
    background:#111;
    filter:grayscale(1) contrast(1.05);
    transition:filter .4s ease;
  }
  .work-card:hover .work-thumb{filter:grayscale(0) contrast(1);}
  .work-thumb img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:transform .6s cubic-bezier(.2,.7,.2,1);
  }
  .work-card:hover .work-thumb img{transform:scale(1.05);}
  .work-info{padding:22px 24px 26px;}
  .work-tag{
    font-family:var(--mono);
    font-size:0.62rem;
    color:var(--amber);
    letter-spacing:0.08em;
    text-transform:uppercase;
  }
  .work-info h3{
    font-family:var(--display);
    font-weight:500;
    font-style:italic;
    font-size:1.15rem;
    margin:8px 0 4px;
  }
  .work-info p{font-size:0.82rem; color:var(--muted); line-height:1.45;}
  .work-arrow{
    position:absolute;
    top:20px;
    right:20px;
    width:30px;
    height:30px;
    border-radius:50%;
    background:var(--ink);
    color:var(--paper);
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:0.88rem;
    opacity:0;
    transform:translateY(-6px) rotate(-30deg);
    transition:opacity .25s ease, transform .25s ease;
  }
  .work-card:hover .work-arrow{opacity:1; transform:translateY(0) rotate(0);}
  
  .work-cta-row{
    display:flex;
    align-items:center;
    justify-content:flex-start;
    padding-top:12px;
    margin-bottom:10px;
  }

  /* ---------- EXPERIENCE (SECTION 4) ---------- */
  .timeline{position:relative; padding-left:0;}
  .tl-item{
    position:relative;
    padding:0;
    border-top:1px solid var(--line);
  }
  .tl-item:first-child{border-top:none;}
  .tl-card{
    background:transparent;
    border:none;
    border-radius:0;
    padding:46px 0;
    display:grid;
    grid-template-columns:140px 1fr;
    gap:36px;
  }
  .tl-role{
    font-family:var(--display);
    font-weight:500;
    font-style:italic;
    font-size:1.55rem;
    grid-column:2;
    margin-bottom:6px;
    line-height:1.2;
  }
  .tl-role span{
    color:var(--amber);
    font-weight:500;
    font-size:0.92rem;
    font-family:var(--body);
    font-style:normal;
    display:block;
    margin-top:3px;
  }
  .tl-date{
    font-family:var(--mono);
    font-size:0.72rem;
    color:var(--muted);
    border:none;
    background:none;
    padding:0;
    grid-column:1;
    grid-row:1/4;
    align-self:start;
    padding-top:6px;
    letter-spacing:0.02em;
  }
  .tl-tags{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin:0 0 20px;
    grid-column:2;
  }
  .tl-tags span{
    font-family:var(--mono);
    font-size:0.64rem;
    color:var(--amber);
    background:none;
    border:1px solid var(--line);
    padding:5px 12px;
    border-radius:100px;
  }
  .tl-products-box{
    grid-column:2;
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:6px;
    padding:20px 22px;
    margin-bottom:22px;
  }
  .tl-products-title{
    font-family:var(--mono);
    font-size:0.7rem;
    color:var(--amber);
    text-transform:uppercase;
    letter-spacing:0.08em;
    margin-bottom:12px;
    display:block;
  }
  .tl-products-grid{
    display:grid;
    grid-template-columns:repeat(2, 1fr);
    gap:12px;
  }
  .tl-product-item{
    background:rgba(255,255,255,0.02);
    border:1px solid var(--line);
    border-radius:4px;
    padding:12px 14px;
  }
  .tl-product-item strong{
    font-size:0.86rem;
    color:var(--ink);
    display:block;
    margin-bottom:3px;
    font-family:var(--body);
  }
  .tl-product-item p{
    font-size:0.76rem;
    color:var(--muted);
    line-height:1.45;
  }
  .tl-list{
    list-style:none;
    display:flex;
    flex-direction:column;
    gap:14px;
    grid-column:2;
    max-width:70ch;
  }
  .tl-list li{
    padding-left:20px;
    position:relative;
    font-size:0.92rem;
    color:#C9C7BE;
    line-height:1.55;
  }
  .tl-list li::before{
    content:"—";
    position:absolute;
    left:0;
    color:var(--amber);
  }
  .tl-list b{font-weight:600; color:var(--ink);}

  /* ---------- AWARDS SECTION (SECTION 5) ---------- */
  .awards-grid{
    display:grid;
    grid-template-columns:repeat(2, 1fr);
    gap:24px;
    align-items:stretch;
  }
  .award-card{
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:8px;
    padding:36px 32px;
    position:relative;
    overflow:hidden;
    display:flex;
    flex-direction:column;
    transition:border-color .25s ease, transform .25s ease, background .25s ease, box-shadow .25s ease;
  }
  .award-card:hover{
    border-color:var(--amber);
    transform:translateY(-3px);
    background:var(--panel-hover);
    box-shadow:0 18px 36px -12px rgba(0,0,0,0.6);
  }
  .award-badge-top{
    display:inline-flex;
    align-items:center;
    gap:8px;
    font-family:var(--mono);
    font-size:0.68rem;
    color:var(--amber);
    letter-spacing:0.08em;
    text-transform:uppercase;
    margin-bottom:18px;
    background:var(--amber-dim);
    padding:5px 12px;
    border-radius:100px;
    align-self:flex-start;
  }
  .award-card h3{
    font-family:var(--display);
    font-size:1.55rem;
    font-weight:500;
    font-style:italic;
    margin-bottom:6px;
    line-height:1.2;
    color:var(--ink);
  }
  .award-org{
    font-family:var(--mono);
    font-size:0.74rem;
    color:var(--amber);
    margin-bottom:14px;
    display:block;
    letter-spacing:0.02em;
  }
  .award-card p{
    color:#C9C7BE;
    font-size:0.92rem;
    line-height:1.6;
    flex:1;
  }

  /* ---------- EDUCATION / LANGUAGES (SECTION 6) ---------- */
  .split{
    display:grid;
    grid-template-columns:1.3fr 1fr;
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
    border-radius:8px;
    overflow:hidden;
  }
  .info-card{background:var(--paper); padding:38px 34px;}
  .info-card h3{
    font-family:var(--display);
    font-weight:500;
    font-style:italic;
    font-size:1.2rem;
    margin-bottom:20px;
  }
  .edu-row{
    display:flex;
    justify-content:space-between;
    gap:16px;
    padding:16px 0;
    border-bottom:1px solid var(--line);
  }
  .edu-row:last-child{border-bottom:none; padding-bottom:0;}
  .edu-row:first-child{padding-top:0;}
  .edu-role{font-weight:600; font-size:0.94rem;}
  .edu-org{color:var(--muted); font-size:0.85rem; margin-top:3px;}
  .edu-date{font-family:var(--mono); font-size:0.7rem; color:var(--muted); white-space:nowrap;}
  .lang-list{display:flex; flex-direction:column; gap:18px;}
  .lang-row{display:flex; justify-content:space-between; align-items:center;}
  .lang-name{font-weight:600; font-size:0.94rem;}
  .lang-level{font-family:var(--mono); font-size:0.68rem; color:var(--amber);}
  .lang-bar{height:2px; background:var(--line); margin-top:8px; overflow:hidden;}
  .lang-bar i{display:block; height:100%; background:var(--amber);}

  /* ---------- CONTACT / FOOTER (SECTION 7) ---------- */
  footer{
    padding:130px 0 60px;
    border-top:1px solid var(--line);
    position:relative;
    width:100%;
  }
  .contact-panel{
    background:transparent;
    color:var(--ink);
    border:1px solid var(--line);
    border-radius:8px;
    padding:76px 56px;
    position:relative;
    overflow:hidden;
    text-align:center;
  }
  .contact-panel h2{
    font-family:var(--display);
    font-weight:500;
    font-style:italic;
    font-size:clamp(2.1rem, 5vw, 3.8rem);
    max-width:22ch;
    margin:0 auto 34px;
    position:relative;
    line-height:1.12;
  }
  .contact-links{
    display:flex;
    flex-wrap:wrap;
    gap:14px;
    position:relative;
    margin-bottom:48px;
    justify-content:center;
  }
  .contact-links a{
    font-family:var(--mono);
    font-size:0.76rem;
    letter-spacing:0.02em;
    border:1px solid var(--line);
    padding:12px 20px;
    border-radius:100px;
    transition:background .2s ease, border-color .2s ease, color .2s ease, transform .15s ease;
  }
  .contact-links a:hover{background:var(--ink); color:var(--paper); border-color:var(--ink); transform:translateY(-2px);}
  .contact-meta{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:28px;
    font-size:0.76rem;
    color:var(--muted);
    position:relative;
    border-top:1px solid var(--line);
    padding-top:28px;
    font-family:var(--mono);
  }
  .foot-bottom{
    text-align:center;
    margin-top:40px;
    font-family:var(--mono);
    font-size:0.7rem;
    color:var(--muted);
  }

  @media (max-width: 880px){
    .hero-grid{grid-template-columns:1fr;}
    .awards-grid{grid-template-columns:1fr;}
    .token-grid{grid-template-columns:1fr;}
    .work-grid{grid-template-columns:1fr 1fr;}
    .split{grid-template-columns:1fr;}
    nav.links{display:none;}
    .contact-panel{padding:54px 24px;}
    .tl-card{grid-template-columns:1fr; gap:12px;}
    .tl-date{grid-row:auto; padding-top:0;}
    .tl-products-grid{grid-template-columns:1fr;}
    section{padding:90px 0 80px;}
    footer{padding:90px 0 50px;}
  }
  @media (max-width: 560px){
    .wrap{padding:0 20px;}
    .nav-inner{padding:16px 20px;}
    .hero{padding:60px 0 45px;}
    section{padding:75px 0 65px;}
    footer{padding:75px 0 40px;}
    .work-grid{grid-template-columns:1fr;}
    html, body{cursor:auto;}
    * { cursor:auto; }
    #cursor-dot, #cursor-ring{display:none;}
  }
  @media (prefers-reduced-motion: reduce){
    *{animation-duration:0.001ms !important; transition-duration:0.001ms !important;}
  }
  @media (hover: none){
    html, body{cursor:auto;}
    * { cursor:auto; }
    #cursor-dot, #cursor-ring{display:none;}
  }

  /* ---------- ASK-ME WIDGET ---------- */
  #askme-fab{
    position:fixed; bottom:24px; right:24px; z-index:200;
    display:flex; align-items:center; gap:10px;
    background:var(--ink); color:var(--paper); border:none;
    padding:13px 20px 13px 16px; border-radius:100px; font-family:var(--body); font-weight:600; font-size:0.86rem;
    box-shadow:0 14px 34px -10px rgba(0,0,0,0.5); cursor:pointer;
    transition:transform .2s ease, box-shadow .2s ease;
  }
  #askme-fab:hover{transform:translateY(-3px); box-shadow:0 18px 40px -8px rgba(0,0,0,0.6);}
  .askme-fab-icon{font-size:1.1rem; line-height:1;}
  #askme-panel{
    position:fixed; bottom:24px; right:24px; z-index:201;
    width:min(400px, calc(100vw - 32px)); max-height:min(580px, calc(100vh - 48px));
    background:var(--panel); border:1px solid var(--line); border-radius:16px;
    box-shadow:0 30px 70px -20px rgba(0,0,0,0.6);
    display:flex; flex-direction:column; overflow:hidden;
    opacity:0; transform:translateY(16px) scale(0.98); pointer-events:none;
    transition:opacity .22s ease, transform .22s ease;
  }
  #askme-panel.open{opacity:1; transform:translateY(0) scale(1); pointer-events:auto;}
  .askme-head{
    display:flex; align-items:flex-start; justify-content:space-between; gap:10px;
    padding:16px 18px 14px; border-bottom:1px solid var(--line); background:rgba(255,255,255,0.02);
  }
  .askme-head strong{font-family:var(--display); font-size:1rem; display:block; font-style:italic;}
  .askme-head span{font-family:var(--mono); font-size:0.66rem; color:var(--muted); display:block; margin-top:2px;}
  #askme-close{
    background:none; border:none; color:var(--muted); font-size:1.1rem; cursor:pointer; padding:2px 6px; line-height:1;
    border-radius:6px; transition:color .15s ease, background .15s ease;
  }
  #askme-close:hover{color:var(--ink); background:var(--line);}
  .askme-thread{
    flex:1; overflow-y:auto; padding:16px 18px; display:flex; flex-direction:column; gap:12px; min-height:140px;
  }
  .askme-msg{
    max-width:90%; padding:11px 14px; border-radius:12px; font-size:0.83rem; line-height:1.5;
  }
  .askme-msg.bot{
    align-self:flex-start; background:var(--cobalt-dim, var(--paper)); border:1px solid var(--cobalt-border); border-bottom-left-radius:3px; color:var(--ink);
  }
  .askme-msg.user{
    align-self:flex-end; background:var(--cobalt); color:#fff; border-bottom-right-radius:3px; font-weight:500;
  }
  .askme-msg.bot .askme-tag{
    display:block; margin-top:6px; font-family:var(--mono); font-size:0.62rem; color:var(--amber); letter-spacing:0.04em; text-transform:uppercase;
  }
  .askme-chips{
    display:flex; flex-wrap:wrap; gap:6px; padding:0 18px 12px;
  }
  .askme-chips button{
    font-family:var(--mono); font-size:0.66rem; background:var(--paper); border:1px solid var(--line); color:var(--muted);
    padding:5px 10px; border-radius:100px; cursor:pointer; transition:border-color .15s ease, color .15s ease, background .15s ease;
  }
  .askme-chips button:hover{border-color:var(--cobalt); color:var(--ink); background:rgba(92,124,250,0.08);}
  .askme-form{
    display:flex; gap:8px; padding:12px 16px; border-top:1px solid var(--line); background:rgba(0,0,0,0.2);
  }
  #askme-input{
    flex:1; border:1px solid var(--line); background:var(--paper); color:var(--ink);
    padding:9px 14px; border-radius:100px; font-family:var(--body); font-size:0.83rem; outline:none;
    transition:border-color .2s ease;
  }
  #askme-input:focus{border-color:var(--cobalt);}
  .askme-form button[type="submit"]{
    width:36px; height:36px; border-radius:50%; background:var(--cobalt); color:#fff; border:none; cursor:pointer;
    font-size:0.95rem; flex-shrink:0; transition:transform .15s ease;
  }
  .askme-form button[type="submit"]:hover{transform:scale(1.05);}
  @media (max-width:560px){
    #askme-fab .askme-fab-text{display:none;}
    #askme-fab{padding:14px; border-radius:50%;}
    #askme-panel{right:16px; left:16px; width:auto; bottom:86px;}
  }

</style>
</head>
<body>

<div id="cursor-dot"></div>
<div id="cursor-ring"></div>

<header class="nav">
  <div class="nav-inner">
    <div class="nav-mark"><span class="dot"></span> Surya&nbsp;S&nbsp;J</div>
    <nav class="links">
      <a href="#expertise">Tools &amp; Skills</a>
      <a href="#work">Work</a>
      <a href="#experience">Experience</a>
      <a href="#awards">Awards</a>
      <a href="#education">Education</a>
      <a href="#contact">Contact</a>
    </nav>
    <div class="nav-actions">
      <a class="nav-resume-btn" href="surya-sj-resume.html" target="_blank" rel="noopener">📄 Resume ↓</a>
      <a class="nav-cta" href="https://wa.me/919600690255" target="_blank" rel="noopener">Say hello →</a>
    </div>
  </div>
</header>

<main>
  <!-- 1. HERO SECTION -->
  <section class="hero">
    <div class="wrap">
      <div class="hero-grid">
        <div>
          <div class="hero-id">
            <div class="hero-avatar-badge">
              <img src="surya-photo.jpg" alt="Surya S J — UI/UX Designer" class="hero-avatar-img">
              <span class="avatar-status" title="Open to UI/UX opportunities"></span>
            </div>
            <div class="hero-id-text">
              <strong>Surya S J</strong>
              <span>UI/UX Designer · Kanyakumari, TN</span>
            </div>
          </div>

          <div class="eyebrow">UI/UX &amp; Product Designer</div>
          <h1 class="headline">Crafting simple, scalable interfaces for <span class="accent">complex products.</span></h1>
          
          <p class="hero-sub">
            Award-winning UI/UX Designer with 3+ years crafting clean design systems, data‑rich dashboards, and intuitive SaaS experiences.
          </p>

          <div class="hero-actions">
            <a class="btn btn-primary" href="surya-sj-resume.html" target="_blank" rel="noopener">📄 Download Resume ↓</a>
            <a class="btn btn-ghost" href="#expertise">Tools &amp; Skills</a>
            <a class="btn btn-ghost" href="#work">Selected Work</a>
          </div>

          <div class="hero-meta">
            <span>📍 Kanyakumari, TN</span>
            <span>✆ +91 96006 90255</span>
            <span>in linkedin.com/in/surya-sj-019102264</span>
            <span>✉ suryajelon123@gmail.com</span>
          </div>
        </div>

        <!-- GAMIFIED HERO COMPONENT: DESIGN ARCADE & VIBE LAB -->
        <div class="arcade-card reveal">
          <div class="arcade-header">
            <div class="arcade-title-group">
              <span class="arcade-live-dot"></span>
              <span class="arcade-title">Playground · Arcade</span>
            </div>
            <div class="arcade-stats">
              <span class="stat-badge">⭐ <b id="player-xp">160</b> XP</span>
              <span class="stat-badge" id="player-level-badge">LVL 2: Creator</span>
            </div>
          </div>

          <!-- ARCADE TABS -->
          <div class="arcade-nav">
            <button class="arcade-tab-btn active" data-game="panel-catch">🕹️ Catch Spark</button>
            <button class="arcade-tab-btn" data-game="panel-balance">🎯 Pixel Eye</button>
            <button class="arcade-tab-btn" data-game="panel-like">❤️ Super Like</button>
          </div>

          <!-- GAME VIEWPORT -->
          <div class="arcade-viewport" id="arcade-viewport">
            
            <!-- MINI-GAME 1: CATCH THE SPARK -->
            <div class="game-panel active" id="panel-catch">
              <div id="game-arena">
                <div class="game-hud">
                  <span>⏱️ Time: <b id="game-time">10s</b></span>
                  <span>🔥 Streak: <b id="game-streak">0x</b></span>
                </div>
                
                <div class="arena-overlay" id="arena-start-screen">
                  <h4>Catch the Sparks!</h4>
                  <p>Tap moving design stars before time runs out to earn XP &amp; level up.</p>
                  <button class="play-start-btn" id="start-game-btn">Start Game ⚡</button>
                </div>
              </div>
            </div>

            <!-- MINI-GAME 2: PIXEL EYE & OPTICAL BALANCE -->
            <div class="game-panel" id="panel-balance">
              <div class="balance-game-wrap">
                <span style="font-family:var(--mono); font-size:0.68rem; color:var(--muted); text-transform:uppercase;">Optical Alignment Test</span>
                
                <div class="balance-stage">
                  <div class="target-zone" id="balance-target" title="Target Center">
                    <span style="font-size:0.65rem; color:var(--muted); font-family:var(--mono);">[CENTER]</span>
                  </div>
                  <div class="movable-orb" id="balance-orb" style="left:15%;">◆</div>
                </div>

                <div class="balance-slider-row">
                  <span style="font-family:var(--mono); font-size:0.65rem; color:var(--muted);">0%</span>
                  <input type="range" min="0" max="100" value="15" class="balance-slider" id="balance-range" aria-label="Align orb to center">
                  <span style="font-family:var(--mono); font-size:0.65rem; color:var(--muted);">100%</span>
                </div>
                
                <div class="balance-feedback" id="balance-msg">Adjust slider to hit exact center (50%)</div>
              </div>
            </div>

            <!-- MINI-GAME 3: SUPERCHARGED LIKE MACHINE -->
            <div class="game-panel" id="panel-like">
              <div class="like-machine-wrap" id="like-machine-container">
                <button class="like-machine-btn" id="super-like-btn" aria-label="Send appreciation with particle explosion">
                  <span style="font-size:1.2rem;">💖</span>
                  <span>Appreciate Portfolio</span>
                  <span style="font-family:var(--mono); font-size:0.8rem; background:rgba(0,0,0,0.25); padding:2px 8px; border-radius:100px;" id="super-like-count">164</span>
                </button>

                <div class="like-combo-badge">
                  <span>⚡ Combo Power: <b id="like-combo-num">x1</b></span>
                </div>
                
                <div class="achievement-pill" id="like-achievement">🏆 Unlocked: Creative Connoisseur</div>
              </div>
            </div>

          </div>

          <div class="arcade-footer">
            <span>🎮 Interactive Micro-Experience</span>
            <span>Surya S J · Design Lab</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- MARQUEE RIBBON (NEXT TO HERO SECTION) -->
  <div class="marquee" aria-hidden="true">
    <div class="marquee-track">
      <span><em>Tools</em>Figma · Adobe XD · Prototyping</span>
      <span><em>Design</em>Scalable Design Systems</span>
      <span><em>Experience</em>Enterprise SaaS &amp; Mobile</span>
      <span><em>Awards</em>People's Choice &amp; Rise and Shine</span>
      <span><em>Disciplines</em>UX Research · IA · Wireframing</span>
      <span><em>Tools</em>Figma · Adobe XD · Prototyping</span>
      <span><em>Design</em>Scalable Design Systems</span>
      <span><em>Experience</em>Enterprise SaaS &amp; Mobile</span>
      <span><em>Awards</em>People's Choice &amp; Rise and Shine</span>
      <span><em>Disciplines</em>UX Research · IA · Wireframing</span>
    </div>
  </div>

  <!-- 2. CORE EXPERTISE & TOOLS SECTION (COMES NEXT TO HERO) -->
  <section id="expertise">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">Core Expertise &amp; Tools</div>
        <h2>Disciplines, Tools &amp; Methods</h2>
        <p class="section-sub">A focused toolkit applied across UX research, design systems, and rapid prototyping.</p>
      </div>
      <div class="token-grid">
        <div class="token-card reveal">
          <div class="swatch"></div>
          <h3>UX &amp; Product Design</h3>
          <div class="pill-row">
            <span class="pill">UX Research</span>
            <span class="pill">Usability Testing</span>
            <span class="pill">Information Architecture</span>
            <span class="pill">User Flows</span>
            <span class="pill">Wireframing</span>
            <span class="pill">Prototyping</span>
            <span class="pill">Design Systems</span>
            <span class="pill">User Stories</span>
            <span class="pill">PRDs &amp; Specs</span>
          </div>
        </div>
        <div class="token-card reveal">
          <div class="swatch"></div>
          <h3>AI &amp; Emerging Tech</h3>
          <div class="pill-row">
            <span class="pill">AI-Assisted Design</span>
            <span class="pill">Conversational UI</span>
            <span class="pill">Natural Language Dashboards</span>
            <span class="pill">Prompt Engineering</span>
            <span class="pill">Rapid Prototyping</span>
            <span class="pill">Decision Science UX</span>
          </div>
        </div>
        <div class="token-card reveal">
          <div class="swatch"></div>
          <h3>Tools &amp; Platforms</h3>
          <div class="pill-row">
            <span class="pill">Figma</span>
            <span class="pill">Adobe XD</span>
            <span class="pill">Photoshop</span>
            <span class="pill">Illustrator</span>
            <span class="pill">Lovable</span>
            <span class="pill">Replit</span>
            <span class="pill">Antigravity</span>
            <span class="pill">ChatGPT</span>
            <span class="pill">Claude</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 3. SELECTED WORK -->
  <section id="work">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">Selected Work</div>
        <h2>Curated Case Studies &amp; Shipped Screens</h2>
        <p class="section-sub">A curated selection of product design, enterprise dashboards, and mobile UI kits from the Behance archive.</p>
      </div>

      <div class="work-grid">
        <a class="work-card reveal" href="https://www.behance.net/gallery/254318179/MentorMaster-Professional-Mentorship-Platform" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/029144254318179.Y3JvcCwxMTUwLDkwMCwyNSww.png" alt="MentorMaster — Professional Mentorship Platform screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Product Design</span>
            <h3>MentorMaster</h3>
            <p>Professional mentorship platform</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/253320589/Enterprise-Admin-Dashboard" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/323f02253320589.Y3JvcCwxMzA5LDEwMjQsNjQsMA.png" alt="Enterprise Admin Dashboard screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Product Design</span>
            <h3>Enterprise Admin Dashboard</h3>
            <p>Data-dense admin console UI</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/212361019/Medicare-Web-application-Dashboard(Mockup)" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/f18170212361019.Y3JvcCwxNDY4LDExNDksNDMsMA.png" alt="Medicare web application dashboard mockup" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Healthcare</span>
            <h3>Medicare Dashboard</h3>
            <p>Web application dashboard mockup</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/212360523/Healthcare-Web-Application-Dashboard" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/cbdad5212360523.Y3JvcCwxNDY4LDExNDksNDMsMA.png" alt="Healthcare web application dashboard screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Healthcare</span>
            <h3>Healthcare Web App</h3>
            <p>Dashboard for a healthcare platform</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/180698595/Case-study-Event-planning-Mobile-application" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/8de4b9180698595.Y3JvcCwxMjc0LDk5NywzMSww.png" alt="Event planning mobile application case study" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Case Study · Mobile</span>
            <h3>Event Planning App</h3>
            <p>End-to-end mobile case study</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/180049227/UI-kit-Event-planning-mobile-app" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/1964c7180049227.Y3JvcCwxMzY2LDEwNjgsMCww.png" alt="UI kit for event planning mobile app" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">UI Kit · Mobile</span>
            <h3>Event Planning UI Kit</h3>
            <p>Componentized mobile UI kit</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/183721341/DESIGNERS-MOBILE-APPLICATION-Learning-app-design" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/1bc716183721341.Y3JvcCw4MDgsNjMyLDAsMA.png" alt="Designer's mobile learning app design" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Mobile · EdTech</span>
            <h3>Designer's Learning App</h3>
            <p>Mobile application for learning design</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/218393235/ASO-Website-Design" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/0fad62218393235.Y3JvcCwxNDQwLDExMjYsMCww.png" alt="ASO website design screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Web Design</span>
            <h3>ASO Website</h3>
            <p>Marketing website design</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/216277189/Designers-Platform-Website-Design" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/4aa2ae216277189.Y3JvcCwxNDQwLDExMjYsMCww.png" alt="Designers Platform website design screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Web Design</span>
            <h3>Designers Platform</h3>
            <p>Website design for a design community</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/179468661/Food-ordering-website" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/d3dbea179468661.Y3JvcCwxMzY2LDEwNjgsMCww.png" alt="Food ordering website screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Web Design</span>
            <h3>Food Ordering Website</h3>
            <p>End-to-end ordering flow</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/212886465/Hotel-Website-Mockup" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/004b60212886465.Y3JvcCwxNDY4LDExNDksNDMsMA.png" alt="Hotel website mockup screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Web Design</span>
            <h3>Hotel Website — Mockup</h3>
            <p>Booking-focused hospitality site</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>

        <a class="work-card reveal" href="https://www.behance.net/gallery/212885597/Hotel-Website" target="_blank" rel="noopener">
          <div class="work-thumb"><img src="https://mir-s3-cdn-cf.behance.net/projects/404/3ddd1d212885597.Y3JvcCwxNDQwLDExMjYsMCww.png" alt="Hotel website screens" loading="lazy"></div>
          <div class="work-info">
            <span class="work-tag">Web Design</span>
            <h3>Hotel Website</h3>
            <p>Hospitality brand website</p>
          </div>
          <span class="work-arrow">↗</span>
        </a>
      </div>

      <div class="work-cta-row reveal">
        <a class="btn btn-ghost" href="https://www.behance.net/srysj1" target="_blank" rel="noopener">View All 12+ Projects on Behance ↗</a>
      </div>
    </div>
  </section>

  <!-- 4. EXPERIENCE SECTION -->
  <section id="experience">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">Work Experience</div>
        <h2>3+ Years in Product Design &amp; SaaS Systems</h2>
        <p class="section-sub">Leading end-to-end product design across EdTech, Healthcare, and scalable enterprise platforms.</p>
      </div>

      <div class="timeline">
        <!-- 1. SHIKSHALOKAM -->
        <div class="tl-item current reveal">
          <div class="tl-card">
            <div class="tl-date">Jul 2025 — Present</div>
            <div class="tl-role">
              Associate UI/UX Designer
              <span>ShikshaLokam · Full-time</span>
            </div>
            <div class="tl-tags">
              <span>Mitra (Conversational AI)</span>
              <span>Mitra Dashboard</span>
              <span>Elevate Platform</span>
              <span>Design Systems</span>
            </div>

            <div class="tl-products-box">
              <span class="tl-products-title">Core Products &amp; Platforms</span>
              <div class="tl-products-grid">
                <div class="tl-product-item">
                  <strong>Mitra (Conversational Platform)</strong>
                  <p>Conversational interface streamlining field data collection, surveys, and multi-state educational observations.</p>
                </div>
                <div class="tl-product-item">
                  <strong>Mitra Analytics Dashboard</strong>
                  <p>Analytics suite delivering real-time block and district performance metrics for decision-makers.</p>
                </div>
                <div class="tl-product-item">
                  <strong>Elevate Platform</strong>
                  <p>Project-based learning and mentoring workflows for statewide teacher development programs.</p>
                </div>
                <div class="tl-product-item">
                  <strong>PoC Prototype Studio</strong>
                  <p>Rapid AI-assisted prototypes validating natural-language query flows with stakeholders.</p>
                </div>
              </div>
            </div>

            <ul class="tl-list">
              <li><b>AI Product Design</b> — Led end-to-end UI/UX for <b>Mitra</b>, designing intuitive conversational flows, voice inputs, and contextual prompt suggestions.</li>
              <li><b>Workflow Optimization</b> — Streamlined survey and assessment journeys on <b>Elevate</b>, reducing friction for state-level field observations.</li>
              <li><b>Design Systems &amp; Tokens</b> — Created reusable Figma component libraries, interaction states, and structured developer handoff specs.</li>
              <li><b>Peer Recognition</b> — Honored with both the <b>Rise and Shine Award (2026)</b> and <b>People's Choice Award (2025)</b> for design excellence.</li>
            </ul>
          </div>
        </div>

        <!-- 2. SMARTAIL PVT LTD -->
        <div class="tl-item reveal">
          <div class="tl-card">
            <div class="tl-date">2024 — 2025</div>
            <div class="tl-role">
              UI/UX Designer
              <span>Smartail Pvt. Ltd · Full-time</span>
            </div>
            <div class="tl-tags">
              <span>DeepGrade</span>
              <span>DeepPrep</span>
              <span>DeepGrade Analytics</span>
              <span>DeepCue</span>
              <span>Healthcare SaaS</span>
            </div>

            <div class="tl-products-box">
              <span class="tl-products-title">Core Smartail Products Designed</span>
              <div class="tl-products-grid">
                <div class="tl-product-item">
                  <strong>DeepGrade (AI Assessment)</strong>
                  <p>Automated evaluation platform for handwritten and digital student exams.</p>
                </div>
                <div class="tl-product-item">
                  <strong>DeepGrade Analytics</strong>
                  <p>Decision-science dashboard identifying learning gaps and cohort performance.</p>
                </div>
                <div class="tl-product-item">
                  <strong>DeepPrep (Exam Preparation)</strong>
                  <p>Adaptive test generation platform tailored for CBSE Class X and competitive boards.</p>
                </div>
                <div class="tl-product-item">
                  <strong>DeepCue (Remedial Flashcards)</strong>
                  <p>Personalized flashcard solution for self-paced student gap revision.</p>
                </div>
              </div>
            </div>

            <ul class="tl-list">
              <li><b>Assessment &amp; Analytics UX</b> — Designed evaluation workspaces and annotation tools for <b>DeepGrade</b>, speeding up grading turnaround times.</li>
              <li><b>Dashboard Visualization</b> — Architected academic performance dashboards in <b>DeepGrade Analytics</b>, turning raw scores into clear cohort insights.</li>
              <li><b>Healthcare SaaS Design</b> — Created accessible patient-provider dashboards and diagnostic portals across B2B/B2C healthcare applications.</li>
              <li><b>User Research</b> — Ran usability testing and stakeholder interviews to validate design decisions prior to engineering sprints.</li>
            </ul>
          </div>
        </div>

        <!-- 3. SMARTAIL INTERNSHIP -->
        <div class="tl-item reveal">
          <div class="tl-card">
            <div class="tl-date">2023 — 2024</div>
            <div class="tl-role">
              UI/UX Design Intern
              <span>Smartail Pvt. Ltd · Internship</span>
            </div>
            <div class="tl-tags">
              <span>Design Systems</span>
              <span>Figma Tokens</span>
              <span>Wireframing</span>
              <span>Design QA</span>
            </div>
            <ul class="tl-list">
              <li><b>Design System Upkeep</b> — Maintained scalable UI kits and typography/color tokens across Smartail's web applications.</li>
              <li><b>Exploration &amp; Wireframes</b> — Supported senior designers with responsive layouts, micro-interactions, and user flow documentation.</li>
              <li><b>Design QA</b> — Conducted pixel-level visual QA audits on live staging builds to ensure high-fidelity implementation.</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 5. AWARDS & HONORS SECTION -->
  <section id="awards">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">Honors &amp; Recognition</div>
        <h2>Awards Earned for Impact &amp; Team Excellence</h2>
        <p class="section-sub">Recognition for cross-functional collaboration, design speed, and user advocacy.</p>
      </div>

      <div class="awards-grid">
        <!-- AWARD 1: PEOPLE'S CHOICE -->
        <div class="award-card reveal">
          <div class="award-badge-top">🏆 Peer-Voted Award</div>
          <h3>People's Choice Award</h3>
          <span class="award-org">ShikshaLokam · 2025</span>
          <p>Voted by cross-functional team members across engineering, product, and leadership for design empathy, collaborative spirit, and commitment to building user-centric interfaces.</p>
        </div>

        <!-- AWARD 2: RISE AND SHINE -->
        <div class="award-card reveal">
          <div class="award-badge-top">🌟 Excellence &amp; Impact</div>
          <h3>Rise and Shine Award</h3>
          <span class="award-org">ShikshaLokam · 2026</span>
          <p>Awarded for high-velocity execution, product ownership, and leading key UI/UX architecture and interactive prototyping milestones.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- 6. EDUCATION & LANGUAGES -->
  <section id="education">
    <div class="wrap">
      <div class="section-head reveal">
        <div class="eyebrow">Education &amp; Languages</div>
        <h2>Credentials &amp; Language Proficiency</h2>
        <p class="section-sub">Engineering fundamentals combined with professional design training.</p>
      </div>
      <div class="split">
        <div class="info-card reveal">
          <h3>Education &amp; Credentials</h3>
          <div class="edu-row">
            <div>
              <div class="edu-role">UI/UX Design Professional Certification</div>
              <div class="edu-org">Image Creative Education</div>
            </div>
            <div class="edu-date">2022 — 2023</div>
          </div>
          <div class="edu-row">
            <div>
              <div class="edu-role">B.E. in Mechatronics Engineering</div>
              <div class="edu-org">Coimbatore Institute of Engineering and Technology (CIET)</div>
            </div>
            <div class="edu-date">2017 — 2021</div>
          </div>
        </div>
        <div class="info-card reveal">
          <h3>Languages</h3>
          <div class="lang-list">
            <div>
              <div class="lang-row"><span class="lang-name">Tamil</span><span class="lang-level">Native</span></div>
              <div class="lang-bar"><i style="width:100%"></i></div>
            </div>
            <div>
              <div class="lang-row"><span class="lang-name">English</span><span class="lang-level">Professional Working</span></div>
              <div class="lang-bar"><i style="width:90%"></i></div>
            </div>
            <div>
              <div class="lang-row"><span class="lang-name">Malayalam</span><span class="lang-level">Conversational</span></div>
              <div class="lang-bar"><i style="width:65%"></i></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 7. FOOTER & CONTACT -->
  <footer id="contact">
    <div class="wrap">
      <div class="contact-panel reveal">
        <div class="eyebrow" style="color:var(--amber); justify-content:center;">Get In Touch</div>
        <h2>Let's design seamless user experiences &amp; intuitive interfaces together.</h2>
        <div class="contact-links">
          <a href="surya-sj-resume.html" target="_blank" rel="noopener" style="background:var(--ink); color:var(--paper); font-weight:600; border-color:var(--ink);">📄 Download Resume (PDF) ↓</a>
          <a href="mailto:suryajelon123@gmail.com">suryajelon123@gmail.com</a>
          <a href="https://wa.me/919600690255" target="_blank" rel="noopener">WhatsApp Chat ↗</a>
          <a href="tel:9600690255">+91 96006 90255</a>
          <a href="https://linkedin.com/in/surya-sj-019102264" target="_blank" rel="noopener">LinkedIn Profile ↗</a>
          <a href="https://behance.net/srysj1" target="_blank" rel="noopener">Behance Portfolio ↗</a>
        </div>
        <div class="contact-meta">
          <span>📍 Based in Kanyakumari, Tamil Nadu, India</span>
          <span>✦ Open to Full-time, Hybrid &amp; Remote Design Roles</span>
        </div>
      </div>
      <div class="foot-bottom">© 2026 Surya S J — UI/UX Designer. Designed with clarity &amp; craft.</div>
    </div>
  </footer>
</main>

<!-- ASK-ME WIDGET START -->
<button id="askme-fab" aria-label="Ask a question about Surya" aria-expanded="false">
  <span class="askme-fab-icon">💬</span><span class="askme-fab-text">Ask about Surya</span>
</button>

<div id="askme-panel" role="dialog" aria-label="Interactive Q&A about Surya S J" aria-hidden="true">
  <div class="askme-head">
    <div>
      <strong>Ask about Surya</strong>
      <span>Interactive Assistant · Answers from portfolio data</span>
    </div>
    <button id="askme-close" aria-label="Close dialog">✕</button>
  </div>
  <div id="askme-thread" class="askme-thread">
    <div class="askme-msg bot">Hi! I can answer questions about Surya's design experience at <b>ShikshaLokam</b> and <b>Smartail</b>, his <b>awards</b>, skills, tools, or how to download his <b>resume</b>!</div>
  </div>
  <div class="askme-chips" id="askme-chips">
    <button data-q="How can I download your resume?">📄 Download Resume</button>
    <button data-q="What tools and design skills do you use?">🛠️ Tools &amp; skills?</button>
    <button data-q="What awards have you received?">🏆 Awards won?</button>
    <button data-q="Tell me about your work experience">🏢 Work experience?</button>
    <button data-q="How can I contact you?">✉️ Contact info?</button>
  </div>
  <form id="askme-form" class="askme-form">
    <input id="askme-input" type="text" autocomplete="off" placeholder="Ask about experience, awards, stack…" aria-label="Type your question">
    <button type="submit" aria-label="Send question">↑</button>
  </form>
</div>
<!-- ASK-ME WIDGET END -->


<script>
  /* =========================================================
     GAMIFIED ARCADE & PLAYGROUND ENGINE
  ========================================================= */

  // Global Player State
  let playerXP = parseInt(localStorage.getItem('surya_player_xp') || '160', 10);
  let totalLikes = parseInt(localStorage.getItem('surya_portfolio_likes') || '164', 10);
  let likeCombo = 1;
  let likeComboTimer = null;

  function updatePlayerLevel() {
    const xpEl = document.getElementById('player-xp');
    const lvlBadge = document.getElementById('player-level-badge');
    if (xpEl) xpEl.textContent = playerXP;
    
    let levelName = 'LVL 1: Scout';
    if (playerXP >= 500) levelName = 'LVL 5: UX Grandmaster 👑';
    else if (playerXP >= 350) levelName = 'LVL 4: Design Boss 🏆';
    else if (playerXP >= 220) levelName = 'LVL 3: Architect ⭐';
    else if (playerXP >= 100) levelName = 'LVL 2: Creator ✨';
    
    if (lvlBadge) lvlBadge.textContent = levelName;
    localStorage.setItem('surya_player_xp', playerXP.toString());
  }
  updatePlayerLevel();

  // 1. ARCADE TAB NAVIGATION
  const gameTabs = document.querySelectorAll('.arcade-tab-btn');
  const gamePanels = document.querySelectorAll('.game-panel');
  gameTabs.forEach(btn => {
    btn.addEventListener('click', () => {
      gameTabs.forEach(b => b.classList.remove('active'));
      gamePanels.forEach(p => p.classList.remove('active'));
      btn.classList.add('active');
      const targetGame = btn.getAttribute('data-game');
      const panel = document.getElementById(targetGame);
      if (panel) panel.classList.add('active');
    });
  });

  // 2. MINI-GAME 1: CATCH THE SPARK (TARGET SPAWNER)
  const startBtn = document.getElementById('start-game-btn');
  const arena = document.getElementById('game-arena');
  const startScreen = document.getElementById('arena-start-screen');
  const timeDisplay = document.getElementById('game-time');
  const streakDisplay = document.getElementById('game-streak');

  let gameInterval = null;
  let spawnInterval = null;
  let timeLeft = 10;
  let currentStreak = 0;

  const sparkIcons = ['⭐', '💎', '🎨', '✨', '⚡', '🚀', '🔥'];
  const sparkColors = ['#5C7CFA', '#D9CBA3', '#10B981', '#F43F5E', '#A855F7'];

  function spawnSpark() {
    if (!arena) return;
    const orb = document.createElement('div');
    orb.className = 'spark-target';
    const randIcon = sparkIcons[Math.floor(Math.random() * sparkIcons.length)];
    const randColor = sparkColors[Math.floor(Math.random() * sparkColors.length)];
    orb.textContent = randIcon;
    orb.style.color = randColor;
    orb.style.background = randColor + '22';
    orb.style.border = `1.5px solid ${randColor}`;

    const maxX = arena.clientWidth - 46;
    const maxY = arena.clientHeight - 46;
    orb.style.left = Math.max(10, Math.floor(Math.random() * maxX)) + 'px';
    orb.style.top = Math.max(28, Math.floor(Math.random() * maxY)) + 'px';

    orb.addEventListener('click', (e) => {
      e.stopPropagation();
      currentStreak++;
      playerXP += 25 * currentStreak;
      streakDisplay.textContent = currentStreak + 'x';
      updatePlayerLevel();
      spawnFloatingSparkle(orb, `+${25 * currentStreak} XP!`, randColor);
      orb.remove();
    });

    arena.appendChild(orb);
    setTimeout(() => {
      if (orb.parentNode) orb.remove();
    }, 2400);
  }

  if (startBtn) {
    startBtn.addEventListener('click', () => {
      startScreen.style.display = 'none';
      timeLeft = 10;
      currentStreak = 0;
      streakDisplay.textContent = '0x';
      timeDisplay.textContent = '10s';

      // Clear any remaining orbs
      document.querySelectorAll('.spark-target').forEach(o => o.remove());

      spawnInterval = setInterval(spawnSpark, 650);
      spawnSpark();

      gameInterval = setInterval(() => {
        timeLeft--;
        timeDisplay.textContent = timeLeft + 's';
        if (timeLeft <= 0) {
          clearInterval(gameInterval);
          clearInterval(spawnInterval);
          document.querySelectorAll('.spark-target').forEach(o => o.remove());
          startScreen.style.display = 'flex';
          startScreen.querySelector('h4').textContent = '🎉 Game Finished!';
          startScreen.querySelector('p').innerHTML = `You leveled up to <b>${playerXP} XP</b>! Streak reached: <b>${currentStreak}x</b>.`;
          startBtn.textContent = 'Play Again ⚡';
        }
      }, 1000);
    });
  }

  // 3. MINI-GAME 2: OPTICAL PIXEL BALANCE
  const balanceRange = document.getElementById('balance-range');
  const balanceOrb = document.getElementById('balance-orb');
  const balanceTarget = document.getElementById('balance-target');
  const balanceMsg = document.getElementById('balance-msg');

  if (balanceRange && balanceOrb) {
    balanceRange.addEventListener('input', (e) => {
      const val = parseInt(e.target.value, 10);
      balanceOrb.style.left = `calc(${val}% - 16px)`;

      // Check optical alignment threshold
      if (val >= 48 && val <= 52) {
        balanceTarget.classList.add('locked');
        balanceOrb.style.background = '#10B981';
        balanceMsg.innerHTML = '🎯 <b>100% Optical Perfection!</b> (+50 XP)';
        balanceMsg.style.color = '#10B981';
        playerXP += 5;
        updatePlayerLevel();
      } else {
        balanceTarget.classList.remove('locked');
        balanceOrb.style.background = 'var(--cobalt)';
        const diff = Math.abs(50 - val);
        balanceMsg.textContent = `Off by ${diff}px — Keep adjusting!`;
        balanceMsg.style.color = 'var(--amber)';
      }
    });
  }

  // 4. MINI-GAME 3: SUPERCHARGED LIKE MACHINE
  const superLikeBtn = document.getElementById('super-like-btn');
  const superLikeCount = document.getElementById('super-like-count');
  const likeComboNum = document.getElementById('like-combo-num');
  const likeAchievement = document.getElementById('like-achievement');

  if (superLikeCount) superLikeCount.textContent = totalLikes;

  function spawnFloatingSparkle(originElem, customText, customColor) {
    const rect = originElem.getBoundingClientRect();
    const sparkle = document.createElement('div');
    sparkle.className = 'floating-sparkle';
    sparkle.textContent = customText || (Math.random() > 0.5 ? '💖' : '✨');
    if (customColor) sparkle.style.color = customColor;

    const dx = (Math.random() - 0.5) * 120 + 'px';
    const dy = -(Math.random() * 80 + 40) + 'px';
    const dr = (Math.random() - 0.5) * 60 + 'deg';
    sparkle.style.setProperty('--dx', dx);
    sparkle.style.setProperty('--dy', dy);
    sparkle.style.setProperty('--dr', dr);
    sparkle.style.left = (rect.left + rect.width / 2 - 12) + 'px';
    sparkle.style.top = (rect.top + window.scrollY - 10) + 'px';

    document.body.appendChild(sparkle);
    setTimeout(() => sparkle.remove(), 1200);
  }

  if (superLikeBtn) {
    superLikeBtn.addEventListener('click', (e) => {
      totalLikes++;
      playerXP += 10 * likeCombo;
      localStorage.setItem('surya_portfolio_likes', totalLikes.toString());
      superLikeCount.textContent = totalLikes;
      updatePlayerLevel();

      // Combo System
      likeCombo = Math.min(likeCombo + 1, 8);
      likeComboNum.textContent = `x${likeCombo} MEGA!`;
      clearTimeout(likeComboTimer);
      likeComboTimer = setTimeout(() => {
        likeCombo = 1;
        likeComboNum.textContent = 'x1';
      }, 1800);

      // Achievements
      if (totalLikes % 5 === 0) {
        likeAchievement.textContent = '🌟 Legendary Patron Achievement Unlocked!';
        likeAchievement.style.color = 'var(--amber)';
      }

      // Burst 3 sparkles per click
      spawnFloatingSparkle(superLikeBtn);
      setTimeout(() => spawnFloatingSparkle(superLikeBtn), 80);
      setTimeout(() => spawnFloatingSparkle(superLikeBtn), 160);
    });
  }

  // 5. Custom dual-ring cursor
  const cDot = document.getElementById('cursor-dot');
  const cRing = document.getElementById('cursor-ring');
  const hasFinePointer = window.matchMedia('(hover:hover) and (pointer:fine)').matches;
  const reduceMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  if (cDot && cRing && hasFinePointer && !reduceMotion) {
    let mx = 0, my = 0, rx = 0, ry = 0;
    window.addEventListener('mousemove', (e)=>{
      mx = e.clientX; my = e.clientY;
      cDot.style.left = mx + 'px'; cDot.style.top = my + 'px';
    });
    function ringLoop(){
      rx += (mx - rx) * 0.18; ry += (my - ry) * 0.18;
      cRing.style.left = rx + 'px'; cRing.style.top = ry + 'px';
      requestAnimationFrame(ringLoop);
    }
    ringLoop();
    document.querySelectorAll('a, button, input').forEach(elem=>{
      elem.addEventListener('mouseenter', ()=>{ cRing.style.width='54px'; cRing.style.height='54px'; cRing.style.opacity='0.9'; cRing.style.borderColor='var(--cobalt)'; });
      elem.addEventListener('mouseleave', ()=>{ cRing.style.width='34px'; cRing.style.height='34px'; cRing.style.opacity='0.6'; cRing.style.borderColor='var(--amber)'; });
    });
  } else if (cDot && cRing) {
    cDot.style.display = 'none'; cRing.style.display = 'none';
  }

  // 6. Scroll reveal
  const revealEls = document.querySelectorAll('.reveal');
  if ('IntersectionObserver' in window && !reduceMotion) {
    const io = new IntersectionObserver((entries)=>{
      entries.forEach(entry=>{
        if(entry.isIntersecting){ entry.target.classList.add('in'); io.unobserve(entry.target); }
      });
    }, {threshold:0.08});
    revealEls.forEach(elem=>io.observe(elem));
  } else {
    revealEls.forEach(elem=>elem.classList.add('in'));
  }
</script>

<script>
  /* ---------- LOCAL Q&A ENGINE ---------- */
  (function(){
    const KB = [
      {
        tags: ["resume", "cv", "download resume", "pdf", "curriculum vitae", "download"],
        a: "You can view, print, or download Surya's complete resume as a PDF here:\n\n👉 <a href='surya-sj-resume.html' target='_blank' style='color:var(--cobalt); font-weight:600; text-decoration:underline;'>📄 Open &amp; Download Surya S J — Resume (PDF / Print-Ready)</a>",
        src: "Resume Document"
      },
      {
        tags: ["tools", "software", "figma", "stack", "skills", "photoshop", "illustrator", "lovable", "replit"],
        a: "Surya's tools & skills:\n• <b>Design Tools:</b> Figma, Adobe XD, Photoshop, Illustrator.\n• <b>Core Methods:</b> UX Research, Usability Testing, Information Architecture, Wireframing, Design Tokens, User Stories.\n• <b>AI & Prototyping:</b> Lovable, Replit, Antigravity, ChatGPT, Claude.",
        src: "Core Expertise & Tools"
      },
      {
        tags: ["award", "awards", "recognition", "honors", "people choice", "rise and shine", "prize", "achievement"],
        a: "Surya has won two prestigious awards at ShikshaLokam:\n\n1. 🏆 <b>People's Choice Award (2025)</b> — Peer-voted across engineering, product, and leadership for design empathy and collaboration.\n2. 🌟 <b>Rise and Shine Award (2026)</b> — Conferred for execution speed, ownership, and leading critical design milestones.",
        src: "Honors & Recognition"
      },
      {
        tags: ["experience", "career", "shikshalokam", "smartail", "work", "role"],
        a: "Surya has 3+ years of experience in UI/UX & product design:\n• <b>Associate UI/UX Designer at ShikshaLokam</b> (Jul 2025–Present): Leading UI/UX for Mitra, Elevate platform, and design systems.\n• <b>UI/UX Designer at Smartail</b> (2024–2025): Designed DeepGrade, DeepPrep, DeepCue, and healthcare SaaS applications.\n• <b>UI/UX Design Intern at Smartail</b> (2023–2024): Maintained design systems and conducted design QA.",
        src: "Experience Overview"
      },
      {
        tags: ["smartail", "smartail products", "deepgrade", "deepprep", "deepcue", "analytics"],
        a: "At Smartail, Surya designed key products:\n• <b>DeepGrade</b>: Automated grading platform for handwritten and digital student exams.\n• <b>DeepGrade Analytics</b>: Cohort diagnostic decision-science dashboard.\n• <b>DeepPrep</b>: AI test preparation platform (CBSE Class X).\n• <b>DeepCue</b>: Personalized remedial flashcard system.",
        src: "Experience — Smartail"
      },
      {
        tags: ["bio", "who", "about", "surya", "intro", "summary", "background"],
        a: "<b>Surya S J</b> is an award-winning UI/UX Designer with 3+ years of experience across EdTech, Healthcare SaaS, and Enterprise Dashboards. He specializes in user research, design systems, and crafting clean, accessible digital products.",
        src: "Profile Overview"
      },
      {
        tags: ["education", "degree", "college", "university", "mechatronics", "image creative"],
        a: "Surya holds a <b>B.E. in Mechatronics Engineering</b> from Coimbatore Institute of Engineering and Technology (CIET, 2017–2021) and a <b>Professional UI/UX Design Certification</b> from Image Creative Education (2022–2023).",
        src: "Education & Credentials"
      },
      {
        tags: ["contact", "email", "phone", "whatsapp", "hire", "linkedin", "behance", "reach"],
        a: "You can reach Surya directly:\n• <b>Email:</b> <a href='mailto:suryajelon123@gmail.com' style='color:var(--cobalt); text-decoration:underline;'>suryajelon123@gmail.com</a>\n• <b>WhatsApp / Phone:</b> <a href='https://wa.me/919600690255' target='_blank' style='color:var(--cobalt); text-decoration:underline;'>+91 96006 90255</a>\n• <b>LinkedIn:</b> <a href='https://linkedin.com/in/surya-sj-019102264' target='_blank' style='color:var(--cobalt); text-decoration:underline;'>linkedin.com/in/surya-sj-019102264</a>\n• <b>Behance:</b> <a href='https://behance.net/srysj1' target='_blank' style='color:var(--cobalt); text-decoration:underline;'>behance.net/srysj1</a>",
        src: "Contact Information"
      },
      {
        tags: ["projects", "behance", "portfolio", "case study", "mentormaster", "medicare"],
        a: "Surya's Behance portfolio (<a href='https://behance.net/srysj1' target='_blank' style='color:var(--cobalt); text-decoration:underline;'>behance.net/srysj1</a>) features 12+ case studies including MentorMaster, Enterprise Admin Dashboard, Medicare Web App, Event Planning UI Kit, and ASO websites.",
        src: "Selected Work — Behance"
      },
      {
        tags: ["location", "city", "kanyakumari", "tamil nadu", "remote"],
        a: "Surya is based in <b>Kanyakumari, Tamil Nadu, India</b>, and is open to full-time, hybrid, and remote UI/UX & Product Design roles.",
        src: "Profile Location"
      }
    ];

    function normalize(s){
      return s.toLowerCase().replace(/[^\w\s]/g,' ').split(/\s+/).filter(Boolean);
    }

    function bestMatch(question){
      const words = normalize(question);
      if(!words.length) return null;
      let best = null, bestScore = 0;

      KB.forEach(entry=>{
        let score = 0;
        entry.tags.forEach(tag=>{
          const tagWords = tag.split(' ');
          if(question.toLowerCase().includes(tag)) score += 3;
          tagWords.forEach(tw=>{
            if(words.includes(tw)) score += 1.5;
            else if(words.some(w => w.length > 3 && (w.includes(tw) || tw.includes(w)))) score += 0.75;
          });
        });
        if(score > bestScore){
          bestScore = score;
          best = entry;
        }
      });
      return bestScore >= 1 ? best : null;
    }

    const fab = document.getElementById('askme-fab');
    const panel = document.getElementById('askme-panel');
    const closeBtn = document.getElementById('askme-close');
    const thread = document.getElementById('askme-thread');
    const form = document.getElementById('askme-form');
    const input = document.getElementById('askme-input');
    const chips = document.getElementById('askme-chips');
    if(!fab || !panel) return;

    function openPanel(){
      panel.classList.add('open');
      panel.setAttribute('aria-hidden','false');
      fab.setAttribute('aria-expanded','true');
      setTimeout(()=>input && input.focus(), 150);
    }
    function closePanel(){
      panel.classList.remove('open');
      panel.setAttribute('aria-hidden','true');
      fab.setAttribute('aria-expanded','false');
    }
    fab.addEventListener('click', ()=>{
      panel.classList.contains('open') ? closePanel() : openPanel();
    });
    closeBtn.addEventListener('click', closePanel);
    document.addEventListener('keydown', (e)=>{ if(e.key === 'Escape') closePanel(); });

    function addMsg(text, who, tag){
      const div = document.createElement('div');
      div.className = 'askme-msg ' + who;
      div.innerHTML = text.replace(/\n/g, '<br>');
      if(tag){
        const t = document.createElement('span');
        t.className = 'askme-tag';
        t.textContent = 'Source: ' + tag;
        div.appendChild(t);
      }
      thread.appendChild(div);
      thread.scrollTop = thread.scrollHeight;
    }

    function ask(q){
      if(!q || !q.trim()) return;
      addMsg(q, 'user');
      const match = bestMatch(q);
      setTimeout(()=>{
        if(match){
          addMsg(match.a, 'bot', match.src);
        } else {
          addMsg("I couldn't find an exact match for that question. You can ask me about Surya's <b>Tools & Skills</b>, his <b>Awards (People's Choice, Rise and Shine)</b>, his <b>Work Experience</b>, or how to <b>Download his Resume</b>.", 'bot');
        }
      }, 220);
    }

    form.addEventListener('submit', (e)=>{
      e.preventDefault();
      const q = input.value;
      input.value = '';
      ask(q);
    });

    chips.addEventListener('click', (e)=>{
      const btn = e.target.closest('button[data-q]');
      if(btn) ask(btn.getAttribute('data-q'));
    });
  })();
</script>
</body>
</html>
