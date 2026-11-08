<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Anay Patel — Software Engineer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0B1220;
    --bg-panel:#101B2E;
    --bg-panel-2:#0E1830;
    --grid-line:rgba(138,180,213,0.10);
    --ink:#E9EEF2;
    --ink-dim:#8FA0B3;
    --ink-dimmer:#5C6C7E;
    --cyan:#6BB6E0;
    --cyan-dim:rgba(107,182,224,0.35);
    --amber:#E8A33D;
    --rule:rgba(255,255,255,0.09);
    --radius:3px;
    --ease:cubic-bezier(0.16, 1, 0.3, 1);
  }

  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}

  body{
    margin:0;
    background:
      linear-gradient(var(--grid-line) 1px, transparent 1px) 0 0/40px 40px,
      linear-gradient(90deg, var(--grid-line) 1px, transparent 1px) 0 0/40px 40px,
      var(--bg);
    color:var(--ink);
    font-family:'Inter', sans-serif;
    font-size:16px;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
    position:relative;
  }
  body.locked{overflow:hidden; height:100vh;}

  h1,h2,h3{
    font-family:'Space Grotesk', sans-serif;
    font-weight:600;
    margin:0;
    letter-spacing:-0.01em;
  }
  .mono{font-family:'IBM Plex Mono', monospace;}
  a{color:inherit;}
  ::selection{background:var(--cyan-dim); color:var(--ink);}
  :focus-visible{outline:2px solid var(--cyan); outline-offset:3px;}

  @media (prefers-reduced-motion: reduce){
    html{scroll-behavior:auto;}
    *{animation-duration:0.01ms !important; transition-duration:0.01ms !important; animation-delay:0s !important;}
  }

  /* ================= preloader ================= */
  #preloader{
    position:fixed; inset:0; z-index:200;
    background:var(--bg);
    display:flex; align-items:center; justify-content:center;
    transition:opacity 0.6s var(--ease), visibility 0.6s var(--ease);
  }
  #preloader.hide{opacity:0; visibility:hidden; pointer-events:none;}
  .boot{
    font-family:'IBM Plex Mono', monospace;
    font-size:0.88rem;
    color:var(--ink-dim);
    width:340px;
  }
  .boot-line{
    opacity:0; transform:translateY(4px);
    margin-bottom:8px;
    transition:opacity 0.3s ease, transform 0.3s ease;
  }
  .boot-line.show{opacity:1; transform:translateY(0);}
  .boot-line .ok{color:#5FCB8C;}
  .boot-cursor{display:inline-block; width:7px; height:14px; background:var(--cyan); margin-left:4px; vertical-align:middle; animation:blink 0.9s steps(1) infinite;}
  @keyframes blink{50%{opacity:0;}}

  /* ================= custom cursor ================= */
  #cursor-ring, #cursor-dot{
    position:fixed; top:0; left:0; z-index:150;
    pointer-events:none; border-radius:50%;
    transform:translate(-50%,-50%);
    will-change:transform;
    opacity:0;
    transition:opacity 0.4s ease, width 0.35s var(--ease), height 0.35s var(--ease), border-color 0.35s var(--ease), background 0.35s var(--ease);
  }
  #cursor-ring.visible, #cursor-dot.visible{opacity:1;}
  #cursor-ring{
    width:30px; height:30px;
    border:1px solid var(--cyan-dim);
  }
  #cursor-dot{ width:5px; height:5px; background:var(--cyan); transition:opacity 0.4s ease, width 0.35s var(--ease), height 0.35s var(--ease), background 0.35s var(--ease); }
  #cursor-ring.hovering{ width:56px; height:56px; background:rgba(107,182,224,0.07); border-color:var(--cyan-dim); }
  #cursor-ring.pressing{ width:22px; height:22px; }
  @media (pointer:coarse){ #cursor-ring, #cursor-dot{display:none;} }

  /* ================= persistent animated background ================= */
  #bgCanvas{ position:fixed; inset:0; z-index:-1; pointer-events:none; }

  /* ================= curtain wipe on load ================= */
  #wipe{
    position:fixed; inset:0; z-index:190; pointer-events:none; opacity:0;
    background:linear-gradient(100deg, transparent 30%, rgba(107,182,224,0.9) 48%, rgba(232,163,61,0.7) 52%, transparent 70%);
    transform:translateX(-120%);
  }
  #wipe.run{ animation:wipeAcross 0.85s cubic-bezier(0.7,0,0.3,1) forwards; }
  @keyframes wipeAcross{ 0%{transform:translateX(-120%); opacity:1;} 80%{opacity:1;} 100%{transform:translateX(120%); opacity:0;} }

  /* ================= scroll progress ================= */
  #scrollProgress{
    position:fixed; top:0; left:0; height:2px;
    background:linear-gradient(90deg, var(--cyan), var(--amber));
    z-index:60; width:0%;
    transition:width 0.1s linear;
  }

  .crop{ position:fixed; width:16px; height:16px; border-color:var(--ink-dimmer); border-style:solid; z-index:40; pointer-events:none; opacity:0.6; }
  .crop.tl{top:14px; left:14px; border-width:1px 0 0 1px;}
  .crop.tr{top:14px; right:14px; border-width:1px 1px 0 0;}
  .crop.bl{bottom:14px; left:14px; border-width:0 0 1px 1px;}
  .crop.br{bottom:14px; right:14px; border-width:0 1px 1px 0;}

  .wrap{max-width:1080px; margin:0 auto; padding:0 40px;}
  @media (max-width:640px){ .wrap{padding:0 22px;} }

  /* ---------- nav ---------- */
  nav{ position:sticky; top:0; z-index:30; background:rgba(11,18,32,0.86); backdrop-filter:blur(8px); border-bottom:1px solid var(--rule);
    transform:translateY(-100%); transition:transform 0.7s var(--ease);
  }
  body:not(.locked) nav{transform:translateY(0);}
  .nav-inner{display:flex; align-items:center; justify-content:space-between; height:60px;}
  .nav-mark{font-family:'Space Grotesk', sans-serif; font-weight:600; font-size:0.98rem;}
  .nav-mark .dot{color:var(--cyan);}
  .nav-links{position:relative; display:flex; gap:28px; list-style:none; margin:0; padding:0;}
  .nav-pill{ position:absolute; bottom:-1px; height:1px; background:var(--cyan); left:0; width:0; transition:left 0.4s var(--ease), width 0.4s var(--ease), opacity 0.3s ease; opacity:0; }
  .nav-links a{ text-decoration:none; color:var(--ink-dim); font-size:0.92rem; position:relative; padding:4px 0; transition:color 0.2s; }
  .nav-links a:hover{color:var(--ink);}
  .nav-links a.active{color:var(--ink);}
  .nav-actions{display:flex; align-items:center; gap:14px;}
  .cmdk-btn{
    display:flex; align-items:center; gap:8px; background:var(--bg-panel); border:1px solid var(--rule); color:var(--ink-dim);
    padding:6px 10px; border-radius:var(--radius); font-family:'IBM Plex Mono', monospace; font-size:0.78rem; cursor:pointer;
    transition:border-color 0.2s, color 0.2s, transform 0.15s var(--ease);
  }
  .cmdk-btn:hover{border-color:var(--cyan-dim); color:var(--ink);}
  .cmdk-btn kbd{background:var(--bg-panel-2); border:1px solid var(--rule); border-radius:2px; padding:0 5px;}
  @media (max-width:760px){ .nav-links{display:none;} }

  /* ---------- hero ---------- */
  header#hero{ padding:96px 0 76px; border-bottom:1px solid var(--rule); position:relative; overflow:hidden; }
  .aura{
    position:absolute; width:520px; height:520px; border-radius:50%;
    background:radial-gradient(circle, rgba(107,182,224,0.16), transparent 70%);
    top:-120px; right:-80px; pointer-events:none; transition:transform 0.3s var(--ease); filter:blur(10px);
  }
  .blob{position:absolute; border-radius:50%; filter:blur(60px); opacity:0.4; pointer-events:none; z-index:0;}
  .blob-a{width:380px; height:380px; background:radial-gradient(circle, rgba(107,182,224,0.35), transparent 70%); top:-100px; left:-60px; animation:driftA 16s ease-in-out infinite alternate;}
  .blob-b{width:300px; height:300px; background:radial-gradient(circle, rgba(232,163,61,0.20), transparent 70%); bottom:-90px; right:8%; animation:driftB 20s ease-in-out infinite alternate;}
  @keyframes driftA{ from{transform:translate(0,0) scale(1);} to{transform:translate(50px,35px) scale(1.15);} }
  @keyframes driftB{ from{transform:translate(0,0) scale(1);} to{transform:translate(-35px,-25px) scale(1.12);} }

  /* ---------- continuous flipping tile field (hero ambient) ---------- */
  .tile-field{
    position:absolute; top:6px; right:40px; z-index:0;
    display:grid; grid-template-columns:repeat(8, 28px); grid-auto-rows:28px; gap:6px;
    perspective:700px;
    -webkit-mask-image:radial-gradient(circle at 60% 40%, black 35%, transparent 75%);
    mask-image:radial-gradient(circle at 60% 40%, black 35%, transparent 75%);
  }
  @media (max-width:980px){ .tile-field{display:none;} }
  .tile{
    position:relative; width:28px; height:28px;
    transform-style:preserve-3d;
    animation:tileFlip var(--dur, 5s) linear infinite;
    animation-delay:var(--d, 0s);
  }
  .tile .face{
    position:absolute; inset:0; border-radius:3px;
    border:1px solid var(--rule);
    backface-visibility:hidden;
  }
  .tile .face.front{ background:rgba(107,182,224,0.06); }
  .tile .face.back{ background:rgba(232,163,61,0.10); transform:rotateY(180deg); }
  @keyframes tileFlip{
    0%, 42%{ transform:rotateY(0deg); }
    50%, 92%{ transform:rotateY(180deg); }
    100%{ transform:rotateY(360deg); }
  }
  .hero-grid{ display:grid; grid-template-columns:1fr auto; gap:56px; align-items:center; max-width:980px; position:relative; z-index:1; }
  @media (max-width:760px){ .hero-grid{grid-template-columns:1fr; justify-items:center; text-align:center;} }
  .hero-copy{min-width:0;}

  /* ---------- portrait ---------- */
  .portrait-wrap{
    width:210px; height:210px; position:relative; flex-shrink:0;
    opacity:0; transform:translateY(14px) scale(0.96);
    transition:opacity 0.8s var(--ease) 0.15s, transform 0.8s var(--ease) 0.15s;
  }
  #hero.ready .portrait-wrap{opacity:1; transform:translateY(0) scale(1);}
  @media (max-width:760px){ .portrait-wrap{width:170px; height:170px; margin-bottom:8px;} }
  .portrait-ring{
    position:absolute; inset:-6px; border-radius:50%;
    background:conic-gradient(from 0deg, var(--cyan), var(--amber), var(--cyan-dim), var(--cyan));
    animation:ringSpin 7s linear infinite;
  }
  @keyframes ringSpin{ to{ transform:rotate(360deg); } }
  .portrait-mask{
    position:absolute; inset:5px; border-radius:50%; overflow:hidden;
    background:var(--bg-panel);
    transform-style:preserve-3d; will-change:transform;
  }
  .portrait-mask img{
    width:100%; height:100%; object-fit:cover; display:block;
    clip-path:inset(100% 0 0 0);
    transition:clip-path 1.1s var(--ease) 0.5s;
    filter:saturate(0.92) contrast(1.03);
  }
  #hero.ready .portrait-mask img{clip-path:inset(0 0 0 0);}
  .portrait-mask::after{
    content:""; position:absolute; left:-10%; right:-10%; height:45%;
    background:linear-gradient(180deg, transparent, rgba(107,182,224,0.4), transparent);
    animation:scanSweep 3.6s ease-in-out infinite;
    animation-delay:1.8s;
    mix-blend-mode:overlay;
    pointer-events:none;
  }
  @keyframes scanSweep{
    0%{ transform:translateY(-140%); }
    60%, 100%{ transform:translateY(220%); }
  }

  .reveal-mask{overflow:hidden;}
  .reveal-mask > *{ transform:translateY(115%); transition:transform 0.85s var(--ease); }
  #hero.ready .reveal-mask > *{transform:translateY(0);}

  .kicker{font-family:'IBM Plex Mono', monospace; font-size:0.82rem; color:var(--ink-dimmer); margin-bottom:18px;}
  h1.name{font-size:clamp(2.4rem, 5vw, 3.6rem); line-height:1.05;}
  .name-underline{
    display:block; height:2px; width:0; margin-top:16px;
    background:linear-gradient(90deg, var(--cyan), var(--amber));
    transition:width 0.8s var(--ease);
  }
  #hero.name-drawn .name-underline{width:110px;}
  .word{display:inline-block; opacity:0; transform:translateY(10px); transition:opacity 0.55s var(--ease), transform 0.55s var(--ease);}
  .word.show{opacity:1; transform:translateY(0);}
  .role-line{ font-size:clamp(1.1rem, 2.1vw, 1.32rem); color:var(--ink-dim); font-weight:400; margin-top:16px; max-width:38ch; }
  .hero-desc{
    margin-top:22px; color:var(--ink-dim); max-width:50ch; font-size:0.98rem;
    opacity:0; transform:translateY(10px); transition:opacity 0.7s var(--ease) 0.5s, transform 0.7s var(--ease) 0.5s;
  }
  #hero.ready .hero-desc{opacity:1; transform:translateY(0);}

  .hero-cta{ display:flex; gap:14px; margin-top:34px; flex-wrap:wrap; opacity:0; transform:translateY(10px); transition:opacity 0.7s var(--ease) 0.65s, transform 0.7s var(--ease) 0.65s; }
  #hero.ready .hero-cta{opacity:1; transform:translateY(0);}

  .btn{
    font-family:'Inter', sans-serif; font-size:0.92rem; padding:11px 20px; border-radius:var(--radius); text-decoration:none; cursor:pointer;
    border:1px solid transparent; display:inline-flex; align-items:center; gap:8px; position:relative; overflow:hidden; will-change:transform;
    transition:transform 0.2s var(--ease), background 0.2s ease, border-color 0.2s ease;
  }
  .btn-primary{background:var(--cyan); color:#08121F; font-weight:500;}
  .btn-primary:hover{background:#7fc2e6;}
  .btn-ghost{border-color:var(--rule); color:var(--ink);}
  .btn-ghost:hover{border-color:var(--cyan-dim);}
  .btn::after{
    content:""; position:absolute; top:0; left:-60%; width:40%; height:100%;
    background:linear-gradient(120deg, transparent, rgba(255,255,255,0.35), transparent);
    transform:skewX(-20deg); transition:left 0.6s ease;
  }
  .btn:hover::after{left:130%;}

  .title-block{
    margin-top:44px; display:flex; gap:28px; flex-wrap:wrap; font-family:'IBM Plex Mono', monospace; font-size:0.76rem; color:var(--ink-dimmer);
    border-top:1px solid var(--rule); padding-top:14px; opacity:0; transition:opacity 0.7s var(--ease) 0.8s;
  }
  #hero.ready .title-block{opacity:1;}
  .title-block span b{color:var(--ink-dim); font-weight:500;}

  /* ---------- reveal-on-scroll ---------- */
  .reveal{opacity:0; transform:translateY(26px); transition:opacity 0.7s var(--ease), transform 0.7s var(--ease);}
  .reveal.in-view{opacity:1; transform:translateY(0);}

  /* ---------- section shell ---------- */
  section{padding:80px 0; border-bottom:1px solid var(--rule);}
  .section-head{display:flex; align-items:baseline; justify-content:space-between; margin-bottom:40px; gap:20px; flex-wrap:wrap;}
  .section-head h2{font-size:clamp(1.5rem, 3vw, 1.9rem);}
  .section-index{font-family:'IBM Plex Mono', monospace; color:var(--ink-dimmer); font-size:0.8rem;}

  /* ---------- work / timeline ---------- */
  .timeline{position:relative; padding-left:26px;}
  .timeline::before{content:""; position:absolute; left:4px; top:6px; bottom:6px; width:1px; background:var(--rule);}
  .timeline::after{ content:""; position:absolute; left:4px; top:6px; width:1px; height:0; background:var(--cyan); transition:height 1.2s var(--ease); }
  .timeline.in-view::after{height:var(--tl-h, 0);}
  .job{position:relative; padding-bottom:44px;}
  .job:last-child{padding-bottom:0;}
  .job::before{
    content:""; position:absolute; left:-26px; top:4px; width:9px; height:9px; border-radius:50%;
    background:var(--bg); border:1.5px solid var(--cyan); transition:transform 0.3s var(--ease), box-shadow 0.3s var(--ease);
  }
  .job:hover::before{transform:scale(1.3); box-shadow:0 0 0 5px rgba(107,182,224,0.15);}
  .job-head{display:flex; justify-content:space-between; align-items:baseline; flex-wrap:wrap; gap:8px; margin-bottom:6px;}
  .job-title{font-family:'Space Grotesk', sans-serif; font-weight:600; font-size:1.08rem;}
  .job-org{color:var(--cyan); font-weight:500;}
  .job-meta{font-family:'IBM Plex Mono', monospace; font-size:0.76rem; color:var(--ink-dimmer); white-space:nowrap;}
  .job-place{color:var(--ink-dim); font-size:0.88rem; margin-bottom:10px;}
  .job ul{margin:0; padding-left:18px; color:var(--ink-dim); font-size:0.94rem;}
  .job li{margin-bottom:7px;}
  .job-tags{display:flex; gap:8px; flex-wrap:wrap; margin-top:14px;}
  .tag{
    font-family:'IBM Plex Mono', monospace; font-size:0.76rem; font-weight:500;
    color:var(--cyan); background:rgba(107,182,224,0.08); border:1px solid var(--cyan-dim);
    padding:4px 11px; border-radius:4px; letter-spacing:0.01em;
  }

  /* ---------- projects ---------- */
  .project-grid{display:grid; grid-template-columns:repeat(auto-fit, minmax(280px, 1fr)); gap:22px;}
  .project-card{
    background:var(--bg-panel); border:1px solid var(--rule); padding:26px; position:relative;
    transition:opacity 0.25s, border-color 0.25s, transform 0.1s linear; transform-style:preserve-3d; perspective:800px; will-change:transform;
  }
  .project-card:hover{border-color:var(--cyan-dim);}
  .project-card::before, .project-card::after{content:""; position:absolute; width:7px; height:7px; border-color:var(--ink-dimmer); border-style:solid; opacity:0.5;}
  .project-card::before{top:8px; left:8px; border-width:1px 0 0 1px;}
  .project-card::after{bottom:8px; right:8px; border-width:0 1px 1px 0;}
  .card-glare{ position:absolute; inset:0; pointer-events:none; background:radial-gradient(circle at var(--mx,50%) var(--my,50%), rgba(107,182,224,0.10), transparent 55%); opacity:0; transition:opacity 0.3s ease; }
  .project-card:hover .card-glare{opacity:1;}
  .project-badge{font-family:'IBM Plex Mono', monospace; font-size:0.72rem; color:var(--amber); margin-bottom:10px; display:block;}
  .project-card h3{font-size:1.15rem; margin-bottom:12px;}
  .project-link{color:var(--ink); text-decoration:none; border-bottom:1px solid var(--cyan-dim); padding-bottom:1px; transition:border-color 0.2s ease, color 0.2s ease;}
  .project-link:hover{color:var(--cyan); border-color:var(--cyan);}
  .project-card p{color:var(--ink-dim); font-size:0.92rem; margin:0 0 14px;}
  .project-card ul{margin:0 0 14px; padding-left:18px; color:var(--ink-dim); font-size:0.9rem;}
  .project-card li{margin-bottom:6px;}

  /* ---------- skills ---------- */
  .skill-modules{display:grid; grid-template-columns:repeat(3, 1fr); gap:28px;}
  @media (max-width:760px){ .skill-modules{grid-template-columns:1fr;} }
  .skill-module h3{font-size:0.98rem; color:var(--cyan); margin-bottom:14px; font-family:'IBM Plex Mono', monospace; font-weight:500;}
  .skill-chips{display:flex; flex-wrap:wrap; gap:8px;}
  .skill-chip{
    font-size:0.83rem; padding:6px 11px; background:var(--bg-panel); border:1px solid var(--rule); border-radius:var(--radius); color:var(--ink-dim);
    transition:border-color 0.2s ease, color 0.2s ease, transform 0.2s var(--ease);
  }
  .skill-chip:hover{border-color:var(--cyan-dim); color:var(--ink); transform:translateY(-2px);}

  /* ---------- education ---------- */
  .edu-row{display:flex; justify-content:space-between; align-items:flex-start; flex-wrap:wrap; gap:16px;}
  .edu-name{font-size:1.15rem; font-family:'Space Grotesk', sans-serif; font-weight:600;}
  .edu-detail{color:var(--ink-dim); margin-top:6px; font-size:0.94rem;}
  .edu-meta{font-family:'IBM Plex Mono', monospace; font-size:0.8rem; color:var(--ink-dimmer); text-align:right;}
  .course-chips{display:flex; flex-wrap:wrap; gap:8px; margin-top:20px;}
  .edu-year{margin-top:18px; font-family:'IBM Plex Mono', monospace; font-size:0.72rem; color:var(--ink-dimmer);}

  /* ---------- connect ---------- */
  #connect{border-bottom:none;}
  .connect-panel{
    background:var(--bg-panel); border:1px solid var(--rule); padding:44px;
    display:grid; grid-template-columns:1.1fr 0.9fr; gap:40px; position:relative; overflow:hidden;
  }
  @media (max-width:760px){ .connect-panel{grid-template-columns:1fr; padding:28px;} }
  .status-line{ font-family:'IBM Plex Mono', monospace; font-size:0.82rem; color:var(--ink-dim); margin-bottom:24px; }
  .connect-links{display:flex; flex-direction:column; gap:14px;}
  .connect-link{
    display:flex; align-items:center; justify-content:space-between; padding:14px 16px; border:1px solid var(--rule);
    text-decoration:none; color:var(--ink); font-size:0.95rem;
    transition:border-color 0.2s, background 0.2s, transform 0.2s var(--ease);
  }
  .connect-link:hover{border-color:var(--cyan-dim); background:rgba(107,182,224,0.05); transform:translateX(4px);}
  .connect-link .arrow{display:inline-block; transition:transform 0.3s var(--ease); color:var(--ink-dimmer);}
  .connect-link:hover .arrow{transform:translate(3px,-3px) rotate(8deg); color:var(--cyan);}
  .connect-link .label{color:var(--ink-dim); font-family:'IBM Plex Mono', monospace; font-size:0.78rem;}
  .email-actions{display:flex; align-items:center; gap:14px;}
  .copy-btn{background:transparent; border:none; color:var(--cyan); font-family:'IBM Plex Mono', monospace; font-size:0.78rem; cursor:pointer; padding:0;}
  .draft-link{color:var(--cyan); font-family:'IBM Plex Mono', monospace; font-size:0.78rem; text-decoration:none; border-bottom:1px solid var(--cyan-dim); padding-bottom:1px;}
  .draft-link:hover{border-color:var(--cyan);}
  .local-card{border:1px solid var(--rule); padding:22px; display:flex; flex-direction:column; justify-content:center; gap:8px;}
  .local-time{font-family:'IBM Plex Mono', monospace; font-size:1.7rem; color:var(--cyan); font-variant-numeric:tabular-nums;}
  .local-label{color:var(--ink-dimmer); font-size:0.8rem;}

  footer{
    padding:30px 0 60px; display:flex; justify-content:space-between; align-items:center;
    color:var(--ink-dimmer); font-family:'IBM Plex Mono', monospace; font-size:0.76rem; flex-wrap:wrap; gap:10px;
  }

  /* ---------- command palette ---------- */
  .cmdk-overlay{
    position:fixed; inset:0; background:rgba(5,9,16,0.7); display:none; align-items:flex-start; justify-content:center;
    padding-top:14vh; z-index:100; backdrop-filter:blur(2px);
  }
  .cmdk-overlay.open{display:flex;}
  .cmdk-panel{
    width:min(560px, 90vw); background:var(--bg-panel); border:1px solid var(--rule); box-shadow:0 20px 60px rgba(0,0,0,0.5);
    transform:translateY(-10px) scale(0.98); opacity:0; animation:cmdkIn 0.25s var(--ease) forwards;
  }
  @keyframes cmdkIn{to{transform:translateY(0) scale(1); opacity:1;}}
  .cmdk-input{ width:100%; padding:16px 18px; background:transparent; border:none; border-bottom:1px solid var(--rule); color:var(--ink); font-family:'IBM Plex Mono', monospace; font-size:0.95rem; }
  .cmdk-input:focus{outline:none;}
  .cmdk-results{max-height:320px; overflow-y:auto;}
  .cmdk-item{display:flex; justify-content:space-between; padding:13px 18px; cursor:pointer; font-size:0.9rem; color:var(--ink-dim); transition:background 0.15s ease;}
  .cmdk-item .tag-small{font-family:'IBM Plex Mono', monospace; font-size:0.72rem; color:var(--ink-dimmer);}
  .cmdk-item.selected{background:rgba(107,182,224,0.1); color:var(--ink);}
  .cmdk-empty{padding:18px; color:var(--ink-dimmer); font-size:0.86rem;}

  /* ================= cursor flock: builds the page, flies like birds, then leaves ================= */
  body.cb-mode .reveal{opacity:1; transform:none;}
  body.cb-mode .cb-hidden{opacity:0 !important; pointer-events:none;}

  #ghostTrails{position:fixed; inset:0; width:100%; height:100%; z-index:80; pointer-events:none;}
  #ghostLayer{position:fixed; inset:0; z-index:90; pointer-events:none; overflow:hidden;}
  /* boxes, carets and working cursors live here: it is part of the page, so the browser scrolls it with the text */
  #ghostDoc{position:absolute; left:0; top:0; width:100%; height:0; z-index:90; pointer-events:none;}
  @media (max-width:700px){ #ghostTrails, #ghostLayer, #ghostDoc{display:none;} }

  .gc{position:absolute; left:0; top:0; opacity:0; transition:opacity 0.5s ease; will-change:transform;}
  .gc.on{opacity:1;}
  .gc-arrow{position:absolute; left:-2px; top:-1.5px; width:18px; height:22px; transform-origin:8px 11px;}
  .gc-arrow svg{
    display:block; width:18px; height:22px; color:var(--c); transform-origin:8px 11px; transition:transform 0.12s ease;
    filter:drop-shadow(0 0 6px color-mix(in srgb, var(--c) 65%, transparent)) drop-shadow(0 2px 4px rgba(0,0,0,0.45));
  }
  .gc.press .gc-arrow svg{transform:scale(0.8);}

  .gc-select{
    position:absolute; left:0; top:0;
    border:1.5px solid var(--c);
    background:color-mix(in srgb, var(--c) 7%, transparent);
    border-radius:3px; opacity:0; transition:opacity 0.3s ease; will-change:transform;
  }
  .gc-select.on{opacity:1;}
  .gc-select i{position:absolute; width:7px; height:7px; background:#0B1220; border:1.5px solid var(--c); border-radius:1.5px;}
  .gc-select i.tl{left:-5px; top:-5px;}
  .gc-select i.tr{right:-5px; top:-5px;}
  .gc-select i.bl{left:-5px; bottom:-5px;}
  .gc-select i.br{right:-5px; bottom:-5px;}
  .gc-select .gc-tag{
    position:absolute; right:-1.5px; top:100%; margin-top:8px; padding:2px 7px;
    background:var(--c); color:#0B1220; font:500 10px/1.4 'IBM Plex Mono', monospace;
    border-radius:3px; white-space:nowrap;
  }

  .gc-ripple{position:absolute; width:16px; height:16px; margin:-8px 0 0 -8px; border-radius:50%; border:2px solid var(--c); animation:gcRipple 0.7s ease-out forwards;}
  @keyframes gcRipple{ from{transform:scale(0.3); opacity:1;} to{transform:scale(3.6); opacity:0;} }
  .gc-caret{
    position:absolute; left:0; top:0; width:2px; border-radius:1px;
    background:var(--c); box-shadow:0 0 8px var(--c);
    animation:gcBlink 0.9s steps(1) infinite; will-change:transform;
  }
  @keyframes gcBlink{ 50%{opacity:0.15;} }
</style>
</head>
<body class="locked">

<canvas id="bgCanvas"></canvas>
<div id="wipe"></div>
<div id="preloader"><div class="boot" id="bootLines"></div></div>
<div id="cursor-ring"></div>
<div id="cursor-dot"></div>
<div id="scrollProgress"></div>

<div class="crop tl"></div>
<div class="crop tr"></div>
<div class="crop bl"></div>
<div class="crop br"></div>

<nav>
  <div class="wrap nav-inner">
    <div class="nav-mark">Anay Patel<span class="dot">.</span></div>
    <ul class="nav-links" id="navLinks">
      <span class="nav-pill" id="navPill"></span>
      <li><a href="#work">Work</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#education">Education</a></li>
      <li><a href="#connect">Connect</a></li>
    </ul>
    <div class="nav-actions">
      <button class="cmdk-btn" id="cmdkOpen" data-magnetic>Jump to <kbd>/</kbd></button>
    </div>
  </div>
</nav>

<header id="hero">
  <div class="blob blob-a"></div>
  <div class="blob blob-b"></div>
  <div class="aura" id="aura"></div>
  <div class="tile-field" id="tileField" aria-hidden="true"></div>
  <div class="wrap hero-grid">
    <div class="hero-copy">
      <div class="reveal-mask"><div class="kicker">Software Engineer · Gainesville, FL</div></div>
      <h1 class="name" id="heroName">Anay Patel</h1>
      <span class="name-underline"></span>
      <p class="role-line" id="roleLine">I like taking a messy problem and building something that actually works — AI systems, data pipelines, and the infrastructure holding them together.</p>
      <p class="hero-desc">Currently studying computer science at the University of Florida, with recent work spanning a generative-AI assistant at BDO, a live quant research pipeline, and generative modeling for neurodegenerative research. Looking to bring that into a software engineering internship this summer.</p>
      <div class="hero-cta">
        <a href="#work" class="btn btn-primary" data-magnetic>See the work</a>
        <a href="#connect" class="btn btn-ghost" data-magnetic>Get in touch</a>
      </div>
      <div class="title-block">
        <span><b>Role</b> Software Engineer</span>
        <span><b>Based</b> Gainesville, FL</span>
        <span><b>Focus</b> AI systems &amp; backend infrastructure</span>
      </div>
    </div>
    <div class="portrait-wrap" id="portraitWrap">
      <div class="portrait-ring"></div>
      <div class="portrait-mask">
        <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAUEBAQEAwUEBAQGBQUGCA0ICAcHCBALDAkNExAUExIQEhIUFx0ZFBYcFhISGiMaHB4fISEhFBkkJyQgJh0gISD/2wBDAQUGBggHCA8ICA8gFRIVICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICD/wAARCAHgAeADASIAAhEBAxEB/8QAHQAAAQUBAQEBAAAAAAAAAAAAAwIEBQYHAQAICf/EAEkQAAEDAgQDBQQHBgUCBQQDAAEAAgMEEQUSITEGQVEHEyJhcRQygaEjQlJikbHBFSQzNHLRQ4Ky4fAl8Qg1U6LCFiZE0lRjkv/EABsBAAIDAQEBAAAAAAAAAAAAAAABAgMEBQYH/8QALBEAAgIBBAEDAwQDAQEAAAAAAAECEQMEEiExQQUTUSIyYQYjcYFCkbEUYv/aAAwDAQACEQMRAD8AI6oBYSl4dVyOqe7YTqmGR4YdVJ8OxZsUaCLhUP6kNPayffROlibI4Zh5qtYmGU0psFqMtG32EWasz4ngIkcAuc8VTs3KdobQVrC0DROmyxuVdijkaB4inbDKOa1RjZRJk7ka4AtcnlFVuo5czn+EKEhmkBaPNJxWZ8NM97XW8Kl7NkN5qmD8XUbGtZLKPxVupscw+pAyyt1818ZVHEtfDUHu5djbdXjhriPEZY2OdK78VZLBKrQlNH1GDSzDwuaUh9DG7VpWNUvFtZTEZnk+qsVHx4RYSFUNTiWKmXt1FKzVjykh9VEdRdRNHxlRzgBzxdTEWM0M40kGqj7nyh7fgW2ve332kJU2INMFkvNSyjRzShvooXjQp7osRTq92etc/kmEp5K1V2ExtYS06qsSx5JMjtwVJP4INDVzV1oNiUom7nWRCAGt6pkRlY57qRiaCwXTQWzmydMcbBIDhaA4pObw+qIQb3SS0ApAJy3AIQnG7iE5Z7pQnN1NgkM9HGC253S3AN5rrLhoSXXdfRIsGkguVwR+IFGLNQSlEAFBGhzSM8KcPjPRJohcBP3R+Sg42WJkYYkkxaKQMeuyT3fklsDcRxiK73Sfd2Oi93fkjYG4jzEhmNSDmeSG6NGwW4Zd3dJMdk9yJJZdGwNwzyJBZ5J6Y0kx+SNgbhgWG6T3eqfmMJHdp7AsZ5F7u06yeS9kRsFY0MaT3RsnhYuBiNgWMzHZcLQnZaOiQWBGwLGuQLmRO8gKS5tkbAsbZLcl4tJCcWvyXMhT2BY2yFcMZITrJrsvFtkbAsYGI32XRGU7LVwsT2BY3yL2RHyr2VPYFlPcwBhUrwzGDirdEwkHgcpfhVt8Vat8EY2zTXwj2EaclmPFMA70rWiz9yAtyWY8VstIfVKcC2MimtiAA0RWxeSM1l0UNFlFKgbBxx+No8004kGTD5D91SbBaRvqovigf9Ol/pU49iMSlkLql4J+stD4YbJkbvayzl/847+ta1wpEDRMJHJaZdEUTrczgA5KfGRqNPRKlJa8WbokmUEWNws0ixARNPE7wvKeQYzWw6iR2nmmzmh2oIK4YvAfRQcU+yVsmqPjetZIGF5OvMq94VxJUzsbmBNwsNeXsrA0c3LWeG25qeO7dQFTkwqrQ1JlzmxV0sJDhYhV+bO+Qv6qQkZdhsmjzazbbKMI7UJuxiG2lIKU+5alAXeXDqiPZZgKkIZsHiTpgsAhtb9JZOMpIFkqAUSMpQdTYrrg7Vq8xtgL8kqA6GEAheAu6xXS+1+i803KVAEyjLokBmtkW1mIGazyAoFiPSR2CC4EIskl7IRNymhMkcOF2hSxZoo7DrAa6KXzR5d1JUMamNIMacukjHNAdPGDa6OABGNJLNEcOa/ZdsEwGhYkmNOnNCG5qlQrGpjSTGnJCSQigsb5Fws02TghIIRQrG5Z5JBb5JyQhOCKCwBauBqLZcKKFYJwXMqWd15FBYAt12SSEYhIIsigsQBqkvZuiBKsigsbNZqlZRZFIskEIoLEWXHNStbrqKCwJC5ZFISSEUFg8pXrInJetdFBZT3jwOUzwoP+qBRMgGRymeFB/wBTC3Y1yZGzVw390Hos04tZ4z6rTwP3QeizXiweJ3qpzXBOLKg0JYC40IoasxM4wfSNUVxQ62HSX6KZjb9I1QPFpIw6X0Uo9gYo/WuNvtrYeFGWoWHyWOx+KvA++tp4XaBQsvtZXy6EifvCXgOAS30tPK3w2Q3Qwvfq6y8aSRovFLdZ5FiGs+HObcxuUdP7TAxw1IspWQ1cY1aSo6qqiY3Ne0g2SSGQVJKZ60NkGoctm4fZamZbTRYzQva+v2sQ5bRw/wDy0Z8kZFwJFgbq3UKPqWASEqQvYOKZTeI76LOhjW1jpzXib+EojWXK4+PW45pgIyAapTHW3ST7qUxtwB0QAl7ha1tUkOF9EtzdEhrfHskM65twkRnxIl7t80hg8VwFEQ41PJDLDqbaI4AFjyQ3OsHBRolY3LNV3JsUppu1KAu4IofYVkogaCUiTFmt0TeveY4wQL6Kuy1TzIbBZ5KTfBZGvJYX4uNbJozEzJPZQLql55Jzh5dJNcjmnGErHJqi6UTy8AlSFkzw5lor25J/Za0iiwThohOCO4ITmqQgNlwhELVwhMYIhIKMQkEIACQkEIxakEJhYEhIIRXBJy6pCAkLlkbKuZQgVgiEktujEBIKY7BZbLoCWVyyQWDISbI2VJLUwB5FzLoipJSAGWpJCIdkM7oA5lXLJS9ZAFQlHgcprhMf9TChpfdcpvhP/wAzC2QMhrA/lB6LNOLPfd6rSx/KD0WacWe+71Vk+icSqMGyOBohxjQIwWZIsPMHjaq9xe2+HS+isbR42qv8W2GHy+ia7EYhAL4k0ffW2cMs/cGg9FitLrizR99bfw639wb6K6YIkn0znO8L0jLUxbXKc5Xl+i87vG7hZ2iaG5qpGjxhMayaKSF12i9k/kqBYhzQVGVckJicctipKINkJQiP28Foscy2nh1v7rH6LFKLIcQBadcy2zh64pY/RRydDROPabFMnsNtE+c4NumziFnQwGQtdslO/AhGJDj5hcLAWEoAam2UpAPiR3x2sRzSBGMxQAgnQrjPE5ceCAUltwdEAFISchsHBEaCd9UU2AsRoogNnOdtZJAJJ6o5YHE2QX+GxSGeDOaXls5JaRzSgdkAgVZHmZbdQT6bxnwq0ujzs2TCSnsT4VOELByIB1NYe6nmGwWl25p1JH5Jxh8Xj2VqgRciw0bLRbJwQuU4AiRCENCsCQUMtRnaIZKVDsE4WQ7Ix1QyEbQs5ZccEqyQUbQsG5CIRnDRDKe0LAuCRayMQkFLaFiCUm910rgCKA8dkN26KkEaooAdilALtl2yKEeI02SCEQ7JBRQ0xBCGQUUpJRQwWU3SSNUQobkqA5Yr2U9UoarxToCnS6tcpzhL/wAyCg5fdcp7hIf9RC2QMhq3/wCIPRZnxX/Ed6rTD/KfBZpxX77vVTn0TiVhg0RWhCjOicNWYmeYPG2yrnGFzhsvorMweMKscYvDcOl9ELsDFqBt8XaPvFblgDD+z2gb2WIYYL4w3+orcsEBbhzSN7K6YRHMnftfdt0M1czdHNKK6WUSHTRcM7To9gVJIaPqGuPiYmNYYnQuINjZSUgp3Dayi6+KPunFrraKxciZE4ZG014c11/EtvwA2pYrdFiGEMLcQBzXBctxwBhMERHRVZSUSalaTewQu6vuOScP0uCg5jlt5rMSAiP5JTweWycgA+hCC4bjogBmdRY8kpgOa668HMozGcbo8FoxLUPb3rzliizAGR3TXYdTyToCQmYAwkkBRUuLYdA8MfVxZybZc4uo+CGvxWBs1dKycyuymOMZoo2nk0XAvb6zrnyCcy8OYO6AQSU0jXN+uaVkgaetwANPipKHyFkhDiFMXtaZWtL/AHQ42v6J+5oIuqNilBiVXjlVgWAUtC+KjYx1TUOjcI2k6tYYwbOeQL6WsNb6hMPbOL20+KYfQ0ohxGnZeSGJhc2MWu18eYkWc38CCpe3fQrNIGVv1gCeV03laHLHWYjwrW0z6itMzq/KO8p6l8rJYnWFznzWOmt7Aa7BOKTib2Ccx0GKVU9OG5r1AB7r7rrnxctWltr80/YfgLNYAIIS22OhVJwXtDwSucIK+shppb2zZjkP4gEf81U8zGqStqJIsLmFSyIXkmZrG3/NzVbg0Oye79jGgbnoFGVuIGKUMyHVL75rGxkTsMkmjUuWCjh+nq6hl97vcArYLgiyPFUHbi3qnmH1DDNkJAPqmMM+EYzJIaKqinbE7K4sdcA9F1+FyRzNfSuzW1sHaqyhFygeMlkcHRQlDWWAjl8L9rFS7XAi4VbXICnhAddGJQ3JDEWXF669ugDhSHBLKQ5MATkgpbkMpAJKESiFDcmAg7rwXrLoCQHbJD0RIcEADulBJslBIDxGiQd0Q7IROqAOFIKIdkMhMBBKQb3RCEg7oA4upQF17KgClynwuVh4R/nwq5KfA5WPhD+eWuBmNVd/KfBZlxVq93qtMd/KD0Wa8UD6Q+qlPolErEYsAjtQ2jwhEaFmLArBdwVQ420w6X0Vyjb4gVTuN/8Ay6X0TXYGQYMM2Lt9VumEeDDmkdFh+Ai+MD1W54b4cNad9FbMIizU2ebtXDPA73mrwkjzkOYiGOneNrKokN5GQPGjrFQ2Iw5Y3ZX3FlMy07R7r1DYjHIInWdopxEyKwRrhXjMbjMt84bYHUkfkAsFwRr21zQ7bMt/4bsKSP0VWUlEkqgBpKa6finlSCXGwTQNNtVmJHrnLbogSzNYCXGydkeFUniqtBe+iExghiidPUyA2LWAGw+NlJKwFYvj+HNc9jqueVsYJfDR++62937MA5kkLP6XF524lUYuKeephEhipfbrTRMbYHK12hcb3NwCdlFYhxFgtNatxSJwgab0uEtcAHRj3TIG/aNzY8hfUm4oeK8aVuMSvgdKWx2IyMcA4Mv7otsPIb21utcMdkW6NKq+0h9K17WMoYZ2tLWNghMhvffM8kN2Onpoq7Vdo2KTsIkkpy4/XljJI6WDSAFn4/Zj4CX96Gn3m5wcvnzsmjqJu9DUtsTpd2o/G4WpYooqcy10vG+P4XUPnoMQbTzSPzvc2/0hP2tdU6puPuJpap+KjE2icsc3M4ZhIOlvXUA6AhZtPUSUc49oPtIHvaWB9LfmpX2m4D4GmOOxL4joY9rAqWyPwLcyXlmmqa32ierOYOzZrXda9yPx63si1FdmAjhOcZSXBpBJP1RY9N1XHV0bYA9oyw5MxP8AmIt+ITiKRksYmaQ640UkhWSxnrH0T4GwMkkAMrmlti0HQWd10+YXmvqfZiaKQ05ffOLmxsL23F+tk0hxJ1LIJJgHMOh090J33l6mB4a0hutid9dx8ChxTBNjQYli7xZ+PTRx291mYAD8U4bUwzSM7+eWvl08VRO4j4BQNRLFFPLEJWNY0hx5AE80uCeCN9s4J55SVXtSLLNGoOJMTgljZhc72CJuVgawAZenmp2m7QOKoZo5ns74B3umMC/4clnVFVNEYfnkAfoM3MKT9pmuPEQwbBgtb4p7UBrtN2o4dWta6uoZ4qtpAyxAC/wO60rAcepMWp/oHnM0AlrhY2Oy+W5X9+BIyaJ1+Tjc/LZWrg/i+vwTFYvaSHU58Bda9h8N1nnBeCSPpUlIJTHCcUpsWoGVVNK2RrubTeyfkLMMSBfkukJQ0XkADKG4IxCG4IAA5DIRnAJBCBgiEMhHISLIADZeSyAkEoEeXCu7rhCBiFxdK8kI4SkEapXNJcQgRy68bLi8gYg2SCllIIQB1pSrpLbLpTAo8h8DlZeEP51RM+EVbQ4Zb/BTnC1NLBW3kbZa4LkzM0138r8Fm3E38U+q0guBpNOizfib+MfVSydEoFcbyRAEgC4uiNBsspYHi1IVM450w6X0VyivnCpXHbrYdL6KSAyzhxubFr+a3PDgBh7M21liPC4vivxW6UDGmgbm00U5hHoUxlM5xzJbqaAjwPsuClje42fYohoJAPDJdVEhlLSOt4XgqDxKKZkLgRop6aOoiHNQuISy9y4OHJTiJkLgZc6vAcNnLfuHo7UjDyssDwNxdiABH1l9A8PG9HGD0VeQlEfSmziEO1tUd7WmUgpL2/R6LOSAty21WF9rnEfcSTYXQZGvmeGzSZQb5RsT5X26nyUt2t9pv/0hTtwnDJCcUqBe7f8ACby15E/IeoXzrNi1dWQSTVs5qJyM9yd9Lm3lqtWHHfLItkdiVZLJUOaZSQDYuLtSUGGlc8h4YwP3Ba6342SI2xAGV7TK4a2vYKRiq3tYGnwH7oFityVFLYdjAyIA2bIBrlaNEVlKWQ53vEbSL27oXt/ZcjmdG18jiTLs1p2HnZJLo43Z5nGWQn3bnf4c1MiROJGlazNDE7MTyH6JEta9vdzA2AIjkvzHK6fVU0j4i0hrSP8ADiaLjyJ1UNK6RgdJ3DrcgTc3+AQBNmmhqaJ8TLEC+Ug3F73sfigwVQhsxrGNcGXcCLuvchM8LmIEjGucw5SRrsnoc2ojL3DLOPfdHZriPPy9EAHfO2SVozFpv/DB971T4TSMyNs187tA2+g/4E0p6TLUsqI3N1GtxrtsDy5IjoDF9JlL8nLqlZKiPMQxGYtjk76VozeEXDreaRklY0lwcSx27QPC3z+KkKdxpWB72Cd7jZkTW6AchbYablNKuuhdU5J5iGP0cxgDWs/DX4nookh5S1LSC8ZnlvnsnbKxxLQNLHQXTEUVPSsDZgXkyEM1sHi1wfmnkRYPDHla7a+TU/FAD+nZlBLssTg7OGtcL/gFKQO7xoY57g7cW5qJjY5jSDI1gvbQjUotO2uE9+8iljO1jkP9iq5Ekad2e4/Ng/GNJFVSPjosQZkLXnw5zsfxX0ISCLhfIney09BnqC6N0L2kOtcnXQ+a3Xg/tAw/EYqXDa+pZDWSMHdZjYSG2rQTz6dQszRZJGh31XrpAdmSuSgyB26QV0pBUbGJKQV1xKQUAccUMlecUgkoA84oZStSklIDwXCV5JcgDhK8EhduEAKOoQ9yu5km4QCPWK4Uq6Q4hACSVwpJIukk3QAQELpsh3svZkAW98VFID7pQmUtNFIHxht1mY4injbclwU/w9i8tfVBrnOsFpi5MpdF8Y8mIjYKg8TX74+q0MRhtNfnZZ7xJ/FPqrZrgjErjTsjtQw0X2RWhZywNGPGFROPdMPl9FfYdXqh9oBth8qa7AzbhMXxO/mFuVEwOomAm2ixHhBt8RvbmtvpWONIwA20U5jj0FZSuzXa9FLKhg0N0KKKcG4N0Z/tLR7pVBMZVDp7G4Kha9zjA7M3kpuWokFw5iicQnY6B1262VkSLITBXB2INFrEOW8YC4eysA6LCcGLX4g2wscy3TA25YGeiryDiSz2OJLgmlXU+y07nEFx2a37R5D4lSIfcWKz7tZxKuwHg5uO0F70lVE6QBtxlJtc/EhUxVuiZ86VMMHHPanjVdi1UyTC8MkcHvD7NneHZQ0c8hIcTbUMYSqDiFdAMWqqins2F8jhC21rMv4dOWie0tf7PgdTT08sjXTSlzxYAOcfec47nw6AfeKrIHeVDXOJOZwXShEpkyXifE5wGRoH2Tff+ycRzxskdZoBIvbUn8UxBInay3mfILsM4bI4NIOuoO//ADZXECULy1hLfeJsPI9f1Qrvkzdy7IG6OkO/mAgseZALnfbnqUqXNI5tFTAtaD433t6lACZ6ungibH45CdLDUnzJUVUh8niEbgOWbRWAR0WHU5lcGyTEe9JoG/2/NVytxBs0ptncTz2TEJjdNBkcx5F9ev8AzZSkVX3wb3rWZrb81BmXRjTtba/mU7p3NLrAENDefqgEWA1hipx4jtoTqmsk75BHkdETryITKWcuAgafERe9ttV2nnBa5sN8rRrIdz/soEyap3PFO8yuuA0i97WCRLVYXRGMGjZNIG3a1x8Ivpc+aYNqXGMMaBd/M8h/zVR1VUxPka2JrxZ2UucRY+dh/ul2SZMYhU97cwsDTTFseUagAi4t6FKppJGBkri5wABcA2wB3tc+VlyjY2Suqc7x3csd9eWh/VPXvpXsyRjMS7O50hs2+wsOduXLnqmgryDOJEFrpLa7BrSU9panv3DuHXd9kkgn4qHNCe/MscsgJOtzfT0RKWeenqo2VAayW92lp/MckmgTLkwuZhT4Jn99mAfGX3u0fe+KDBVsdkMrCYmlrZor2IHJ7HDmiMLJ4RIG3JBt5X3ULh0h9oNDM6zvF3burfsn9FmXk0M+puCMdlmpafDqqSWUOjzU1RKQ4yAbsLhoXN09QQVeF8vcGY/W4bXOpLyveSKqCG9252Dx6ci5l9fLVfTdPMyopIaiPVkrA9voRdVtUVNBSkErpXOaiAgpBCW46oZISaAS4IRCI4pBKQxBFkgoh1QyECE3SHFLskObdIYi68V4iySgRwpJNko+i4RdACM2q6TovZV4jRIAZSUorw3QB5csuryBFEkbdhVr4NZarVae3wlWrhAfva2w7M0ujT3fyvwWccR6yn1WkP8A5X4LOOItJz6qeTocCvAG6M0FcG2iWDZZiwLADnVB7QD+4ShX+E3NlnnaCT7FImuxopHBzP36/mtohDhSMyjksb4MF6z4rZmFzaVuXopzHHo5HJUNdexTsVcgbZzUCCZ9rlqP7S3ZzQqCY2qKlhBuxQGJOiMLjaxVgmfA5pu0KAxMRGF2VWRIsi8DEZr2lm+ZbrggBpWeiwrAmN9vaWn6y3XBCfZmgdFXlHEluaFiVDQ4rhVVhmIwiekqozFLGfrNIsUS5buo3F8Tgw3CaqvqDljp4nSuPk0En8lQuyZ8K8S4Q/h7iLEMBbN3vs1XNTh53cAbNJ+CgMmV7HA3aHany6qc4gxObGcWqsXlaO9q3yTkDk52v5aKuNnfa4OhZy5FdaHRnl2SVRd0jpGg2ecwIGwtsmsETmE5SDp12QoaqTu3NeXb+HVcLpMj3F5JtzUyJJ073RzsabZRtfn6J0ydscjn5h4uZOlyoSKZzS4kXytvojMc5z26c9khokJaITOdJUVDZ77WNgP1UZUU4a6zJow37EZHzUgHi1w0OI3I5JtPC2eFxa4H0SsdEO65lsWlttE9oyHNLDvcC6Yta8PLeY5FOaQHOCfdzC6kRXYqrkLAGDRzgAT5I97UkcLDbNYutzCZTHvKxwOx+SPDOW1cZy3toB5JE12PBnJLCLA7HyTRziDpE27dbXJ8rqUlYWhndmwDSQDzuoyocG1LJW6Mkby5X5fiopkmh/BUSR0D7mzyLAnfnYItGXAseXOOU31NhfzKhXTExtYTazv0UzRkMiPePIda7Q4X38k+hEiyVkbQXRsJO2U3HqbJ62nhqqR5DAJw2webn/t0TODuswkqHANBvlGpcpmgzTS+0wwOjOgHMkeQChKRKKHeHFzcPs5rhJC0kjbl/f8ANQF3mpgmY3xl4I8he5/VWfFZXNppyxhhc5oaWnoLDTrcAlVGgbPPTwiMhzruH4/8Kphy2y2XwWyGd1LitHicVx3Mscp1tmaRqPwX1ngA/wDtnDDfemZa/S2i+acJwaTGaSqwiADv4ooD3o1952XboN19R0dM2jw6npWathibGD6Cyrm7IMURZIJRHBIICpXAATuuJbkjmnYA3XQiSjEBCcEAILkm66UlACrrhtZcSCUgPEJJsu3SCgDxsuXSSSuXSAVdcJXLpLjogDjrJISSV1qAoUuFdSUCKi8eAq0cIt/e1Wn+4VaeER+8rdDsyM0l/wDLfBZzxGLzH1Wjyfy3wWc8RD6U+qnk6JwIBoslhJaUsLPRYHgHiWedoLb0jwtGgGqz3j0j2Z90eRoqPBkVqnXqtdDgymbpyWW8Ige0C3Vai9wbA24vopTHHoLT1DLatCK+SF27QmdPNDexajyGAjTRVUSByNgc0qCxOOPuXEOUq8R8nqIxGMGJxD7qyKIsjcBYBXtIN7uW8YIGimZ6LCcAjLa9utwXLdMIJNMwW5KrKSiSsjc+gWXduGIHCuynEwHhslYWUrATvnd4rfAFaiy43WDf+Jd80nDGDxR27ptUXv8AXKQPzVUFckSPmGKpcIy6QBzR5cuaj2s7qRzHG7Dq1yeZA2ONtxY7pk97xJK0nwi+i6iKWJebyWGjQjteJY3tNr2G34JlG6+hOiJE8tnFja+hUiB7Nq5pG4IRaeqaxmV7yHNILSvZGmQ62I3HVdhjjY7M6PMfM7JEgkIdfPnLemXQlKmmc4guAvye3Q/HqjNcxoLnENb1PNPqCWJ81nm0Z0ALRoeqrbosjG+BhHAXMDXsHeuIbmtrbmhFhpmkEXaTb0VmadXMMcYdsH9UzrMPc4ZSLvkIAaNyVWsnyWvHxwV8xH2uQb8wfVHjilE7mxjUN18x0VpwrBY6mriaIg5paQ/mQLc/ik12HjB60OmaTE8ZQ8D52/NReZXSJLA63MhItKfunm7ORvqwpjPHalFr52OuD5KYn9mbKX09RHIHe80c/wAU0fGxzy0NIa62l9lOMiEoENncZS5wzvJzEnW5R4qiWzhmIdmBJ580qWnMcpAbdt976pcVLbK8ttm2VjlwV7XZL4e7Vrpr2tfXXQeSsVHVyva11+5YDqQToOg81W4InyPY5lyQcpaPL9LKw07Y5Lwh/eStGYRjQHyJWeXJfFUPa2pkn7upldcxDIAeWp1/50RaKjhY1s8Ia1mri0aXP2fxXXsZUDuu7e6Q271wAcGHWw0O1t9N0CQ9xDTUf1nObm03P/b8lD8DNW7H2l/FVXNM2xkpRFlO4LXZv1W+30WQdjmHWZW1snidlDQT9U3P6LXtlW3yVy7PFCciEpDkNkQTkMmyW42QHOSA8XIbjdeKSgZxcXikF1kCFFIOq7mXLpDOFIJSydEIlAjh0SLrpukhIBWq4Uq1wkuFkACIXmrx3XLpjFri5dezJCKtJ7hVq4Q/mSqrJ7h9Va+EB9OVvh2YmaPIf3f4LN+IXfT281o838ufRZtxB/MfFSydFkCFARGpLUsLOWDmHms549BMDgOq0WHc+iz3jdwLCPNNdgQXCMRE4PmtJlt3IB6Kg8KtHeAjqr/OB3QBNtE59ko9DeNkRcNSE7dDG5ujk1jjaSBmToRG2hUBjOWm00eFFV8L2wuObkpiaGQbFRFc2UQuvfZTRFjHh9rxXtvqC5bvgbSIGX6LC+Hg4VzM32lumDutTsHkqcpOJLvaCFRO1XhV3E3ZtjFLBEZKuOAzwNbqS9hzAD1sQryCjNNiDbQbhUJ07Gfmw/WNzR6gJsQT9IRodHK1ceYS7Au0DHsMMfdimrZcjRsGkkt+RCqrSHHmL3uupF2rK2Nu7IlDRpcozYbzFpFyeg2RGSAkNiY1pHN2pCl8Gon1lWGZrkOF/hunKW1WEY26EQ4ZPPl7uG/K5OilYOGZ5NQY2Ec3An5KzuMVFCRYNDRrYbpgaqqewyPkbSRb62zW8ydlgeab6OgsEF9xDv4Uqi/NLKx56oRwWppn+FocBvY6qSbjlG2Qx+11FQb2vECbpctbFKXNjqXxTMNnR1LC3W22uxT35PIbMXgHQ0gfMBKzN1aVaKXDaKOVroKdrX2Ic4bgKq9/K1wflLHj8PgrJgVQZ32J1JVOS3yaMW1Oi50uFMOHFzGZHuNy4DVyg8V4Ykqn66jYkjYdFf8ACqZrqFpzHM3UX2Vbx+rlie4xtJaL3sudvkp1E6rxxcfqKHLwZQwT3ne30Yd08pOGaGWT6V0j2N2Z7rf91HV2IV1XViKIuaPsRi7z/ZAwrGYRWNhFHPVOeTbM9rb/ABcVtSytdnPfsxfRfqPgfBaiBjhRxtkt7wbofUDdMa/srpXF8tBeFwFy1ty34A3KfYFjWA10rIYqypwmeS7WipHdBxBsQCfCSDuFeKOprKCpFHieWRsg+iqY/ckH6H/gWSWTLjfZqjiw5F0fPFVhGIYRWyMmjvFq0kD5o9LUDKMzomyt917g4fPkV9BYjw7S15790TXgakHmDodfisT4gwV2C8ZyYcI2yUrm5wyQbA/n/wBlswan3OH2c/Ppvb5XRIRVENRRMAk/eBdpDNA42vvz01+Cimxd5iWa4eY3BxtysD/dAmzRtjYx1yX94fQaBKhzGeQscPpCy+uvNabMZ9F9i7my8MYjMSC81WU+gYP7rSnLPux6jbScAMmDSHVc75STuR7o/JaA4qBTLsQUJ7rJbkB97oEcJukFdJ0SCUAcIQylkobjqkBzkkOCVmSL6osZyySlpN0Ac3CGRqiHZDKBHCkJZSSkBzMvE3CSUkmyBnikrt1y6LGe3XrLw3XUWFFXk91WzhD+OVVJPc+KtfCAPfFdCBgNEm/lz6LNsf1qbea0Wozezn0Wb45cVdz1TyFkCLCWNkMG6I3dZywcRbH0Wa8dkhunVaXANHeizjjht7jzUl2Ay4RuS2/VX+dpdEBdUbhRoa5vqr1M0uYLIn2Sj0DhpnEjVOzTSNboUinglvojysma26rJEdMJWqIr3Sdy6+1lKzyyAm91EV8zu4cCOSsiQY24fzGtYD9pbjg7T3DPRYfw47NWsuLeJbfhBIibboqspOJMWNgbIzLW1Q2uuwJY1NlmGfGHb/Qil7ZcRlDCGVcMM3iGjiWWPzasdsQQ5fYP/iE4YpazB8K4kdEx0tFMYXg7yMc0lo9A4fNfMNRh8VRROMcDYpmm92CwcPRbMeVJJMn7TktyK7TxZprW1uPzWm4ThEdDD30bdXga+dtVR6SlLaqNrm2e5wuPitigpGiliYRsNVDUz6LtNC22yo1wqnF3dMaXcri9lFNwKtrJRLVVsb7G/dn3fwWoDCmTssIwfKyby8N28TKWx+7Yfos0clLg2vFfZnR4TndM6QVDImudms0AgfNSUdGKOgqKP2mKo9plMsrpYA57nfjYKw1GEVTSf3Zxt9qRIhwqZgzytbG0cgFP3G+yPsrwiqtw11NGWRue9r9S1zbBvpqrVwrhZBbJINzcLraYTyhjW+G+p6q5YNQ5C0BvSyjKVl2PH9RZsKhb3YjsqtxNhFRFJN3ebI8EtLdx1V6oKM7lrgOuycV2HmWHxDbYrDNVKzq7d0KPnqna/DK1zqaV8T72IkY3VLoOGop69kzZpIXMkErHNcBkcDcEadVqmI8MwVRL3QBsnUAa+oUIeG30j7sjI/oJHyur1kdcGKWnV8ocnhSPFMNipMWxqeop2uMvduIsXuOZxJAuSTzRqXAabCZTFhtdVPpiL9zI8uDT5X5INNHM1xaYXuA5uAKn6OKV20Zb6bKn6n2WKMV9qJjBZi93dStIBFtQqL2o4XEccwzEQ3I58bmZhzI5fgtEoYi0tLxY33soHtIpDPglLLl8UMtx8UsKUZ8EdSt2NmDzsPeh3Ju39vyU/hfC1bXYI2qpZKQ1YaSad0lpnBpvcNtY6HrqrBhfAdViLaeaRwijfYi/O+v6D8VK+zfs3iikayzXRzNZpzGy1z1CTqJkwaKWRXI3LA8PZhnDuH0UbQ0RQMHxtc/NPXI5Pgb6Ju92quOM+xDtkB51RXO0QHFACCUNxSykFJjoTdIJXXJBURnCk6rt0kuTQMXyXEnMuF2qkI6UMrpckEoBHdkkrvJcKQxBSS0pd7LmZAA7ELlkopN1EDoC8SvLhCAK2/3firfwgPpSqhJ7nxVv4Qv3pXTgYGX+o/gH0Wa4+f3weq0moP0B9FmuP61nxTyFkCLA02SwEht7+SIFQWMcw+670Wb8bGxPqtIg9x3os1441P8AmQuw8A+FdcvqrzKDkFlSOE2nK1XpwdkFglPslHo7TmVp0TqR8uTYocLpG28KNJO4N1aqyRDVEj7m4UNiMn0DrjkpypnGvhUDiMrXQOFgrosrYnhpwfWx/wBS3HCWjuG+iw3hkg1sZGniW6YUPoG+ioylkeiQvbSyUy9rpJuDcnRFY4FuyzjKN2r4PUYz2eVjKYZpaVzakN+0G3zfI3+C+YMKwwTSVOdvustr1JX233Uct2SNzMcC1zTsQdCF8n8UYeMAxfF6JrSzu6l7B/SDp8ik78HR0kk4uDKE7DWHiSiiYBfvDnsb7arQmNu9rfq30VH4foZjijsTLjkzuaAeZy6n8lfaOzy0k7oyO0kWQjtkywUMAytNrKcjoaeSK7/E8ja6iKSRmgBsOilaecB7yTvtZVJ0dCEbQynw+IPc0sDTys1VrFmQ08ZLyAbaAc1cKura2JxcdAFnmL56t752O290E+akpJukE40g9BhbxGKuXw31DegVtwt0MWV+h1We1fEwipRCXhsg/wAMusUbB+J88jY5CY3E6BxuD6FSdkIuKZt9LUxy6MNjtZPaiiklpMrHkEhUzB611TK3JodFKY/jmMUsPdYXRxvyi7pZXmw8g0an5LHPK26o6UYJKwGOUNZQUraxkhu0gH/fyUfR4lTYlGWOs2YGxHmltxPFMXwcUlfE2NznAuc24Fgb6X1VOxRkuC4q2siuYXOs8dD1Tg35IzpF3ioY2vJI/RSdPStFi0ho2Vew7Fo6lrSToQArTTSNcdxryU3NEdg9FO7ICLGx3sorjClE/CdSSPEwBw9QQrFG5scYZ11TbEYm1FIad1sr9FiWT6+CucbTRWYK2hlmFFT1kYmow3PHbUEtB/KyrPEMZHG1KGtJ72VkjfimGOQjBOKvbqY2hrwZco+q4Gx+Gl1b8Kw1+N8U4LWOF44oM7/8rjZWRi93Hk1xlHHDc/CNVd7g9E1kTmR+pTSRy654lgi6yG5y64oZcmI4SkkrxKQSoMaOlIK7mSC5IZw7pBSiUkoA9deuuEpN0AecUlevquXQM7ySbr10m6APOKQSunde0QI4kpRK4gDi9dd0XNEAV2T3R6q4cI++VTZT4R6q4cIG8hXUh2c9l9qP4B9Fm+OfznxWkVP8A+izXHDes+KMhZAjglhCCK1UkxzDo13os040sZR/UtLjH0bj5LLeNXgTj+pC7AecLN+jbYK6d6WAAhUzhM3iaVdczdLhRn2WR6HDKoW9xckqGkasS4zFbVq7IISPdVZIhqqRmvhUFiJjMDrDVWCqbCb6KAxFsfcO9FfErYnhfKayMj7S3TCj9A0josO4YY32yOx3ct3wqL92aR0WfN2WR6HmUOCUyOwC8GkOsjZCAs4zwdY6LAe13ByeL55GgH2yBszR1IGU/kt4GbOVm3bFhEtThmF4nTuLJ4XuhzDo4XF/LQpPo06aW3IjAKC9NDDBKMhzFzWkWub62U9SyhrXN5g2Tesp6qUZXxMc4WDHW1CRmLcztidVHs3S+6ybpawE5rgjZS0NYW6nYBU6llLJMmtrqZMj5Jo6dmhfufJUTXwb8MuOQOM4o+WQU8byGu948yE2YzvIcpuG7JkS+V3teW+dxOuzW30+SVU4zS0bA1hbJJy10CshGkVzybmMsQwd0j87G3PmFGnDKhjgO4cfNoUy3HZ5orkhjOrRonMeITNeM5kYTqCRZW8kFjT5H+DYzLhrWMmnebC1smvyCulHiT6xodFDI0Hm5pF1VMPr3SEgkl3J2UXVpon1Erj3VLUTlrczg1pNh1WZwSds3K3GrJIUtS5ocGm9766BQuN0XtFPJFJFc2s4dVKnFqmkphPNRzsgccrZC02v0Td+PYTXNyOqGCYD0JUHLkm4UuyhYPWPpqt9HK7xRmwJ+s3kVomEV3eOZrc2sLLMMWfD/wDUUM1K8Fpk7t2U9dbfiFecDLopu7dtuPRRzKlZHDO+C/VUl42ObrpcDa6495dEy5t4L36JoHufAG7gbrtbNHT0j85sA0N+JNv1WDHyyczOcVoqzG6yKqpYHyU/eZA77AB005LWeC8NywTyN8RiaynuPLU/Mqnh8sVPLC13dkncDl5LZOBcHgp+D6V0Rz98XSE+d/8AZdOCp2YtZl/acfkYy0b+QKavpJuivLsPYBfLdN5MPaeS0e4zgbEUd1LL0KC6nk6FXs4aOgQX4Yy9ixP3R7CimCToUkwSfZKvIwdhOrV44My+jQl7gbCiGnk+yUk08vQq+jBozu1cdgrLaNS9wNpQfZ5Oi4YJOhV8/YbSPd1Sf2K0fUR7gbCiGnkPIr3skp+qVfm4LGNct0v9jsJ0aEe4PYjP/Ypj9Ur3sEx+qVowwZgb7guvMwiO/uJe4w2ozc0E17ELv7Om6FaO7BY73LUsYTERYMCN7FtRmYw+YnYrxw+a/ulaT+xGcgPwSf2RENMqPcY9qM3OHz/ZQzQzg+6VpjcIjIPgC4cDYTsPwRvYbUZn7DOeRXvYJ/slacMBZ0H4LowOPN7oKN7DajBZfdHqrhwgPEVT5dh6q4cIblduHZyWXup/gH0WbY1rWn1WkVP8ufRZvjH86fVGUsxkcBZEbokAaorRfRUIsY4iBdG4Dos44wwuaaXMzUg3Wk05yxuKhaqWGWscyRgIIWDWZ5YI74oCscLQPhiDZG2VtuwWuh01DExpdFaycdwyQ6utZPDqo5Yby1dDiIwELszYcps5JihiBt3lkuWCPJpIrrvwMiKlsZB1VdxRjRC4h3JWKphbr41XcViIgd4uS0rorYrhZtqyMg38S3zB3D2Zo8lg/CbLVUYvfxLdcLFqdvosuXssj0SNrOuUbMCAgOPhuEhr7HyVJIdZWg3VQ7RaSrrOEz7FC6YwSiV8bBdzmgEGw52vdWd0p2Xmu0SZKEtslJHy42sdVzmloKWarrHnKyGJhc4npYIGLYNiGAVYwvFmsFZFGx0gY64aXNDrX6i9j5hfVMUcEUrpYoI2SO957WAE+pWNdtFEI8Xw7FGi3tELoX+rDcfJ3ySUaRs/9HuSSqjJwTHMHnYqbw57XYvA5x8LhooYEPafuo8M+UMeNHRm4VclZtxyoTjOH1Bo5aGB5jliNhbY/wDAqbheF1rsf7rFIXRxRuD8ztWvAIuPwutVmdBVNhxAakgNeEGqoqedly0G+zhurYSpDlHkl6Q8G4Dw9jcVXPTmCN4l7m4LzmALWtHM3GidU3aH2b1GK0sk0kkLY4XDvZqVwYLkeHS5vvyt5qox0jY5MhhjmaOTv91K0dDw++Ytr8IjOmgEbbfkpqvI44FL/IuFL2ldllNjznxTkfQtHfiifkLsx0Hhve1tbJ7L2zdnVNxDO9jqyeJ0DA6aKlOV7rG7QCQempFlSncN8IPeZRhkLbnbJ/YqWpMF4biLW0uFwNfbdsQv+KHtNEdH/wDTLzh/E3BeM4FgsLKyJrJXOn7iT3mZW6h/TU897aXXz5xlgtVX8Xtdw7cU+TxybXdckm3QCy2mDAo54msLSGcru2+CDXYVR0jHRU0QD3DV53Kzpxi+CyWOlVsxbAcImZUMp5nmWQVJe55HvFavT0YiqGSHkAFEUOGsjxxvdt8DNz5q2PiGYhovcrHqp8pInp4VEdR5vC0HZPH8KYpxTh1V+yi0z0bmTCMm3e2J8IPI8/gmsTNNtlrPZ7TGDAJqp7bOqJdPQC353VOnjulyVavM8Ud0ezJKTAMcqaptHJgdYKgGxa6EtA9SdFumAYOcHwCloHkGSMEvI2zE3NlL96LbobpRsulGCj5ONn1UsySaoG9g2QHR66pySCLrmUFw8k2jLYAxDRIdC07hOn2CRa5ToLBCJoslGFttgiW1SgEUgsQ2naeS77O3ojNNglDUJ7UQ3DZtMOi46mF9k6BXdwUbUG5jH2cXS2wAHZOC3UpTRcBG0e4D3A9F0QN8kRxKSD5opCtiHRNAskshaEpzhdLZqFEkmIEIylDNO0akJ3yKFIATunSFYERttYBdEQXM1ilgoodnRE1eETV0HVd0CKA+XJhoPVXHhAbqnyEOAseauXCA3XZxtPlHMZdav+AfRZ1i+taVfsTe5lM83tosmxTHGRYkYp9DyJRmkl2WQHjRqigaJpBXU04GV4unoFxcG4VKaZNhov4T/RUmvnczFi0FXJ0ohpnuPRUCvqGSYg6Rp20WDXpSwtAWPCqy4yOOhUxSwNnmtnsCqrhTXShuXkrBDI6meHF1ua8hjebHgkoMadDqroJIpAWyA/FB9mnc3e/xTOpxUEjM/mm1JikstSWRkkXW3D6rKLjB8sHMJVQSsvcqvYm1/cO8XJWev75zdQLkKtVtJWSsytjNivV48tw3SH2F4SBFZED9pbvhg/d2+ix7hTA6mOaOSXkVrMdXHRUozvF7KnJki2a8eGc+EiVJsEHMM9k0oa5lZfKdinjmWkuotUGXFLG9sjzrXuN0u/hv0STvcJWwISKjzG3cs47aqVjuEKKbLd8dV4T6sP8AZaRG7UKgdsTr8GUzetW3/Q5BZj+5Hz1FU20J1sjM11G3NRTiY53NvbVPaeS5AvqotHRiydoJT3D6YnQqRpn54zGdXDQhQVPLleJOd9VNMDTPHPEbX380kXphvdF3MDwU6iMZaCI7epRBTxh5dc2cNhzSqehY+pGYFzefiKRYuOQ8Tyx/uAdDuCpOmrJWOH0DDyvfZJ/ZlEG6w6+d0VlHBEA5rLdBfVKUEzRGbLBRVbzF4yBpqmlW4Sue+5ItZAa14DQ1jmm2uuwTpsGdoGUi2pWZqi7dZG4dSWe+XndSOUmS9tAnTKcQtdYZS47odrNd10WDJLdKyxcI7GRnyt+sbLdsBoRQ8O0VMfebEC71Op/NYZStDqllvrPDRp56r6CD2tYGjYCy2aRcNnG9Rk7igMosdENrTuU4Ja47LgyhbbOUcDbt1XSLDRKB1XbaJVYrA7uRGtSsnkitappBYLu9V3KjZbJLtE6ojYLKeq9bRK3K4QgAZJCWwr2W5SrWCSQCSQlMtlKQ4LwupCOv90hIY2wRSNFwKIwLhYLsZS3i+yS0WUSa6OOJukNFyTdEOpXQ0Ab7pCBBu66BcXSiReyU23NMYkNXCeSI4gaIBegD5RYZ436gkArRODX54w61rqk0lZBNma9tnjcEJ9h3EkWFzmC/PQBS0mojHhs5lGuVrWugcCARZZDxTgUVXVOcwa+SvFHjctfTPe0HbYhVzEKpntZe/QjkulOUckS2Bk9TDi2DTF0Zc+MHYq2cM8Qtr2iOQ2cNCDyTnEJ4Ky8WUB3kFAUeHw4ZiDqovy5txdcaWojhybYu0S4LrjBIw5xZ0WZxiokkkDWkkuV+/atJWUbo2OzWCq7J2U9ZIGta7oFXqNQ5RTSHVlp4cgZHSfSt8ZCZY5VSQTeHYLuDYrA3SQ5BuQUvEizEA4xWXM1DUoe2vJPiqK4Xul8RJJPJTmC05jd3kjbXQKbDpGeIN0T8iqbFljFvguXo/SMyn7kipph8Tq2xNLm6qJGOMbGSGF1lyWKpfdsp0TSopGx05Jbb0Xo3jzqkKKafJYMJ4pLrBsZbysrH7TV1zPAw2PVUnhqha+rZm2JWzYVh9MynBIzaKb0s7vcdzBqo4Uq5I/h6kngac97nUqxnV267laxtmAAIZOq2xTSpmbUZ3mnuYtw6FKaCW67pN7gJQeByUjOcbo66oPa9Y8I0g61Q/wBLloIAJus/7XrN4Tox1qx/ock+izF96Pm/EIrHN0Q4JbWLTYhSdZF3jXaclAyZoH3GyUXfBvkqdonYpgWXuL/mpKjrrXYTboqtHUBzRZ1iitqi0i+45puI1Mv9JicZs151VjoainDRc5T9q2yyWLEHNeSbi/MFWDDsVkBDWSmx1s5VSTjyaMc03RpTjZgf34c08/JKp3xEgONzuDzCq8WIh8AyuOu9inVNWNIsZba73VEs3BsjHku8EDJoe6a/K73jfcp3kZDHc3va2qrVJiWSMEP57hSLsSYYfG4F35rHPI3wX0kPu8aRqdOSZSyMGl7a+ij58WDnlsIzkb22CQx736yG7vRUbfkCdwgmbEqNhOhmYAP8wW9ObYn1WEcOMzY7QAf/AMiMf+4LfXt1K6GmX0s43qH3RQABecLIgGqVkBNyVpOYAaSCnDfNcyC6KGgKaRFnmjVEuAkXHJcBJViZEWXaIRN0o3SAhjo8F1dDbrpbZIQlcuur1khnDYjVc9EqyTayAOl1wkZxfZKtokEEapDR0kFeNgEjXmkl+mig2SR0nVdLkPUnVLA0UQEOJDtF4OKWQCu5LDVMdiCS66EGE2Fyj26CyUG7ABArMFxPgh4qTJTizvLms94iwiqw+ra8tc3Xfot6krQ9umpVJ4oofbmEsvruCFLU6eMpuUDnuDoYcLY/FFhpgqspeBo5QWN4tSmtkkY8ZQOqj5MJroIyYwXM/AhUzFmVTKju3FwBOxXLefPFe2+iN0WJuMwXd3QH9SjaltRiMnjlLIz5qCZOKZt9yiUmIyT1AaCQDpdZVicfqZJMtbHUWF4eQyS77bE7qHwqpfiNdJtoeXJT9FgLa2B0sjs5Auqy2KbCsfe6nBDToR1XRjt9uy2LtFthwsS5hs62hCHAyrpKjK+5F9CpfAmyysdUStIGW6KysjlqpInRXsFGOGM8djHMNUO5ByeJIfV20sgQVHd1ZY6PwW6I000Qfowa+S6GjdLYwQxqKguv4VX8Sq5I4za/oVaZ2xmO4byVQxiRmR1t10lTBlj4SkMs0RtbVbNQaUw9FjHBnikistqoW/u49FmycPgtXQe+q6WgnZeIsuNdY2VYzoaQ3VcdHrcJT7gaJcRzbpAJbdo1KyrtXrHz4dSs1yNmzAf5SFKV/aDDiPaJT8G4EWyNgzyV9UNQAwfw2/GwJ+ATXtDoTU8MuqA2/dOa4kche36rdDB+zKTXgjGdZYoxJzczHCxKjaulDmXAupjJlu06EID482gauRdM7tWiqlhiJuLC/NHZIxwAfa6fVdIfESLKNMJaSei0RnZQ4USULITbS3xT+FjGgEFtxsRooSF7gLAqXomiQgXVc50i3HC2STal7WgRtFueu6cw1NTf6KHluTdKp4MrdGi3mpejos9nAXusUsqXg3LE/kRTTVmUaZXnmSnzBPILzyOt9kaXUjBQsG4S307WEeFZ3kvouWOuwcGXQNbYDYBPotSBbfn0TJoINxoFIU4BZc7HRVssLDgM4psUpKktuIpGvA62K3unnirKWOphdmjkbmaV88URyyBx2BA/stJwziqm4ZoKGPF3d3QVM3ciflA8jTN902OvIrtaPBv08prwzgeoyrLFfg0AiyTmslF7XNDmkOBFwRqCEEnVQfBhCh6V3ibh2u2iI0XdqmmRaCtJJRAktaAFxz8qdiFOI6oVwHIZdcrg3ujdYDlrguk3CAHeaW12inYUKsvXsNV66SToSUAezhd31SBYnZLGg0SA8vGwGy7cJL3AbIYCDfokZbLpcSV0uAVbJCcuq7caAJLnXKTmGcpDF35ogNwghFj5pAzo12CUABqVy5F0nPqmRMPPFFO3ZzUk40ysyhpaTdZTK58FOZHvJ06pzw7xXhkUndVMjWuYdcxXTcUuzPvNLxNtO2gdK4ZHdQsnxp0VVK8gXe3n1Vq4i4sopcLfHS1DHB4012VIo8Nr6qA1mcvG65GvlCKSE4pqyHjwaurZjliLWdSncGGPopblt7c1ZcPxiKOE072ASbG6nKbC4qyjfI4gucNAmsEM2OrIqKG2B4gwUT2ZgCG/ioWhpjW8UvEkZLCND8USLD56KueyNxyuOynqWlZR1MNQ4WeTq6689DPLBOWJvhFiaSJCqf8As+sjpWsswjUrtHUYU6pLDYyN1KlcRjoqmJjnuHeluihqejw6mL5O9a6qJuWgro4dVswTyPwiMZJkpNPhQeLNAKbSOw6fwMFij+y4fPA2d4DTzCq2I4hBT4vDFSDMCdSOS1YNXHNpY5odkiTqzGyMsDdSqbjTWCMm1lcaiamLA593PI1N1UcbfC9jgwrq6OUpQuQFh4LAEkVltND/AAB6LGeDG/SRLZqH+XHonk7LF0HdeyS33/VGy30sklgYC9xAaBcknZQGKDMzVmHav2i03DGETYJhNSHY3UtyksN/ZWndx+9bYfFQ/aH2yw4b3uDcJSsnqhdstcPEyI9Gfad57DzXzlV109bWSTTzOlke4uc95u5xO5J5rfg0zk90+imeSuEaz2HUTpcVx7F3gnuoo6Zjjrq5xc75NC3aN8M9O+kqGNex4LS1wuCDyWUdiLGt4LxOS2r8Q1PpG3+60o3Dg4bhdZIzN8mP8T4DUYJi8kD4yIHuJgk5Pb0v1GxChu5a8W2W/wBRRUOM4e6ixCFssTuR0IPIg8j5rKeIuGKvh+pJeDLRvNoqgDQ/dd0d+fJef1ukeO5w6/4d3SapZPol2VCan8BDmhwGxCgqilcAXBlgOStjoy4e7e6Z1VOLHLtzC5cZ0zpShZWBEbAtGikKM924EnREMFpB4bDyR4qcukAGvqpydojBU+CwUdMZ42OFzfkDorHSwNjbl0FvkoXCnvi8GjbKfjIsC9wsVzp9nSh0SEWQx3zDyTWpLg6zG38ydEWN0bRoRdN5pC+Q3Nx0KrRNiWkFvLVPKYGwFkybYAbDqlQzVVZWswvC2h1Q4Xc8+7C3m539uZV2PFLLJRiuSmeSOOLlJ8FowWH2zEcrBmipyM7uRkOzfgNT8FM9otCajszxSCJt5KeIVDLdWEE/K6keHsHhwvD4omAkNG7t3E6lx8ydVKV1OysoaimkALJonxuHk5pH6r2+DTrBiWJf3/J5HUZ3nyPI/wCin9ifaF+0sOj4YxWovUQj91keffb9j1HLyW2EEr4NwKrlw7Evo3uY6J2jgbEEFfR3BPa7G+WLCuJ5AL+GOtPyD/8A9vxWDV6Np74LgjjyXwzZgLaAIrBY7IcT2SxtkjcHscLhzTcEdQjNFjdcyi2xYQ3tSxdedqFFxFYAN8kogLpvfReDTzTSodgyDdeFxzRLJBbe6Bo6H3F1x79LLmo06LhBIQSOh4GiWXaINrFE3KEyNCXO1tdezErpaLr2UA3CCJ4Ek6rxaF2/lZcJG6iySBlpJXg3W6VddBCiSOWRGaOskblKaLanZAhTje4Q8vj1Xu8GbReY4blMD4fxbEXdwYm/FUeWB1VVZNbE6lWf2KtxOrywxnKTuVaaXhCGCkD3tvJvrzWPVeowx8N8lOHSZcqtIzmow6SijbIxziN7XWkcE4mavDDTu3tayi6/CjYsLbgI/DEJoKs8m3XI1OdZsV2VuEsctsgmJUMseJOyixcbgqfwieqggDJTdOa+l9pqGTR2IC82zXWNvCqY62ax7YPkjOktyHENPJJIZnakoGJxy543AG7SEV2Jsp4i7k1R1NxFDXTvjIBy6Kj2X90yhSsscbmzUzXO/iMCbVNFBcYgxlpLWdZIgnLtWiwKRUTObA+IOuTyRDJuwzh+CpNxlwP6UxSwdzNq2TQEciopmBw09XJM83IOiXSztDGAu1Bup58UVRTidrh4hqsP6b1FZHhn0bSsVcOe9nH0VYxOBzQStD/ZpkbcWsoHGsMLIy4WsvqOOcaqJNoe8Gx+OOy2CjFoBcr55oeM8P4ejc54NTM3RsbDYX8zyVe4l7TeJMeYaYVhoqM6ez05LQR947uVsdJkyu+kJ5IxR9BcQ9pvCfDTXxTVvttY3T2als9wPmdm/ErAuOu1TG+LJHU0bnYdhg0FNE8/Seb3fW9NlQTLqSSSm8rwd10sWjhj5fLM8srkAmlLiSSmrHXlt1RJSEGMfSBX0Vm/diFSDw3i9NfWOta+3k6Mf/qtZDQfNYb2KVOTEcapL+/HFKB6EtP5hbix2mqdAxQOQ3anh9nraZ9JWQsmhkGV7Hi4ITVoulZS03CNtqgTooPEXBFRhWetwwPqqDdzBrJCPP7TfPcc+qp00UcrLNP+ZbzDUvZvsqxxDwTS4q2StwfJS1p8TovdjmP/AMT57deq4Wr9N/zw/wCjuaX1D/DL/sxt0DmvvlBAPJO44Ge9YByfT0VVQ1b6WsgfTzsPijkFiP8AnXZFiDXO8QHkVw5WuGdmKT5QSliytzAE6KXgy5Abi3omUZIbZrrDqjsqGsF+fUrJJNs1RdIfPfljvpqo2SqDLkplX4o1rQM9/TYIWEYdiPE2JGmoiYoI7d7ORdsY/V3QfotGDSyyNJIozaiMFbY5pW4hjWIDD8Mbd51e8+7G37RP/CVrHDvDVLg9GIogXPcQ6SV/vSu6n9ByRcA4fosFom01LFlB1e92rpHdXHmfy5KfFgLBes02mjpo8fceZ1Gplnf4FiwbYLk7xHTueTsLr3JRHEte3D+HK6pLrd3A91/RpK2QVsxydI+So574lK/kXuPzVjimLom6+ip1C/O8uvc3VkhcO7tfVbIrgp8mk8IdpuNcLyRxCY1VC3R1JK67bfdP1T6LceHu1zhDG3NhmqThlS7ZlT7p9HjT8bL5DkkLbkcl5tQ/L4HEPGrf7fFYs2hx5OVwyyOVrhn35FJHNGJIpGyMdqHNNwfilEXXxVw1x7j2CStkwvFZqfrHmux3kWnRbTwx2701Rkp+JaLunbe00wuPizf8FysuhyQ5XKNEcsWbWGWXbJjheNYXjdIKrCq6GriO5jdcj1G4+KfE2C5r4LUIdohE2HqlO1KSddFEmj2a/JKskNFkomwUSQN/MpAcbFdLsw0SSLBIKPB/UrufWwSC02814NISsixYdcpQBJ8klrdboo1QAO2qW1t9EuwA1SHEeiB2dOVuySSDuUg9b3XLZj5JBR4kX0Xmkg3slWb6r3kgZ8wYZHQUMTRK1uc+StMeHRVtKXste19FnMlXUy1TZWUznRsO6msG4qqjikdM9gY0m2ULja70xybkkfRsHoWZY3XSO1mGONY6K3PohT4I6lgdKxuvorXO6FleZpLAEX1UViONUr3imY4OJNrLybw6jJP2UqSZ5nV6fHFP3HyVuDGBSQv9o09U3psRZXlz4ni2+ic8R4C+fDC+EavCrWGUNThsRiJsvR6TRQxxdvk8fnVPauiRxCVz43RRnXqhUcEdDAXht3FEgp3y3LjzT/2a0QO9loy6f3FtTMvuKPFD3DppHNHeNtbYKUkMJIOXUjdR8MjRCDawCcOkbJSZmkac1y8eCeFtS5BtNcEJW1BpZHWN/ForlwzC+toWl7rNG91nWMYjhEDQX1Dp5wblkew9Sq3iXF+JVdJ7FFUOp6XnFES0O9TzXQ9N/Tmqll96K2p+X3/o0Rml2a/xBx3gGBNfS0rm4jVtGrYneBp83bfALIcf4zxTGi5sswggO0MOg+PMqtSTP3doOSA6QOJJNyvpGj9Ox6aNdv5ZCWVyOPkJJNyhFy84lJb4n+i6dFNin6DQWA80ymkIPknzhdqYTDVQkiSGr5STslwuu8XSHMC7Gcrh1VRM0zsjq20/aFFC53hq6aSK3no4f6V9Di7XEHQhfJXDldUYVj1FiFM3PNTzMka0n3jfb4i4+K+t4poa+hgrqV2aKZgc0+R2+PJNCYRjwOactN0xykO1TiNxsmhMdAApQu03BQmuRQ4FS22Kxni2EYfxBSimxBhbI0fRVDPfiPl1HkdFmeMYFiHD0wjrWCSBxtHUsHgf5eR8j81q9/Huu4hU4bFhj3YzJAyjkPdkT2IkP2QD7x8hqufq9Djyrc+H8nQ0utnie3tGHTVoi2sR5KNnxMnRpt5DdaFiPAeFYq9lVhM2IUED94X0zpR6tJIt6Eldwvs6wikrzJVTy4k9liIJ2hjWnq5oNz5A6eq5EPTMjZ1Z+o46KlwzwnXcTztq6h76fDg6xePemPMM8urthyuVtmGYZR4VRRUdFTsgiYNGtG3n5nzOqLR0zKeIANDSAAABYAdAOQTuIHMS5dnDp44I1Hv5ORlzyzPnoKLNaDzS2+IoDiSdNkWM2VlFVhDoFmXapihh4OxJjXWzRlg+O60epkyxmx5LFe1ipaOF5wTrJI2MfE3PyC04ocORVkl0jD6F4DrjcHYqcik00Vdi8Lg4bjbyUvBKHNBFx1HRWxIseyP01Qc+tySCNiuvcLX5puXK2iB2R5jmD2mwfrYcjzT2nrS1ocXEHYpmWGWItGp3b6poJCNioUFl6wriXEcIq2VOH10lNM3Z8T7X/DdbTwt25y2ZS8TU3fN29qgFnD+pux+C+ZoakgAEqRhq8vM35WWbNpMWZfUuS2GWUD7qwjHsJx6kFVhNdHVR88p1b6jcKRJNyAF8R4TxFXYXVMqsPrZaWdmodG4grbeEe21jwyj4nh12FXA3/U39R+C4Wf03Jj5hyjZDPGXD4NvaD01SXAkWQMNxPD8Wo21eHVkVVA4aPjdf8enxTo+S5bVdmiwTRqlFpPJKY0gpeU2SSBsAWXd0C9YBFIIQjoo0RFBdaCuNRgNE0gOAeFDe1H5ITkNCAkDquaImXS6GfeUCdimrpuvN9F4lSSFZ8r4FUioMtNURhoY1MMNipIePqds7wI3HQHa6e4lhk+A8VVVBZ3dSNzRO6+SpGNw4gKiOrbIWSsfdp5hbMmROKT5Ptunl7mFuEvuNh4/w6pdQtkw1hzFumVZVDR4jhzRUVkby8m+qvvD/ABdWV2GinqgO9jFiXDdHr5oMRp3d9G0OYCdAudqoQb3Y4nh9Z+n8uVuakMsNxI4hhwZMMptYNKjJMBq6mr7wSfR9AhYa6GnqnVE8zYqK9u8JsAuYxxrhdA/Jhczq542LQWsHxO/wWTTaXLPJ9EWzw2dQi3GT6BPpqijxAUjgSSLgrs+K4ZREtnq2ZxuxniPyVLxjibEcXqjPVTNjFsoZF4QB06lQUlSG3yalenj6NGUlKbr+DlyjFvgvNZxhA1jm0dNv9aQ/oFVsQ4ir6xhhdMRFe+VvhChJJnOPvX80Fzl18Wiw4+VHkXC6DPncfP1QXPvyskFySTdbkqCzj3crpGYXAJsvOCZVTyxocD7puk3QLkeOH2SHeibQ11IZ3Uxma2oB1jd4T890uJxOhN1yqp6WrYG1dPHMBsXDUehGoUXb6Gq8jokbFNZmjMQEy9lqKfSirnBg/wAKpHeN+DhqPmuiaqDrT0+W5tnY8Pb/AHHxCg5eGiVfAtzbeqSG2PVEI16lJ2SGOqaV0b2yN3YQ4fDVfWPDcrY6eOC/0FS3vofK4u5vzuPivk2n98DkV9PcISPrezrB6mN308UTcrvvMJb+inFWmJlukaQ61tQiAWbqEiKVlTTR1TNnDxA8vL4HROCLgaIoiCBIciXN9EmwumON45Q8OYU7EK4GQ+7FCz3pXdB0HU8kSkoK2NJydIYcYcaYPwRg7K7Ez31XPdtJRMdZ87huT9lg0u74C5Xzdj3F2McW1/tmMVPeuBtHE0WjhF/dY3YD5nmSoLjrE8ZxbjKqxXF6p1S6o1gdazWRj3Y2j6obtb481E0dXaUB3X9QuNmzSyPno7ukwxxq/JY6fE8UprCkxKrgFtop3tHvdAVM4dxBj9FisWKUmMVcdbHf6Qvz5xe2V4N8zfI/JQFOWvaHDnb809pyCWgc7fNyqs6sccJfcj6S4N7TcL4lfFhWJCOgxlwOSMH6OotuYyef3T8Lq/MDgbH8eq+TaHh6mx+shiqKyopI6WM1WemH0hcHANAP1fevfyW98FcWtqImYNi00hnYAyKomIzTW+1b635rTh1F/TM4ut0qxT+gvBalt0C464dY/A9V7zW6jmpjKvkyxO9Fgfa/WtENDQg+NzzK4eQFv1W6Yk4ZbeS+Z+0+q9o4qHiu1rS1voDb88y1pVj/AJKG7mU2PUpwx5Zq3fpfdAiFtUV3JNDH8UzZI738rHkkvNhdMQ4tJcNwNfNCdUVkzPA+OnYeY8bv0A+ae4jQ+dXRUrc872sbyJKCZI53mWFpyO11GyYx0VO2Xvnh00o+vKcx/DYJ4DYWQrfYceAwuAXAgganyRWS63BTaV5igaBvI7L8NyvNKEBKRVBsBe9lIw1JFiHKAbIQnMcxb8VMRd8E4pxXBaptThldLTSjmx1r+o2PxW1cMduMUrY6biajLXWH71TDT1cz+y+aI6g31T2KqIcDrcLJn0eLN9y5+SyGaUOj7qwnFsLxukFVhVfDVxEbxuuR6jcfFSJFhuvh/Dcer8MqGVNBVy00zDo+J5afktZ4e7dMWpmMgx2jjxCPQd9Ge7kt58j8lxc3pmSHMOUbI54y74PoNw80MtNlWuH+PeF+Iw1tFiccdQ7/APHnPdv9NdD8FahbZceUJRdSVGi/gCAUZo01XQ0XSrJJUFnLJJGqWkE6IYCCEHqikE7LwjuqxiAdEkjRG7srgAvqrEgswXje0oZKWhs0fuuPNZRjmK0dPXUzK9mVx1HQq5HiSvx/A2CqpmCVvNU/iCmjxWWnhqoGtdHoHBZ+Yx3XZ9Dj6xi0OPZfN9B2zmpk9qoHtbAxuZ5B2HmoQcWzUVZNVtcKmJgNoiLNd0uUz4qwk8Kinhp6p/d4hGXOYHaWBCrZl72ilZZurDyXofT9JDLD3Jrs836z+o8uRrHpnS8jyrxeereTJIdSXBjdGtJ6BMHzl+uvrfdNBJdrfTouOeQV3IQUVSR4qUnJ2wzpD1uhOeTzQ8+9iuFysoiKLl4kpIN17mpCPb6ry96rx0QMQU0q4+8icE8KG8XCiwGtI7NCwk62sfUJ0RomNM7LJLGfquv+KfjZRj0SYF7ddEI7W6pw5AcLoaBCeSSUUDRDdoVBkgkRsRqvpDslqva+AO4Juaaplj+Bs8f6ivm6I+ILduxGp/dcZoSdnRTgeoc0/wDxUocSRGXKNQpHey1joXfwZ9R0DuY+I/JSJPdnI7XofJM6unEsZbsdwRuD1S6KoNSzu5bNli9+/Lz9ChtRdMdblaHEkkdPCZ5j4RsBu49Aqdi0H7VndUVgDjbK1vJjegVinD6omQm0Y0Y3oP7qMmisCCFnnhll5fRbCUYGY4/wNR4tSS0zI8jy1z43NGrHDYj+3NYXW4dV4Rib6GuiySxOAPQi4sR5FfXlNT3qbluzHLOO0/hAYhhz8Uo4rVdK0u8I1e0alv6j/dYMunljVnQ0+dbqMgwya8QF72t+RPVS9AA6aMEW1b+RPVVfDpC2XLfSxN/8qtuHjLKDfYn5NWV9Hew/U0at2cYYyqqMXkcLiKOnjHoc7j/pH4KwYzhALiaZuVw1uFCdm1axlXjcLdC+GGUeeVzmn/UFoMVMXxOmk5rVp9L7mPecn1HNs1MosTwlxLJO1uEYw61Q3SKZ2mfyPmrk+7dCqMMNgqJTmZrfQjQhT1BXzNd+zq12Z4F4pT9cDr5ha4KeNqM+vk5UtsuYgMcqu4pZ5hq5rbNHU8vnZfMfHjrcZTU17+zxRRHzdlzH5uX0TizjVYlHStN2MOd/ryH6/gvmjiipFbxti9QDo6rkAPk05R+S6UlUUjIu2xnG2wXSlNGgSXaKIzgO+iAW5RpsjDYob9kwFROuLFLtZ46Juw2db5p0wZnDXRMQmp8VRE37DC74k/7LwuFyQ3qZT9mzfwH+68hAwgNiiNcEBKDrIAeNdbnujMkPVMWuRmkFOxUSUUx01T2ObX3rFQ7Hc7pwyS4tdOwJuOsew3BNxrfotQ4E7XMVwKVlFir34jhtvde76SL+lx3HkVjTZ3DS+nmj+0Zad2m5ACozYceWNTROE3F8H2zwtxrgfF0cgwyVzJ4hd8Eos8DqOoVkI1XxzwDxJNgfFmH17JCGNlDJR1Y42cD/AM5L7GBBAINwdQV5bV6dYJ0ujowluVniEO1yuueAkNdcrA2WULyroFl7SySTyBSAU7RqA5zgETla693d91O7A+UKXDZqOEyuuQdwmdVh8szWSZHWzbq7EtlovdFuirfFGNx4PhHhiu46A25q6ej2Q7Oc90nbdsyPtBxB0/FzqfMXNoomQC/W1z+ag6aU5ddj5JliVXJXY3XVkr85lmcSfku0zzoAvT6OKhjjFfBVM81xbmjO7CW/gu5ieaTMMlY/mHtDx+R/JJzLWRCZrFcvqkFy7fVMYW68NrlJDl2+qYCiVxcvde1umB4pDhoiab3SXBJgRz/BXNdsJAW/Eaj9U+BuLpnXtIhErd4yHj4JzG4ObpqCLhVrhjOuQyEUhIsmwE622QXg5ro/JCfqosZ6P3t1rnY1WCLiyopidKijeAPNrmu/QrIGGzvJaB2aVRp+P8Hds2SYwn0e0t/VRuuQPpl4u0WTKpgjLg8jxdeqfD3QmtQdFplFPsgm10Khs5hbyKBLTtvcotMl1HupoTI+KMGpIA2YVE8SVEeHcO4jiMsHtDKWnfK6L7YA28rqapx9O/8ApKzvtdx79mcKtwmJ1qjFHFrgNxCyxf8AicrfxVGoaWNtl+BOWRRR8/UdM2pp66oyGAxxvc3u3OAabbDyGm6BwzUOrWmOsqql8t7ktleD/wC3yun8V6fhyslyi8gy7a2v6A8/NQmFgUmPviv4HO8rC/rYc15w9dWxxNx7LoBScbNimxOcw1NNJTsjmBcHSXaWjNbT3TvzsFulRaOEMboAvmihqO6jhnhcxkzC17XNcwFrtCDpbmvoPD8VGN4LRYo2wNVEHvA2a/Zw/wD9Arr6CdrZ/Zx/VsLjJZV54HtMzxEpNbcuGU5HsN2uHIpxTi1rJrVuvKQurtUuGcPc10R+lK2WpkeXFodK9zudhcn5L5VjkNTUPmcbulcXn1Jv+q+l+Lar2LgnG6q9iyjkA9XDKPm5fM9K2zgByFlXk+6hx6JNu2iE/wB5HaLN1QngXSGCDtHW3AudQNCbJL/X/n/PJEDdc1yNLEg8kggA3AGqBAQ0h17W189v+eiewEBpc7YalNtC7dFlOWmLb6vIb/f5IARFdzc53eS4/FL+C4EpMDgXgV6y4kARpF7ojTYoDSUVJsYdrijMfa101BRA5R3BQ7Dr80Keoc6qhizOJJMhPpoEPvLJpSS+0YjNJbRtox+v5qLkSSLlhL3XDr2K+1+HcRjxDhnDKprw4yU0ZJ88ouvifDRZzW8l9D8EVWK4VwJh2MxZ6mjGdk0I1LQ15FwuD6m7pm3AuDZXDMvZbAHZMcJxihxWiZU0c7ZGPF7g7J+6y4n5NBwk2suF19NkCaqhgN5Hhg6lIir6OV9mTscfI3QA625rwcQd10PiAvcLwLHHRwUkhHypScSD2FntMT4i7k9tlP0GIYBWwRx1rWSh1mkGxvqpWpo8NqqcMmp2EDoFm/FGCRYTiFJXUMhbAZBmbfQLzPpP6rWtn7U40zTqfTZYFvTMLr2NpsRr44xZjayZjP6Q8gJFNMC6y9i88dRitVJF/DdK9zfO7if1TKN5a8FfVsTqKOFLklaveCUdSw/EXH5IRKVMS/D5MouWjOPUaoQeHNuNjqtTZAXe66ChZtSvA6pWAfMlhyb3uURpUkAYHqu3QwTdKUgFHQLhXuWq98UAAmZmjcCN03oHHuTGT4onZD+nyT51rFRw+gxIjlM35j/ZVy4djHxsknoleq4RdMQlBfzRyOaBJZRYwQOqsvDVWaLG8PrQbGCeOT8HAqs81JUTtQL+SglaaGfZryA45TcXNvRNJ9k2wGt/aPDeF1wN+/pY3n1ygH5gp1UjRaU7SZWJpRrqiVNshuh03VFqBeNC7GMqVuacgblpA/EL5n7TceGP8X108L81JS/ulOeRawm7tbe87MfwW88W40eHuDsUxKN2WoEJhgP/APY85W/hq7/KvlWctEYa1zdNNXNv+q5uvydY1/J1vT8V3kf8Ex3LX8Nd0BYHW+3M+ZH1eRBUJUU8kWIwTuzAkEAuJvcE9R+QU5hEzHURiJGaxsQRc+F3Qg80Sqoi6saWxOtmI0a4fWPQDr1/35Pg9K4bkmTNA+R0LfE8X6l/U+Xmth7NqsT4BVUbn3NLUZmi97NeL9BzaVjNDdkTLMcL2+o8cmdCtJ7NKkx4rW0xc76WmDwCXbtc3qPvFatHOsqKPUse/TSfxya7Ba/kFHVJ+lcn1I7Mxx8lHzn6U9br0kOzxEihdqtZ7L2fTQg2dV1EUPwBLz/oCwukGt1qPbRWWbgmGNOpMtS4fgwf/JZnSC2qzydyZYuh2bgFDcUYoD0hiTtokOKUSkHZSInmgFwSpzedjPsNzH1O3yC7E0lwCC13ePkl5Pdp6bD5IGgrSliyGEseSAOpOpSwCvWso2MSN0UagHqhEEIrPdVbZJIUuh1gkpJPmq2yVA6uoENPJIdmglcwdpbEzN7zvEfU6qOxOUvkhphu91yPIalTeFtzSagbKN+SVeC34ePdcd19d9nlAyPs0wyF7BaVr5CD95xK+PqR5jtcahfT3BnaLgNHwBhcWIVjIZ4Ie7cw7nKSAuJ6jJKKlLo14uiscSR4r2e8ZtxHC3u/ZVW+74b+EHmPJbTg9fDimGQVsJzMlYHBfPnH/aFBxKW0VBARAx+bvH7u9Ap3s34/hwymOGYo8shGrHnUDyXlMOswvK8aZd5Nvq6GCsp3QzRtc1wsQQsG4+4PxHhNz8cwKunZS3u+NshvH5jyWm1fadwnSxOe/E2OsL2aCSsR7Qu1ibiGnmwzDYRFRu8Jkf7zvhyXSyba5E6oPwx2j4vUYtTUWKYo80sjg3vNLj1K3GowzE/ZWVWE15EwF8r/ABMf5FfF0DqinnjMOaW591ouV9g9nPFFNifBdGauYMqoWd3K15s4EdQoYm23GQldGbyzMdmbAwyA7WKz7tRq5qHgprnjI6WdsTNddiT8gi4DX1lKXRYhVTwyA2DnC4Ko3aziFZLW0FBPVtnhDDOwNPU2ufwXl/QfRVh18eOO/wDRu1ep9zFbZlrnX1SQbG6U9qSAvsB54laV2Zgadv0TOG7A6F28ZLD8ESkcQbJM/gxB4tpI0P8AjsfyCsvgiKvrulAoJOqW03RYgzUQITCiBTQC82qXdBvqlBykAUc0r0skNN0q+ikBwhMK9hEYlbq6I5wpC6FIA4WsotWgORua9gc3VpFwUsjRM6F2Rr6d28TrD0OoT7cJLlDEEWFr39E3kanJ6IEgSYhuPeTylJzi3Ipkd06pjZ9trqKGfTnZZW+2cAU0bjd1JPJAfIGzx/qKuNT7qyjsXrrxYthxdyjqGjzBLHfm1atUnwhW4+qIvsFTFOZh9Hc7JtTmzrJ1U6QkqXkDEO2jFMkOF4O14GYvqpGlwFwPA3cH76xSVzi3R5+DnfoFofajVvquOa5rXOy0rI6cWzjUNDnbae88rPXMe4HQ3A6P815/Uz3ZZM9Rpce3DFf2GpZMotnbbK7QvBv4T1CmS6N8oAY13j5CM/X9VDQF7BbvCBY/WeOTuoUtE8OlBLmu8fORv2x1asjOrifA9pWAQsIiB8I1EX3W9Cr7wFK6PiyFpBAkhlj2ePqk/W/pVAiaHRNLWA+HcMY76o6EK5cFkwcXYaCzKHSuZ7jm7tkHUhW4HWWL/I9THdp5r8P/AIb1Qj93e7yUXO76f4qUo9KJ3ooeQF1VbqbL1se2fPZGD9qtZ7V2gvgDrtpKaKG3QkZz/qVZpm2Aul8RVwxTjTF64HM2WrkLT90HKPkAlQt8Kyd8lwskDRAfz0v8Ud502Tdx1TQAl4LyUBdSInpH93SyOHvEZW+p0SGABoA2CTUgmaKEH3RnP5D9UtAxSI0H4JARBsosAgbokEI8Y1IuhvFioWSSBapbN7Lmh5JTRqoNk0dcLFBe4DdOX6DzUXiFQIKaSQ7NaSqmyaI2BxqMWnqD7sf0bfzKtmFt2zc1WMJhLYGB/vO8TvU6lWujAYWt6BJ8KgXLsnYhbYp5NVd3hcJcdWSOZ+Nj/dMqWQE2BCVijf8ApVQb6sLZB+Nj+a4/qeD39PKBdF8jmKoZ3Zlc8aJtJjkkYJjda2xWudmfZ7w9jOAtrMWkE0sjQ7IXaNBWbdo3DVDw9xXJQ4bJnpy3MG3vl8l4vH6WoPc2Wu6sq0/ElTch/iHUJp+1o5jY7lBmpiRbKm4gyyNcG6hdVxaVdlaaLDg2MOwrF4Ksxd81p1YeYV94gdxDVOp8VoMMq6WlqWhl49M3S4CyttVnqGANsWreqDiviOr4Mo54cMikipsuZ5+sB5KeLG5QaL1XQ2rMOxSk7qWtEcglGXIG7L594qlDuKK+JkhkjhkMTSTfY6j8br6MxPimFrKnEa50TI6WkfUsYT75A8IHqbBfLk73vkdJIc0jyXOPUnU/Na/0/gaUss+zVr5Y4YY4sfTdjd+6GdEsnVcK9YcENTus5KrjbuJujiw/Ef3CAxxBTiqHeYfJbdozj1Gqmug8gM10RhTUPuLg7o0LrlJAPWapaFEUaysREQSuhJIXL2TAO3YJY9UFpRWlSQC0lwXeS9a4KYEbJeDEWP8AqyjIfXcKSBuNEzrojJTuLfebqD5jZFpZhNTskH1hf0KguHQwxQXjdHOyG4aJsQydo4osLhmBQ3jUrsZs5Vrhgar2S13s3HVLAXWbWRyQfEtzD5tC36oHhXytwviBw3iDDq8G3s1RHIT5BwJ+V19WVoDXEN1bfT05K2HbQn4GtPbMn1W29NbromFP79k8xSQQYTJMToxuY/AXUm6YdnyZxLN7fj+LVYAd31ZM4ENvpncBs7o0bqvNiIJHd3Ou0Z8/NSLy2ajEpLXF4zm/du3zE72PNNO5BB8AO/8AhtP2uhXmJO3Z7WMNqS/B5rHNJsHNGv1ZG/aUlBKQ8XkGruch+0OoTIQuFzkI1P8AhuH2uhT2CQsc27y0X+09v1m9QVBmiHA4YQ+FosHHL0jd9X4K1cK/RcU4U4RgAVcYJERG73Dkbc1VGuD4x4w4ZPtRu+p52KsWBDu8eoZWx2yVcZBEQ0+lPNpTg6kmXzV45L8M+j6fw0Tr9FWcUrG0NBXV7jZtNBJLf+lpI+dlZwctI/y0WZ9pNd7HwJiQabOqiymH+Z1z8mlevuotnziraMCpmkuDnG7jv6qajbZvlZRlK3xjy1Uq0ZRbkBus3RaIfsU2cUaU8kAqSEcuiQtzPFyhbnReneYqJ5GjpLMb8d/ldAIAx/ezSz8nu8PoNvkjjZCY3K0NGwRQLndIYto80VoNrobRpuigW0JUWwSCRk5vkuyN6rjBZwS3jQ3Nj6KtsmkNwixgEoVtUeMeEKDJJCJhYGxsq1jMhkfDSB2srxceQ1KsdQ4Aa7qqOPtGOSybthaGD1Op/RV9uizpWTmGx53W0urDE0h+uhsoPD2ltnAqwMe3TT49EpPkIrgdUr3NAubEOUxMxktM/OM0b4nX+Gv6KJjAzEed1MxeKhbr7pc0+haVnzq4MkhrLPxXg1NTV1JFXUlG8WY9oIa4JvWUWPT0pxetgnkY/UyvBJWj1Pa5htZw7QYJVYWGmMsZI4EZbCwuFf8AiziHhs8Bsp6FkUr5ow1jW26bry9qm7NSSaPmKoeaaO7xdxUayOWWQvvoeSnKqmdUVxBb4G7BDhgjjqiHDQJY+VyUydcIj4oSJSSF9F9knEuBVvDMmA4g1jJIfCQ/ZwPNYJUT08Bc/LZTfBlDPLWPxAlzGO0AvbRWb1jRKHyA7QmPg4cwR8jsss7TG9nMZQCfmsunNn2Wh9p9bFU8T0dHHp7JTZpB0e43/ID8Vm87vpSu76VFx00W/PJic3JWxBK6Chl1yug3XVIhAQE5aWlhaTod02aAUVosNymmIionZWGMnVhyn4FPKZ2qYT+CumaPrEO/H/snFM/xbqKY2S0SPoeaaQuTkHRXJkRL/JIuluQzshgLa7VGB0TZpRWnkU0wDj1Sr6IYK7dTEcfq0hMaL6Kompidjnb6H/dPyo+q+hqYankDld6FRfyNEn+SQ9KabrzhopCGkgQhujvG6DaxVbGStE67g089F9V4HX/tTg/CcQJu6WlZn/qaMrvm0r5NpHahfRPZbiArOAnUpdd9DUuZb7rwHD55lKP3IT6LvTAukCbccVHsfA2JzZrZaaQ/+wp5Sj6QBV7tam7js9r2jd8Jbp5kD9UZXSZPErmkfNu2GxNLyC1jRZz/ALv3m+aYuDXAkZTof/TPJymQ1zaRrTnYABzkaNm+oUXJbU94NjvI08j1avNHuZR6ECI62jvqdREPvdHJ3CQ14PiZr1kb9ZvqgBjXBwDA7U/UYebuhR4QWvBLSz4Pbzb0ukyURwHjIPpbjJt3jT9Q/aCmMNGWvgk7sHJO11xE07PPNpUKJfB/F0y7Gb7p+0FJQeE94GZ7OvcMY76x5tIKS7L+0z6dkd+5ynzP5rEO1+ty0uEYY12ssslQ8eTQGj5uctnMgdhhfyOq+c+0ytNZx6+nDrsooI4fRxGd3+oL10n9B83XZWqVoLhf8VInofxTSmZYXvqnBd1VBYBktdBIuborzcoevJSQjgbdwAKHVESVUUP1Ym5j6n/b805jDblzzZrRcnoEzgJkLpne9IS4pMYQBLtrzXrLqVgKF72F04YL+qCwAmydMFmgqEmTihA3XXG4XXCyHmJbYqBIQb3TqIHKDbZNra3T2OwiJvoFCT4JIhcXqRAx73GwY0kqBwiMmEPk9+Ql7vU6onEU/eyspGamZ9j/AEjUpzRMALdOarh5kSl8E1SssBbRSsTjp6phAAA3VPWeSTYyWhyl9ywPvrbZSURtRVDRYljM4+Fx+qiIH2cLKcw+jlrKuKjiYXyVV4WtHMuGg/FU5vsZJFRoaF1RiEcb9cxWiyU7aWhZC3SwUfUcP1vDlbnxOjfC5gvqNPxT1tfDVYW+uf4Wja68Tkm26Lop0RQphmc61yUqj4aqMZxSCjpHBs0rg0EpArTLRvngiJA2Kkuz2trKjtCwkG7R32oHRX45W0hKDbtmkUP/AIb4Z3xzYrjUsjSBeONgbr6p7jvZbHwrhRqsPrC6GLdjxr+K3lsjY6cOcbWCyLjavxri/GG8PcOwufSxO/eKk6MB+zfmtc4RkqZZzXB8dcU4zFjfGOPYxDCYIJ6giKJxuWMHhaL+jVWHHMSUSSZxow82DpnukNvMoUeoXq8UFCCgvBzWcIXRe6Jl0JSLBXCCNNkQOBQAlAoAjMQs2rY8C2a7V2mf9IuYqP3fvObSCEClfdwPVQb5JVwT8J0ToFMYDoE8CuiViihnZL3SHbKTATc3SgUjZeB1SAdNN0tAY66MCpoQvkm9TEJYXMI3CNdJJ0TADQzukp25/fZ4HeoTsqMYe4xItJsyYaf1BSN7tSi+BsG/ZAI1Thw01QHDVJiDQOs8LYOyHExFjNfhbneGrp+8YPvxm/8Apc78FjcZs4K5cG4oMJ4qwyvcbMjnaJD9x3hd8iUXxYz6eoheVtxzVL7a5AOD54uRawcucjQrxRMLZcpNy11lnXblJl4ecw6ZpIGakc5L89PqqGd/Sy7TK8sf5MYZE4UrSIyAA3UMcOTebSo6V1mEGU7bGUjkftBSMLCaZtotNNRFf7HNhTKQkNt3haMvOR7fq/eC86e7a4G2hzaB5ueTHc3eiLE3K8Huy30jcBu3oUNxBc65DvER7zHc3dbJcbBdv0JGv/pnqzm0oK0OBKWs/iEWb/6zh9V32gnROeF9wH77iN/1vgeaaseWggy5bN271zfqu6gok0gMbxmD9SNXRv8ArDrYpeS7wfTFPM1/DtPI42a6JjifLKCvlqurDiuOV2Ju3qp3yj0J0+VlueNYw6g7FPbWOtLLh8MMZ+9IxrB8iT8FgtOxos1o0GgXq5vhHzuqbJCEABKcuN0C492tlWMERquD0XSSvNFz6JiEVZyUgjHvTHL/AJRqf0HxSWAABDmd3lc5v1Yhl+O5/t8EvvYmjV7R8VEYRdG6CJ2E+AOd/S0ldMknKE/5iAhjQ6YNU5bbLvso9rpzsYmepLkXLM5ozVTh5MaAq2TQ4ke1oOZwATP2um73uxOzMeV0QUVM83lY+U3+vISPwFk7iiigaBBBHF5saAVC0T5AxWkjD2g5TzIIui1EgionX3KXnc6XI4klo5nqf+yieI6xlHQveTqGXA8zsqZy4JxRU8/tmOSS7ti8A9dyrJSMF2qt4NCQzM7Vx1PqVaYGgWTXEaF27JKPQA9E6jdcpnHYhOoQASokiQhOgJJV04bqG0uLYRWOJAgrInEjoHAqkwe5bysrBSTFuHOeD4o3tdf8VTm+1k49n1dxtwfBj2FSxRNaJTq11l84cXcG4lgUEFLIS2N77aCwK+vMOlFXg9FUnXvoI3/i0FZ52rYfDU4XRtazNMagZABqV5XUYri2a4vwYA6iZR4THCGauHJaV2V8A1MOJx8RVlOY2NH0LXixPmrpwh2dU0fdYljEQlmAuyJwuGf7rTGwRxxhjGhoGwCr0+BxW6RKUkuEMZac1MPdvJDedl6joKaijEdPC2No5NFk/azVKyhbqK7Pyun8DmQ8o2hvxtr80ZjcrAmpcZJrnclPnjK8t6L1kTlMTsFy1107r3NWCsQR5IZdZH5IEjSVFoYxrHB8D28rKOoZLtaOY0T6cHIdFE0bi2rezzuqm+Sa5TLRA7ZPmuuoqndspCM6LREqYe6S4r19FwqdCEErwK67ZD2KjQw7Drujgpq02RWkqSEGvqujZIuu8lIBrWsJj7xnvxnOPgnUMrZY2vbs8XC4RcbXTOjf3UktMf8ADOZvoUumMkXbbIDhqik3CE5NoRxnUqVonZtDzCiQdQn9G+0gUaGj6+4bqDWYLhlY43dPSxSE+ZYL/NZp28T5aCmhvbPVRcwNmyHmrr2aVPtnAWCyXuYonQO9WPcPyss57eagtrcOiDrXnze9baJ391nzv9ts2aRfvxX5M1hjBjYTEHajaNrubPskFN3+CK/ueH7UjPqj1Ro2l4aTDnGa38NjvrN5ggoLiWx39wZL7SMt4B6rhntgEjy5xvJm1O8jXc3dQvMYA5pMemmoi/o5tKNISXH6TMM2n0rT9Z32ggiEkg90dNf4bTb3PslIhQ5a4taQXZbD7cjeTuoQqycd04GQPu6wHeMd9ZvJwSg5zWkEuYQLf4jeT/VM8Rnc5paZM/i271rvrN5OCF2E3US/cYYkD2OcFUANnVbY5XDT3Yo/LzcFRqZgIF07xvERWYLwfQtOlDgzCRYCzpJHHlps1qDTCzR1Xpou4p/hHgpKpP8Alh3ajXVBO+qI463QndUyIgnVKEncsdKdmC9uvQfikAFxA3Sas+GOAfWOd3oNvn+STYIZxU4tmcM7ibkuN7lOGNDRo0D0C6BolD0UKJBAfNdyt0sFwWRW2JGt1BkjjW67I4Gg0Qnac7LvfRN0MjQel9VFk0GsMwAHNHi961k1zlxGSKR3nlsPnZOIxPnaSWRgam/iPyUaJWJGtS8jrZUrjCpMuLx4e03sWvf5ADT5q7tZlmcPvG34rN8Qcaji/EpnahsxYD5N0H5KqS6JIlaCMMiAspeJ3i0UXSm7QApGAWN1IiScR0CfQgk+qj4na2UlBrZNoY7iG2uimcPb3lPVRX1Meb4g3UXGPJS2EWFWAbAG7T8RZZ8v2snHs+0uF3l/BeCPJuTQw/6AnM+HwVdTHLPGHmM3bcbFB4bgdBwjg8DhZ0dHC0+uQKWAAXAatmmzrWhjQAFwrt0nmhsR1eXhddNkID//2Q==" alt="Anay Patel" id="portraitImg">
      </div>
    </div>
  </div>
</header>

<main>

  <section id="work">
    <div class="wrap">
      <div class="section-head reveal">
        <h2>Work experience</h2>
        <span class="section-index mono">3 roles · 2025–2026</span>
      </div>
      <div class="timeline reveal" id="jobList">

        <article class="job">
          <div class="job-head">
            <div><span class="job-title">Software Engineer Intern</span> · <span class="job-org">BDO USA</span></div>
            <div class="job-meta">Jun – Aug 2026</div>
          </div>
          <div class="job-place">New York, NY</div>
          <ul>
            <li>Built an enterprise generative-AI assistant with a persona-driven RAG architecture on .NET 8 and Angular, projected to cut workflow research time by 40%, using Microsoft Entra ID for service-to-service auth.</li>
            <li>Cut time-to-first-token by 22% by designing an asynchronous streaming pipeline with incremental token delivery, keepalive processing, and cancellation propagation.</li>
            <li>Strengthened API resilience and projected a 30% drop in incident triage time by instrumenting end-to-end latency telemetry in Azure Application Insights alongside rate limiting and SSRF protections.</li>
          </ul>
          <div class="job-tags"><span class="tag">RAG</span><span class="tag">.NET 8</span><span class="tag">Angular</span><span class="tag">Azure</span></div>
        </article>

        <article class="job">
          <div class="job-head">
            <div><span class="job-title">Software Engineer &amp; Quantitative Developer</span> · <span class="job-org">AlgoGators Investment Fund</span></div>
            <div class="job-meta">Aug 2025 – Jan 2026</div>
          </div>
          <div class="job-place">$500,000 live portfolio · Gainesville, FL</div>
          <ul>
            <li>Automated portfolio metrics reporting with a background task pipeline in Python and Celery on a Redis message broker, dynamically rendering backtesting data into custom HTML emails for stakeholders.</li>
            <li>Built a custom rate-limiting and circuit-breaker wrapper for external financial APIs, preventing HTTP timeout errors and managing automated retry-backoffs during high-frequency data ingestion.</li>
            <li>Devised the Market Condition Sensitive Strategy (MCSS), a predictive trading strategy using scikit-learn Random Forest classifiers on macroeconomic indicators to dynamically toggle capital allocation between momentum and mean-reversion models based on real-time volatility.</li>
          </ul>
          <div class="job-tags"><span class="tag">Python</span><span class="tag">Celery</span><span class="tag">Redis</span><span class="tag">scikit-learn</span></div>
        </article>

        <article class="job">
          <div class="job-head">
            <div><span class="job-title">Machine Learning Researcher</span> · <span class="job-org">Digital Worlds Institute, UF</span></div>
            <div class="job-meta">Aug 2025 – Jan 2026</div>
          </div>
          <div class="job-place">Gainesville, FL</div>
          <ul>
            <li>Built Python pipelines with ANTsPy and NumPy to preprocess and spatially map 249 3D MRI scans to the MNI152 template.</li>
            <li>Generated 150+ synthetic brain scans with PyTorch and 3D-StyleGANs to address data scarcity in neurodegenerative research.</li>
            <li>Validated structural reliability of generated scans across 130+ volumetric regions with scikit-learn and XGBoost, reaching AUROC scores above 0.94.</li>
          </ul>
          <div class="job-tags"><span class="tag">PyTorch</span><span class="tag">StyleGAN</span><span class="tag">scikit-learn</span></div>
        </article>

      </div>
    </div>
  </section>

  <section id="projects">
    <div class="wrap">
      <div class="section-head reveal">
        <h2>Projects</h2>
        <span class="section-index mono">3 shown</span>
      </div>
      <div class="project-grid" id="projectList">

        <div class="project-card reveal">
          <div class="card-glare"></div>
          <span class="project-badge">Aug 2026 – present</span>
          <h3><a href="https://www.apple.com/app-store/" target="_blank" rel="noopener" class="project-link">Visionary ↗</a></h3>
          <p>A real-time computer vision system for movement tracking and dietary logging.</p>
          <ul>
            <li>Built a real-time biomechanical kinematics engine processing 33-point spatial coordinate maps at 30 FPS with under 30ms latency, using OpenCV, MediaPipe Pose, and NumPy vector trigonometry over a WebSocket streaming pipeline.</li>
            <li>Built a multimodal dietary-logging pipeline combining OpenAI Whisper transcription and Gemini with strict Pydantic validation against the USDA FoodData Central API, reaching 98% schema parsing accuracy under 1.5s.</li>
            <li>Deployed a high-concurrency FastAPI backend handling 100 concurrent WebSocket streams, cutting query latency 40% with Docker and Redis caching.</li>
          </ul>
          <div class="job-tags"><span class="tag">FastAPI</span><span class="tag">OpenCV</span><span class="tag">LangChain</span><span class="tag">Docker</span><span class="tag">Redis</span></div>
        </div>

        <div class="project-card reveal">
          <div class="card-glare"></div>
          <span class="project-badge">1st place — Internet Programming Hackathon</span>
          <h3><a href="https://sobaskee.github.io/AGame-ServeUP/" target="_blank" rel="noopener" class="project-link">ServeUp! ↗</a></h3>
          <p>A full-stack recipe platform with generative AI at its core.</p>
          <ul>
            <li>Built a full-stack app with an Express/TypeScript REST API backed by MongoDB and a React frontend, integrating autonomous LangGraph multi-agent sub-agents to audit OCR scans and process Spoonacular API recipes.</li>
            <li>Developed a live Generative AI Recipe Canvas using Gemini 2.5 Flash, Server-Sent Events streaming, and Zod schema validation for zero-shot culinary style transfer with real-time macro calculations.</li>
            <li>Engineered a decentralized peer-to-peer sync pipeline using WebRTC DataChannels, Yjs CRDTs, and the WebCrypto API for real-time, serverless multi-user state agreement.</li>
          </ul>
          <div class="job-tags"><span class="tag">React</span><span class="tag">TypeScript</span><span class="tag">Node.js</span><span class="tag">Express</span></div>
        </div>

        <div class="project-card reveal">
          <div class="card-glare"></div>
          <span class="project-badge">Aug – Dec 2025</span>
          <h3><a href="https://drive.google.com/file/d/1EG3m2M_9PsSluh_FTnCtabf6jEKvDrTS/view?usp=sharing" target="_blank" rel="noopener" class="project-link">Market Mood Mapper ↗</a></h3>
          <p>A pipeline linking earnings-call sentiment to short-term stock price behavior.</p>
          <ul>
            <li>Built an automated ETL pipeline ingesting 100k+ minute-level stock price records to compute cumulative abnormal returns across earnings windows.</li>
            <li>Applied a FinBERT and PySentiment NLP extraction engine to unstructured earnings call transcripts, gathering 36 semantic features with full data coverage.</li>
            <li>Modeled transcript sentiment across 5-, 30-, and 60-minute post-event windows using cross-sectional OLS regressions with HC3 robust standard errors.</li>
          </ul>
          <div class="job-tags"><span class="tag">Python</span><span class="tag">SQL</span><span class="tag">FinBERT</span><span class="tag">pandas</span></div>
        </div>

      </div>
    </div>
  </section>

  <section id="skills">
    <div class="wrap">
      <div class="section-head reveal">
        <h2>Skills</h2>
        <span class="section-index mono">by category</span>
      </div>
      <div class="skill-modules">
        <div class="skill-module reveal">
          <h3>Languages</h3>
          <div class="skill-chips">
            <span class="skill-chip">Python</span><span class="skill-chip">C++</span><span class="skill-chip">C#</span>
            <span class="skill-chip">JavaScript</span><span class="skill-chip">TypeScript</span><span class="skill-chip">Java</span>
            <span class="skill-chip">SQL</span><span class="skill-chip">HTML/CSS</span><span class="skill-chip">MATLAB</span><span class="skill-chip">RISC-V ASM</span>
          </div>
        </div>
        <div class="skill-module reveal">
          <h3>Frameworks &amp; libraries</h3>
          <div class="skill-chips">
            <span class="skill-chip">React</span><span class="skill-chip">Next.js</span><span class="skill-chip">Flask</span>
            <span class="skill-chip">PyTorch</span><span class="skill-chip">TensorFlow</span><span class="skill-chip">Keras</span>
            <span class="skill-chip">scikit-learn</span><span class="skill-chip">LangChain</span><span class="skill-chip">SQLAlchemy</span>
            <span class="skill-chip">MongoDB</span><span class="skill-chip">PostgreSQL</span>
          </div>
        </div>
        <div class="skill-module reveal">
          <h3>Practices &amp; tools</h3>
          <div class="skill-chips">
            <span class="skill-chip">RAG</span><span class="skill-chip">MCP</span><span class="skill-chip">Agentic AI</span>
            <span class="skill-chip">Data Pipelines</span><span class="skill-chip">Git/GitHub</span><span class="skill-chip">Agile/Scrum</span>
            <span class="skill-chip">Google OAuth</span><span class="skill-chip">Jupyter</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="education">
    <div class="wrap">
      <div class="section-head reveal">
        <h2>Education</h2>
      </div>
      <div class="edu-row reveal">
        <div>
          <div class="edu-name">University of Florida</div>
          <div class="edu-detail">Bachelor of Science in Computer Science · GPA 3.8</div>
        </div>
        <div class="edu-meta">Gainesville, FL</div>
      </div>
      <div class="course-chips reveal">
        <span class="skill-chip">Software Engineering Fundamentals</span>
        <span class="skill-chip">Data Structures &amp; Algorithms</span>
        <span class="skill-chip">Frontiers of AI</span>
        <span class="skill-chip">Operating Systems</span>
        <span class="skill-chip">Internet Programming</span>
        <span class="skill-chip">Information and Databases</span>
        <span class="skill-chip">AI Fundamentals</span>
      </div>
      <div class="edu-year reveal">Class of 2028</div>
    </div>
  </section>

  <section id="connect">
    <div class="wrap">
      <div class="section-head reveal">
        <h2>Connect with me</h2>
      </div>
      <div class="connect-panel reveal">
        <div>
          <div class="status-line">Always up for talking through a hard problem — reach out below.</div>
          <div class="connect-links">
            <div class="connect-link" data-magnetic>
              <span><span class="label">Email</span><br>anay06p@gmail.com</span>
              <span class="email-actions">
                <button class="copy-btn" id="copyEmailBtn" type="button">Copy</button>
                <a class="draft-link" href="mailto:anay06p@gmail.com">Draft email ↗</a>
              </span>
            </div>
            <a class="connect-link" href="https://linkedin.com/in/anaypatel-" target="_blank" rel="noopener" data-magnetic>
              <span><span class="label">LinkedIn</span><br>linkedin.com/in/anaypatel-</span>
              <span class="arrow" aria-hidden="true">↗</span>
            </a>
            <a class="connect-link" href="https://github.com/patelanay" target="_blank" rel="noopener" data-magnetic>
              <span><span class="label">GitHub</span><br>github.com/patelanay</span>
              <span class="arrow" aria-hidden="true">↗</span>
            </a>
          </div>
        </div>
        <div class="local-card">
          <div class="local-label">Local time — Gainesville, FL</div>
          <div class="local-time" id="localTime">--:--:--</div>
          <div class="local-label" id="localDate">—</div>
        </div>
      </div>
    </div>
  </section>

</main>

<footer>
  <div class="wrap" style="display:flex; justify-content:space-between; width:100%; flex-wrap:wrap; gap:10px;">
    <span>Anay Patel · US Citizen</span>
    <span id="footerYear"></span>
  </div>
</footer>

<div class="cmdk-overlay" id="cmdkOverlay">
  <div class="cmdk-panel">
    <input class="cmdk-input" id="cmdkInput" type="text" placeholder="Jump to a section or project…" autocomplete="off">
    <div class="cmdk-results" id="cmdkResults"></div>
  </div>
</div>

<script>
(function(){
  const reduced = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  const fine = window.matchMedia('(pointer: fine)').matches;
  const cbMode = !reduced && window.innerWidth >= 700;   // cursors build the page (otherwise normal scroll reveals)
  const units = [];

  /* ================= persistent animated background ================= */
  (function initParticles(){
    const canvas = document.getElementById('bgCanvas');
    const ctx = canvas.getContext('2d');
    let w, h, particles = [];

    function resize(){
      w = canvas.width = window.innerWidth;
      h = canvas.height = window.innerHeight;
    }
    resize();
    window.addEventListener('resize', resize);

    const count = Math.max(24, Math.min(70, Math.floor((window.innerWidth * window.innerHeight) / 26000)));
    for(let i=0; i<count; i++){
      particles.push({
        x: Math.random()*w,
        y: Math.random()*h,
        vx: (Math.random()-0.5) * 0.18,
        vy: (Math.random()-0.5) * 0.18,
        r: Math.random()*1.3 + 0.6
      });
    }

    function drawFrame(){
      ctx.clearRect(0, 0, w, h);
      for(const p of particles){
        p.x += p.vx; p.y += p.vy;
        if(p.x < 0) p.x = w; if(p.x > w) p.x = 0;
        if(p.y < 0) p.y = h; if(p.y > h) p.y = 0;
      }
      for(let i=0; i<particles.length; i++){
        const a = particles[i];
        ctx.beginPath();
        ctx.arc(a.x, a.y, a.r, 0, Math.PI*2);
        ctx.fillStyle = 'rgba(107,182,224,0.4)';
        ctx.fill();
        for(let j=i+1; j<particles.length; j++){
          const b = particles[j];
          const dx = a.x-b.x, dy = a.y-b.y;
          const dist = Math.sqrt(dx*dx + dy*dy);
          if(dist < 130){
            ctx.beginPath();
            ctx.moveTo(a.x, a.y);
            ctx.lineTo(b.x, b.y);
            ctx.strokeStyle = 'rgba(107,182,224,' + (0.14 * (1 - dist/130)) + ')';
            ctx.lineWidth = 1;
            ctx.stroke();
          }
        }
      }
    }

    if(reduced){
      drawFrame(); // one static frame, no motion
    } else {
      (function loop(){ drawFrame(); requestAnimationFrame(loop); })();
    }
  })();

  /* ================= scramble-text reveal ================= */
  const SCRAMBLE_CHARS = '!<>-_\\/[]{}—=+*^?#$%01';
  function scrambleText(el, finalText, tickMs){
    tickMs = tickMs || 35;
    clearInterval(el._scrambleTimer);
    if(reduced){ el.textContent = finalText; return; }
    let iteration = 0;
    el._scrambleTimer = setInterval(()=>{
      el.textContent = finalText.split('').map((ch, i)=>{
        if(ch === ' ') return ' ';
        if(i < iteration) return finalText[i];
        return SCRAMBLE_CHARS[Math.floor(Math.random()*SCRAMBLE_CHARS.length)];
      }).join('');
      if(iteration >= finalText.length){
        clearInterval(el._scrambleTimer);
        el.textContent = finalText;
      }
      iteration += 0.6;
    }, tickMs);
  }

  /* pre-scramble the hero name immediately so nothing correct is visible before the preloader lifts */
  const heroNameEl = document.getElementById('heroName');
  const heroNameFinal = heroNameEl.textContent;
  if(!reduced){
    heroNameEl.textContent = heroNameFinal.split('').map(ch => ch === ' ' ? ' ' : SCRAMBLE_CHARS[Math.floor(Math.random()*SCRAMBLE_CHARS.length)]).join('');
  }

  /* wrap the role-line into words so it can cascade in one word at a time */
  const roleLineEl = document.getElementById('roleLine');
  roleLineEl.innerHTML = roleLineEl.textContent.split(' ').map(w => '<span class="word">'+w+'</span>').join(' ');

  /* ================= preloader boot sequence ================= */
  const bootLines = [
    'anay@portfolio ~ % initializing session',
    'loading experience.json ... <span class="ok">ok</span>',
    'connecting pipelines ... <span class="ok">ok</span>',
    'rendering interface <span class="boot-cursor"></span>'
  ];
  const bootEl = document.getElementById('bootLines');
  const preloader = document.getElementById('preloader');
  const heroEl = document.getElementById('hero');
  const wipeEl = document.getElementById('wipe');

  function finishBoot(){
    wipeEl.classList.add('run');
    preloader.classList.add('hide');
    document.body.classList.remove('locked');
    heroEl.classList.add('ready');
    if(cbMode){
      // cursors will drag every hero element into place, so skip the timed intro
      roleLineEl.querySelectorAll('.word').forEach(w => w.classList.add('show'));
      setTimeout(startSwarm, 300);
      return;
    }
    scrambleText(heroNameEl, heroNameFinal, 32);
    const scrambleDuration = Math.ceil(heroNameFinal.length/0.6) * 32 + 80;
    setTimeout(()=>{
      heroEl.classList.add('name-drawn');
      roleLineEl.querySelectorAll('.word').forEach((w,i)=>{
        setTimeout(()=> w.classList.add('show'), i*45);
      });
    }, reduced ? 0 : scrambleDuration);
  }


  if(reduced){
    finishBoot();
  } else {
    bootLines.forEach((line, i)=>{
      const div = document.createElement('div');
      div.className = 'boot-line';
      div.innerHTML = line;
      bootEl.appendChild(div);
      setTimeout(()=> div.classList.add('show'), 120 + i*220);
    });
    setTimeout(finishBoot, 120 + bootLines.length*220 + 380);
  }

  /* ================= custom cursor ================= */
  if(fine && !reduced){
    const ring = document.getElementById('cursor-ring');
    const dot = document.getElementById('cursor-dot');
    let rx=0, ry=0, dotx=0, doty=0, dx=0, dy=0, primed=false;

    window.addEventListener('mousemove', (e)=>{
      dx = e.clientX; dy = e.clientY;
      if(!primed){
        // snap to first position instantly so the cursor doesn't swoop in from the corner
        rx = dotx = dx; ry = doty = dy;
        ring.style.transform = 'translate('+rx+'px,'+ry+'px) translate(-50%,-50%)';
        dot.style.transform = 'translate('+dotx+'px,'+doty+'px) translate(-50%,-50%)';
        requestAnimationFrame(()=>{ ring.classList.add('visible'); dot.classList.add('visible'); });
        primed = true;
      }
    });
    (function loop(){
      // dot trails tightly, ring trails a touch looser for a soft, connected feel
      dotx += (dx-dotx)*0.35; doty += (dy-doty)*0.35;
      rx += (dx-rx)*0.14; ry += (dy-ry)*0.14;
      dot.style.transform = 'translate('+dotx+'px,'+doty+'px) translate(-50%,-50%)';
      ring.style.transform = 'translate('+rx+'px,'+ry+'px) translate(-50%,-50%)';
      requestAnimationFrame(loop);
    })();
    document.addEventListener('mouseover', (e)=>{
      if(e.target.closest('a, button, .skill-chip')) ring.classList.add('hovering');
    });
    document.addEventListener('mouseout', (e)=>{
      if(e.target.closest('a, button, .skill-chip')) ring.classList.remove('hovering');
    });
    document.addEventListener('mousedown', ()=> ring.classList.add('pressing'));
    document.addEventListener('mouseup', ()=> ring.classList.remove('pressing'));
    document.addEventListener('mouseleave', ()=>{ ring.classList.remove('visible'); dot.classList.remove('visible'); primed=false; });
  } else {
    document.getElementById('cursor-ring').style.display='none';
    document.getElementById('cursor-dot').style.display='none';
  }

  /* ================= continuously flipping tile field ================= */
  (function initTileField(){
    const field = document.getElementById('tileField');
    if(!field) return;
    const cols = 8, rows = 6;
    for(let i=0; i<cols*rows; i++){
      const tile = document.createElement('div');
      tile.className = 'tile';
      const dur = (4 + Math.random()*3.5).toFixed(2);
      const delay = (-(Math.random()*dur)).toFixed(2); // negative delay = starts mid-flip, so tiles are already out of sync on load
      tile.style.setProperty('--dur', dur + 's');
      tile.style.setProperty('--d', delay + 's');
      tile.innerHTML = '<div class="face front"></div><div class="face back"></div>';
      field.appendChild(tile);
    }
  })();

  /* ================= scroll progress ================= */
  const progress = document.getElementById('scrollProgress');
  function updateProgress(){
    const h = document.documentElement;
    const top = Math.max(h.scrollTop, document.body.scrollTop);
    const max = Math.max(h.scrollHeight, document.body.scrollHeight) - window.innerHeight;
    const scrolled = max > 0 ? top / max * 100 : 0;
    progress.style.width = scrolled + '%';
  }
  document.addEventListener('scroll', updateProgress, {passive:true, capture:true});

  /* ================= hero aura follows cursor ================= */
  if(fine && !reduced){
    const aura = document.getElementById('aura');
    heroEl.addEventListener('mousemove', (e)=>{
      const r = heroEl.getBoundingClientRect();
      const px = (e.clientX - r.left) - 260;
      const py = (e.clientY - r.top) - 260;
      aura.style.transform = 'translate('+(px*0.15)+'px,'+(py*0.15)+'px)';
    });
  }

  /* ================= scrollspy + nav pill ================= */
  const links = Array.from(document.querySelectorAll('#navLinks a'));
  const sections = links.map(a => document.querySelector(a.getAttribute('href')));
  const pill = document.getElementById('navPill');

  function movePill(link){
    if(!link) return;
    pill.style.left = link.offsetLeft + 'px';
    pill.style.width = link.offsetWidth + 'px';
    pill.style.opacity = '1';
  }

  const io = new IntersectionObserver((entries)=>{
    entries.forEach(entry=>{
      if(entry.isIntersecting){
        const id = '#' + entry.target.id;
        links.forEach(a => a.classList.toggle('active', a.getAttribute('href') === id));
        movePill(links.find(a => a.getAttribute('href') === id));
      }
    });
  }, { rootMargin: '-45% 0px -50% 0px' });
  sections.forEach(s => s && io.observe(s));

  /* ================= scroll reveal ================= */
  const revealIo = new IntersectionObserver((entries)=>{
    entries.forEach((entry, i)=>{
      if(entry.isIntersecting){
        setTimeout(()=> entry.target.classList.add('in-view'), i*40);
        revealIo.unobserve(entry.target);
      }
    });
  }, {threshold:0.15, rootMargin:'0px 0px -60px 0px'});
  document.querySelectorAll('.reveal').forEach(el => revealIo.observe(el));

  /* timeline height reveal */
  const timelineEl = document.getElementById('jobList');
  const jobs = timelineEl.querySelectorAll('.job');
  if(jobs.length){
    const last = jobs[jobs.length-1];
    timelineEl.style.setProperty('--tl-h', (last.offsetTop + 12) + 'px');
  }
  new IntersectionObserver((entries)=>{
    entries.forEach(e=>{ if(e.isIntersecting) timelineEl.classList.add('in-view'); });
  }, {threshold:0.2}).observe(timelineEl);

  /* ================= magnetic elements ================= */
  if(fine && !reduced){
    document.querySelectorAll('[data-magnetic]').forEach(el=>{
      el.addEventListener('mousemove', (e)=>{
        const r = el.getBoundingClientRect();
        const mx = e.clientX - r.left - r.width/2;
        const my = e.clientY - r.top - r.height/2;
        el.style.transform = 'translate('+(mx*0.22)+'px,'+(my*0.35)+'px)';
      });
      el.addEventListener('mouseleave', ()=>{ el.style.transform = 'translate(0,0)'; });
    });
  }

  /* ================= project card tilt + glare ================= */
  if(fine && !reduced){
    document.querySelectorAll('.project-card').forEach(card=>{
      card.addEventListener('mousemove', (e)=>{
        const r = card.getBoundingClientRect();
        const px = (e.clientX - r.left)/r.width;
        const py = (e.clientY - r.top)/r.height;
        const rx = (py-0.5) * -8;
        const ry = (px-0.5) * 8;
        card.style.transform = 'perspective(800px) rotateX('+rx+'deg) rotateY('+ry+'deg) translateZ(0)';
        card.style.setProperty('--mx', (px*100)+'%');
        card.style.setProperty('--my', (py*100)+'%');
      });
      card.addEventListener('mouseleave', ()=>{
        card.style.transform = 'perspective(800px) rotateX(0) rotateY(0)';
      });
    });
  }

  /* ================= portrait tilt ================= */
  if(fine && !reduced){
    const portrait = document.getElementById('portraitWrap');
    if(portrait){
      const mask = portrait.querySelector('.portrait-mask');
      portrait.addEventListener('mousemove', (e)=>{
        const r = portrait.getBoundingClientRect();
        const px = (e.clientX - r.left)/r.width;
        const py = (e.clientY - r.top)/r.height;
        const rx = (py-0.5) * -10;
        const ry = (px-0.5) * 10;
        mask.style.transform = 'perspective(600px) rotateX('+rx+'deg) rotateY('+ry+'deg)';
      });
      portrait.addEventListener('mouseleave', ()=>{
        mask.style.transform = 'perspective(600px) rotateX(0) rotateY(0)';
      });
    }
  }

  /* ---- copy email ---- */
  const copyBtn = document.getElementById('copyEmailBtn');
  copyBtn.addEventListener('click', ()=>{
    navigator.clipboard.writeText('anay06p@gmail.com').then(()=>{
      const original = copyBtn.textContent;
      copyBtn.textContent = 'Copied';
      setTimeout(()=> copyBtn.textContent = original, 1600);
    });
  });

  /* ---- live local time ---- */
  const timeEl = document.getElementById('localTime');
  const dateEl = document.getElementById('localDate');
  function tick(){
    const now = new Date();
    timeEl.textContent = new Intl.DateTimeFormat('en-US', {timeZone:'America/New_York', hour:'2-digit', minute:'2-digit', second:'2-digit', hour12:true}).format(now);
    dateEl.textContent = new Intl.DateTimeFormat('en-US', {timeZone:'America/New_York', weekday:'short', month:'short', day:'numeric'}).format(now);
  }
  tick(); setInterval(tick, 1000);
  document.getElementById('footerYear').textContent = new Intl.DateTimeFormat('en-US', {year:'numeric'}).format(new Date());

  /* ---- command palette ---- */
  const index = [
    {label:'Work experience', hint:'section', target:'#work'},
    {label:'Software Engineer Intern — BDO USA', hint:'work', target:'#work'},
    {label:'Software Engineer & Quant Developer — AlgoGators', hint:'work', target:'#work'},
    {label:'ML Researcher — Digital Worlds Institute', hint:'work', target:'#work'},
    {label:'Projects', hint:'section', target:'#projects'},
    {label:'Visionary', hint:'project', target:'#projects'},
    {label:'ServeUp!', hint:'project', target:'#projects'},
    {label:'Market Mood Mapper', hint:'project', target:'#projects'},
    {label:'Skills', hint:'section', target:'#skills'},
    {label:'Education', hint:'section', target:'#education'},
    {label:'Connect / contact info', hint:'section', target:'#connect'},
  ];
  const overlay = document.getElementById('cmdkOverlay');
  const input = document.getElementById('cmdkInput');
  const results = document.getElementById('cmdkResults');
  let selectedIdx = 0;
  let currentList = [];

  function renderResults(query){
    const q = query.trim().toLowerCase();
    currentList = index.filter(i => i.label.toLowerCase().includes(q));
    results.innerHTML = '';
    if(currentList.length === 0){ results.innerHTML = '<div class="cmdk-empty">No matches</div>'; return; }
    currentList.forEach((item, i)=>{
      const el = document.createElement('div');
      el.className = 'cmdk-item' + (i === selectedIdx ? ' selected' : '');
      el.innerHTML = '<span>' + item.label + '</span><span class="tag-small">' + item.hint + '</span>';
      el.addEventListener('click', ()=> go(item));
      results.appendChild(el);
    });
  }
  function go(item){ closeCmdk(); document.querySelector(item.target).scrollIntoView({behavior:'smooth', block:'start'}); }
  function openCmdk(){ overlay.classList.add('open'); input.value=''; selectedIdx=0; renderResults(''); setTimeout(()=> input.focus(), 30); }
  function closeCmdk(){ overlay.classList.remove('open'); }

  document.getElementById('cmdkOpen').addEventListener('click', openCmdk);
  overlay.addEventListener('click', (e)=>{ if(e.target === overlay) closeCmdk(); });
  input.addEventListener('input', ()=>{ selectedIdx = 0; renderResults(input.value); });

  document.addEventListener('keydown', (e)=>{
    const typing = ['INPUT','TEXTAREA'].includes(document.activeElement.tagName);
    if(e.key === '/' && !typing){ e.preventDefault(); openCmdk(); }
    else if(e.key === 'Escape' && overlay.classList.contains('open')){ closeCmdk(); }
    else if(overlay.classList.contains('open')){
      if(e.key === 'ArrowDown'){ e.preventDefault(); selectedIdx = Math.min(selectedIdx+1, currentList.length-1); renderResults(input.value); }
      if(e.key === 'ArrowUp'){ e.preventDefault(); selectedIdx = Math.max(selectedIdx-1, 0); renderResults(input.value); }
      if(e.key === 'Enter' && currentList[selectedIdx]){ go(currentList[selectedIdx]); }
    }
  });

  window.addEventListener('resize', ()=> movePill(document.querySelector('.nav-links a.active')));

  /* ================= nav link hover scramble ================= */
  if(!reduced){
    document.querySelectorAll('.nav-links a').forEach(link=>{
      const original = link.textContent;
      link.addEventListener('mouseenter', ()=> scrambleText(link, original, 22));
    });
  }

  /* ================= cursor flock: builds the page, flies like birds, then leaves ================= */

  /* Splits an element's text into per-character spans (hidden) so a cursor can "type" it in
     without changing the layout. */
  function charify(el){
    if(el._chars) return el._chars;
    const chars = [];
    const walker = document.createTreeWalker(el, NodeFilter.SHOW_TEXT);
    const nodes = [];
    while(walker.nextNode()) nodes.push(walker.currentNode);
    nodes.forEach(n=>{
      const text = n.nodeValue;
      if(!text) return;
      const frag = document.createDocumentFragment();
      for(const ch of text){
        const sp = document.createElement('span');
        sp.className = 'cx';
        sp.textContent = ch;
        sp.style.visibility = 'hidden';
        frag.appendChild(sp);
        chars.push(sp);
      }
      n.parentNode.replaceChild(frag, n);
    });
    el._chars = chars;
    return chars;
  }

  /* Every "unit" starts hidden; a cursor performs some action on it and it appears. */
  function initBuildUnits(){
    if(!cbMode) return;
    document.body.classList.add('cb-mode');

    const add = (el, kind, hero)=>{
      const u = {el, kind, hero: !!hero, built:false, queued: !!hero, taken: !!hero, queuedAt:0,
                 typeEl:null, idxEl:null, plan:null, touched:false};
      if(kind === 'name') u.typeEl = el;
      if(kind === 'desc' || kind === 'role' || kind === 'year') u.typeEl = el;
      if(kind === 'kicker') u.typeEl = el.querySelector('.kicker') || el;
      if(kind === 'head'){ u.typeEl = el.querySelector('h2'); u.idxEl = el.querySelector('.section-index'); }
      el.classList.add('cb-hidden');
      units.push(u);
      return u;
    };

    [['#heroName','name'], ['.hero-copy .reveal-mask','kicker'], ['#portraitWrap','portrait'], ['#roleLine','role'],
     ['.hero-desc','desc'], ['.hero-cta','cta'], ['.title-block','meta'], ['#tileField','tiles']
    ].forEach(([sel, kind])=>{
      const el = document.querySelector(sel);
      if(!el) return;
      if(kind === 'tiles' && getComputedStyle(el).display === 'none') return;
      add(el, kind, true);
    });

    [['#work .section-head','head'], ['#work .job','job'],
     ['#projects .section-head','head'], ['#projects .project-card','card'],
     ['#skills .section-head','head'], ['#skills .skill-module','module'],
     ['#education .section-head','head'], ['#education .edu-row','edurow'], ['#education .course-chips','chips'], ['#education .edu-year','year'],
     ['#connect .section-head','head'], ['#connect .connect-panel','panel']
    ].forEach(([sel, kind])=>{
      document.querySelectorAll(sel).forEach(el => add(el, kind, false));
    });
  }
  initBuildUnits();

  function finalizeUnit(u, fade){
    if(u.built) return;
    u.built = true;
    const el = u.el;
    el.style.clipPath = '';
    if(u.touched){ el.style.transform = ''; el.style.opacity = ''; }
    if(fade){
      el.style.transition = 'opacity 0.6s ease';
      setTimeout(()=>{ el.style.transition = ''; }, 700);
    } else {
      el.style.transition = '';
    }
    el.classList.remove('cb-hidden');
    if(u.kind === 'name'){
      if(!heroNameEl._chars) heroNameEl.textContent = heroNameFinal;
      heroEl.classList.add('name-drawn');
    }
    if(u.typeEl && u.typeEl._chars) u.typeEl._chars.forEach(c => { c.style.visibility = ''; });
    if(u.idxEl) u.idxEl.style.visibility = '';
  }
  function revealAllNow(){ units.forEach(u => finalizeUnit(u, true)); }

  let swarmStarted = false;
  function startSwarm(){
    if(swarmStarted || !cbMode) return;
    swarmStarted = true;
    try { runSwarm(); }
    catch(err){ console.error('cursor flock failed, revealing page', err); revealAllNow(); }
  }

  function runSwarm(){
    const COLORS = ['#6BB6E0','#E8A33D','#A78BFA','#5FCB8C','#F472B6','#F87171','#38BDF8','#FDE68A'];
    const COUNT = 8;
    const ARROW = '<svg viewBox="0 0 18 22" width="18" height="22"><path d="M2 1.5 L2 17.5 L6.1 13.6 L8.9 20.2 L11.6 19 L8.8 12.6 L14.2 12.4 Z" fill="currentColor" stroke="#0B1220" stroke-width="1.3" stroke-linejoin="round"/></svg>';
    const clamp = (v, a, b) => Math.max(a, Math.min(b, v));
    const ease = t => t < 0.5 ? 4*t*t*t : 1 - Math.pow(-2*t + 2, 3)/2;            // in-out cubic
    const easeOutBack = t => 1 + 2.70158*Math.pow(t - 1, 3) + 1.70158*Math.pow(t - 1, 2);
    const ARROW_FRONT = 115.6; // degrees to rotate the arrow glyph so its tip leads the direction of travel
    const OVER = '-36px';      // lets clipped elements keep overflow (e.g. the timeline dot) while revealing
    /* Where the page-anchored layer currently sits on screen (it moves with the page when you scroll). */
    const LR = {left:0, top:0};

    /* ---------- what each kind of thing gets done to it ---------- */
    const POOLS = {
      name:['type'], kicker:['edge'], portrait:['corner'], role:['edge'], desc:['type'], cta:['pop'], meta:['edge'], tiles:['paint'],
      head:['type','type','edge'], year:['type'],
      job:['corner','paint','edge'], card:['corner','pop'], module:['pop','corner','edge','paint'],
      edurow:['edge','corner'], chips:['paint','pop','edge'], panel:['corner','pop']
    };
    const EDGE_DIR = {kicker:'right', role:'down', meta:'right', head:'right'};
    const recent = [];
    function pickAction(u){
      const pool = POOLS[u.kind] || ['corner'];
      let choices = pool.filter(a => !recent.includes(a));
      if(!choices.length) choices = pool;
      const type = choices[Math.floor(Math.random()*choices.length)];
      recent.push(type); if(recent.length > 2) recent.shift();
      const plan = {
        type, dir:'down',
        ax: 0, ay: 0,
        ox: (Math.random() - 0.5)*160, oy: -(70 + Math.random()*50), rot: (Math.random() - 0.5)*8
      };
      if(type === 'edge') plan.dir = EDGE_DIR[u.kind] || ['down','right'][Math.floor(Math.random()*2)];
      return plan;
    }
    const paintRows = r => clamp(Math.round(r.height/48), 2, 6);

    /* where the cursor has to be to begin the action */
    function startPoint(u){
      const pl = u.plan, r = u.el.getBoundingClientRect();
      switch(pl.type){
        case 'corner': return {x: r.left + pl.ax*r.width, y: r.top + pl.ay*r.height};
        case 'edge':
          if(pl.dir === 'down')  return {x: r.left + r.width/2, y: r.top};
          if(pl.dir === 'up')    return {x: r.left + r.width/2, y: r.bottom};
          if(pl.dir === 'right') return {x: r.left,  y: r.top + r.height/2};
          return {x: r.right, y: r.top + r.height/2};
        case 'type': {
          const te = u.typeEl || u.el, tr = te.getBoundingClientRect();
          const lh = parseFloat(getComputedStyle(te).lineHeight) || 20;
          return {x: tr.left + 5, y: tr.top + Math.min(tr.height/2, lh/2)};
        }
        case 'drop': return {x: r.left + r.width/2 + pl.ox, y: r.top + r.height/2 + pl.oy};
        case 'pop':  return {x: r.left + r.width/2, y: r.top + r.height/2};
        default:     return {x: r.left + 2, y: r.top + r.height/(2*paintRows(r))};   // paint
      }
    }

    /* ---------- layers ---------- */
    const trailCanvas = document.createElement('canvas');
    trailCanvas.id = 'ghostTrails';
    document.body.appendChild(trailCanvas);
    const tctx = trailCanvas.getContext('2d');
    const dpr = Math.min(2, window.devicePixelRatio || 1);
    function sizeCanvas(){
      trailCanvas.width = Math.round(window.innerWidth * dpr);
      trailCanvas.height = Math.round(window.innerHeight * dpr);
      tctx.setTransform(dpr, 0, 0, dpr, 0, 0);
    }
    sizeCanvas();
    window.addEventListener('resize', sizeCanvas);

    const layer = document.createElement('div');
    layer.id = 'ghostLayer';
    layer.setAttribute('aria-hidden', 'true');
    const curLayer = document.createElement('div');           // flying / flocking cursors (fixed to the screen)
    layer.appendChild(curLayer);
    document.body.appendChild(layer);

    const docLayer = document.createElement('div');           // selection boxes, carets, working cursors (glued to the page)
    docLayer.id = 'ghostDoc';
    docLayer.setAttribute('aria-hidden', 'true');
    const selLayer = document.createElement('div');
    const docCur = document.createElement('div');
    docLayer.appendChild(selLayer);
    docLayer.appendChild(docCur);
    document.body.appendChild(docLayer);

    /* ---------- cursors ---------- */
    const ghosts = [];
    const t0 = performance.now();
    const vw0 = window.innerWidth, vh0 = window.innerHeight;
    const heroUnits = units.filter(u => u.hero);

    for(let i = 0; i < COUNT; i++){
      const color = COLORS[i % COLORS.length];
      const root = document.createElement('div');
      root.className = 'gc';
      root.style.setProperty('--c', color);
      root.innerHTML = '<div class="gc-arrow">' + ARROW + '</div>';
      curLayer.appendChild(root);

      const sel = document.createElement('div');
      sel.className = 'gc-select';
      sel.style.setProperty('--c', color);
      sel.innerHTML = '<i class="tl"></i><i class="tr"></i><i class="bl"></i><i class="br"></i><span class="gc-tag"></span>';
      selLayer.appendChild(sel);

      const g = {
        idx:i, color, root, sel,
        arrow: root.querySelector('.gc-arrow'), selTag: sel.querySelector('.gc-tag'),
        x:0, y:0, px:0, py:0, vx:0, vy:0, rot:0, phase: Math.random()*6.28,
        state:'flock', sub:null, task:null, plan:null, subStart:0, startAt:0, lead:0, dur:0, holdMs:0,
        fsx:0, fsy:0, flyDist:0, flyDur:0, arcSign: i % 2 ? 1 : -1,
        chars:null, typed:0, caret:null, rows:1, gone:false, inDoc:false, plx:0, ply:0
      };

      const u = heroUnits[i];
      let sx, sy;
      if(u){
        /* hero cursors enter from the screen edge nearest the thing they will work on */
        u.plan = pickAction(u);
        const sp = startPoint(u);
        const dl = sp.x, dr = vw0 - sp.x, dt_ = sp.y, db = vh0 - sp.y, m = Math.min(dl, dr, dt_, db);
        const jy = clamp(sp.y + (Math.random() - 0.5)*120, 20, vh0 - 20), jx = clamp(sp.x + (Math.random() - 0.5)*120, 20, vw0 - 20);
        if(m === dl){ sx = -50; sy = jy; } else if(m === dr){ sx = vw0 + 50; sy = jy; }
        else if(m === dt_){ sx = jx; sy = -50; } else { sx = jx; sy = vh0 + 50; }
        g.state = 'work'; g.sub = 'wait'; g.task = u; g.plan = u.plan; g.startAt = t0 + 300 + i*170;
      } else {
        switch(i % 4){
          case 0:  sx = -50;          sy = Math.random()*vh0; break;
          case 1:  sx = vw0 + 50;     sy = Math.random()*vh0; break;
          case 2:  sx = Math.random()*vw0; sy = vh0 + 50;     break;
          default: sx = Math.random()*vw0; sy = -50;
        }
        const a = Math.atan2(vh0/2 - sy, vw0/2 - sx);
        g.vx = Math.cos(a)*190; g.vy = Math.sin(a)*190;
      }
      g.x = g.px = sx; g.y = g.py = sy;
      root.style.transform = 'translate3d(' + sx + 'px,' + sy + 'px,0)';
      ghosts.push(g);
      requestAnimationFrame(()=> root.classList.add('on'));
    }

    function ripple(x, y, color){
      const r = document.createElement('div');
      r.className = 'gc-ripple';
      r.style.left = (x - LR.left) + 'px';
      r.style.top = (y - LR.top) + 'px';
      r.style.setProperty('--c', color);
      docCur.appendChild(r);
      setTimeout(()=> r.remove(), 750);
    }
    function setSelection(g, left, top, w, h){
      g.sel.style.transform = 'translate3d(' + (left - LR.left).toFixed(1) + 'px,' + (top - LR.top).toFixed(1) + 'px,0)';
      g.sel.style.width = Math.max(0, w).toFixed(1) + 'px';
      g.sel.style.height = Math.max(0, h).toFixed(1) + 'px';
      g.selTag.textContent = Math.round(w) + ' × ' + Math.round(h);
    }

    function enterDoc(g){                       // from here on the browser scrolls this cursor with the text
      docCur.appendChild(g.root);
      g.inDoc = true; g.plx = g.x - LR.left; g.ply = g.y - LR.top;
    }
    function exitDoc(g){
      if(!g.inDoc) return;
      curLayer.appendChild(g.root);
      g.inDoc = false;
    }

    /* ---------- flight: a straight, timed glide to the start point (follows the target if the page scrolls) ---------- */
    function startFlight(g, now){
      g.sub = 'fly'; g.subStart = now; g.fsx = g.x; g.fsy = g.y;
      const sp = startPoint(g.task);
      g.flyDist = Math.hypot(sp.x - g.x, sp.y - g.y);
      g.flyDur = clamp(g.flyDist/1.5 + 180, 280, 900);     // ~1500px/s plus a short ramp
    }

    /* ---------- the actions ---------- */
    function cornerClip(pl, e){
      const far = ((1 - e)*100).toFixed(2) + '%';
      const L = pl.ax === 0 ? OVER : far, R = pl.ax === 0 ? far : OVER;
      const T = pl.ay === 0 ? OVER : far, B = pl.ay === 0 ? far : OVER;
      return 'inset(' + T + ' ' + R + ' ' + B + ' ' + L + ')';
    }
    function edgeClip(dir, e){
      const far = ((1 - e)*100).toFixed(2) + '%';
      if(dir === 'down')  return 'inset(' + OVER + ' ' + OVER + ' ' + far + ' ' + OVER + ')';
      if(dir === 'up')    return 'inset(' + far + ' ' + OVER + ' ' + OVER + ' ' + OVER + ')';
      if(dir === 'right') return 'inset(' + OVER + ' ' + far + ' ' + OVER + ' ' + OVER + ')';
      return 'inset(' + OVER + ' ' + OVER + ' ' + OVER + ' ' + far + ')';
    }

    function beginAct(g, now){
      const u = g.task, el = u.el, pl = g.plan;
      const r = el.getBoundingClientRect();
      g.sub = 'act'; g.subStart = now; g.lead = 0; u.touched = true;
      enterDoc(g);
      el.style.transition = 'none';
      let showSel = true;

      if(pl.type === 'corner'){
        g.dur = clamp(380 + Math.hypot(r.width, r.height)*0.35, 480, 950);
        el.style.clipPath = cornerClip(pl, 0);
      }
      else if(pl.type === 'edge'){
        const len = (pl.dir === 'down' || pl.dir === 'up') ? r.height : r.width;
        g.dur = clamp(380 + len*0.45, 450, 900);
        el.style.clipPath = edgeClip(pl.dir, 0);
      }
      else if(pl.type === 'paint'){
        g.rows = paintRows(r);
        g.dur = clamp(500 + g.rows*220, 700, 1500);
        el.style.clipPath = 'polygon(0 0, 0 0, 0 0)';
      }
      else if(pl.type === 'type'){
        if(u.kind === 'name') heroNameEl.textContent = heroNameFinal;
        g.chars = charify(u.typeEl || el);
        g.typed = 0;
        if(u.idxEl) u.idxEl.style.visibility = 'hidden';
        g.lead = 160;
        g.dur = clamp(g.chars.length*18, 450, 1500);
        g.caret = document.createElement('div');
        g.caret.className = 'gc-caret';
        g.caret.style.setProperty('--c', g.color);
        docCur.appendChild(g.caret);
      }
      else if(pl.type === 'drop'){
        g.dur = 700;
        el.style.opacity = '0';
        el.style.transform = 'translate(' + pl.ox + 'px,' + pl.oy + 'px) rotate(' + pl.rot + 'deg) scale(0.95)';
      }
      else { // pop
        g.dur = 420; g.lead = 140; showSel = false;
        el.style.opacity = '0';
        el.style.transform = 'scale(0.8)';
      }

      el.classList.remove('cb-hidden');
      g.root.classList.add('press');
      ripple(g.x, g.y, g.color);
      if(showSel) g.sel.classList.add('on');
    }

    function runAct(g, now, dt){
      const u = g.task, el = u.el, pl = g.plan;
      const live = el.getBoundingClientRect();
      if(live.bottom < -20 || live.top > window.innerHeight + 20){      // scrolled completely away: wrap it up quietly
        finalizeUnit(u, false);
        if(g.caret){ g.caret.remove(); g.caret = null; }
        g.sel.classList.remove('on');
        g.x = clamp(g.x, 40, window.innerWidth - 40); g.y = clamp(g.y, 40, window.innerHeight - 40);
        exitDoc(g);
        g.sub = 'hold'; g.subStart = now; g.holdMs = 60;
        g.vx = 0; g.vy = 0; g.px = g.x; g.py = g.y;
        return;
      }
      const r = live;
      const p = clamp((now - g.subStart - g.lead)/g.dur, 0, 1);

      if(pl.type === 'corner'){
        const e = ease(p);
        g.x = r.left + (pl.ax === 0 ? e : 1 - e)*r.width;
        g.y = r.top  + (pl.ay === 0 ? e : 1 - e)*r.height;
        el.style.clipPath = cornerClip(pl, e);
        setSelection(g, pl.ax === 0 ? r.left : r.left + (1 - e)*r.width, pl.ay === 0 ? r.top : r.top + (1 - e)*r.height, r.width*e, r.height*e);
      }
      else if(pl.type === 'edge'){
        const e = ease(p);
        el.style.clipPath = edgeClip(pl.dir, e);
        if(pl.dir === 'down'){  g.x = r.left + r.width/2; g.y = r.top + e*r.height;    setSelection(g, r.left, r.top, r.width, r.height*e); }
        if(pl.dir === 'up'){    g.x = r.left + r.width/2; g.y = r.bottom - e*r.height; setSelection(g, r.left, r.bottom - e*r.height, r.width, r.height*e); }
        if(pl.dir === 'right'){ g.x = r.left + e*r.width;  g.y = r.top + r.height/2;   setSelection(g, r.left, r.top, r.width*e, r.height); }
        if(pl.dir === 'left'){  g.x = r.right - e*r.width; g.y = r.top + r.height/2;   setSelection(g, r.right - e*r.width, r.top, r.width*e, r.height); }
      }
      else if(pl.type === 'paint'){
        const N = g.rows, q = p*N, i = Math.min(N - 1, Math.floor(q)), f = q - i;
        const ltr = i % 2 === 0, xe = ((ltr ? f : 1 - f)*100).toFixed(2);
        const y0 = (i/N*100).toFixed(2), y1 = ((i + 1)/N*100).toFixed(2);
        el.style.clipPath = ltr
          ? 'polygon(0 0, 100% 0, 100% ' + y0 + '%, ' + xe + '% ' + y0 + '%, ' + xe + '% ' + y1 + '%, 0 ' + y1 + '%)'
          : 'polygon(0 0, 100% 0, 100% ' + y1 + '%, ' + xe + '% ' + y1 + '%, ' + xe + '% ' + y0 + '%, 0 ' + y0 + '%)';
        g.x = r.left + (ltr ? f : 1 - f)*r.width;
        g.y = r.top + (i + 0.5)/N*r.height;
        setSelection(g, r.left, r.top, r.width, r.height);
      }
      else if(pl.type === 'type'){
        const sp = startPoint(u);
        g.x = sp.x; g.y = sp.y;                       // pointer stays where it clicked
        const n = Math.floor(p*g.chars.length);
        while(g.typed < n){ g.chars[g.typed].style.visibility = ''; g.typed++; }
        const cr = (g.typed > 0 ? g.chars[g.typed - 1] : g.chars[0]).getBoundingClientRect();
        g.caret.style.height = cr.height + 'px';
        g.caret.style.transform = 'translate3d(' + ((g.typed > 0 ? cr.right : cr.left) - LR.left).toFixed(1) + 'px,' + (cr.top - LR.top).toFixed(1) + 'px,0)';
        const tr = (u.typeEl || el).getBoundingClientRect();
        setSelection(g, tr.left - 4, tr.top - 3, tr.width + 8, tr.height + 6);
      }
      else if(pl.type === 'drop'){
        const f = 1 - ease(p);
        el.style.transform = 'translate(' + (pl.ox*f).toFixed(1) + 'px,' + (pl.oy*f).toFixed(1) + 'px) rotate(' + (pl.rot*f).toFixed(2) + 'deg) scale(' + (1 - 0.05*f).toFixed(3) + ')';
        el.style.opacity = String(Math.min(1, p*4));
        g.x = r.left + r.width/2; g.y = r.top + r.height/2;   // the cursor is carrying it by the middle
        setSelection(g, r.left, r.top, r.width, r.height);
      }
      else { // pop
        el.style.transform = 'scale(' + (0.8 + 0.2*easeOutBack(p)).toFixed(3) + ')';
        el.style.opacity = String(Math.min(1, p*4));
        g.x = r.left + r.width/2; g.y = r.top + r.height/2;
      }

      /* motion is measured in page coordinates, so scrolling never shows up as cursor speed (or a streaky trail) */
      const lx = g.x - LR.left, ly = g.y - LR.top;
      g.px = g.plx + LR.left; g.py = g.ply + LR.top;
      g.vx = clamp((lx - g.plx)/Math.max(dt, 0.001), -2500, 2500);
      g.vy = clamp((ly - g.ply)/Math.max(dt, 0.001), -2500, 2500);
      g.plx = lx; g.ply = ly;

      if(p >= 1){
        finalizeUnit(u, false);
        if(pl.type === 'drop') ripple(g.x, g.y, g.color);
        g.sub = 'hold'; g.subStart = now;
        g.holdMs = pl.type === 'type' ? 280 : (pl.type === 'pop' ? 120 : 220);
      }
    }

    /* ---------- shared helpers ---------- */
    function integrate(g, dt, maxSp){
      let sp = Math.hypot(g.vx, g.vy);
      if(sp > maxSp){ g.vx *= maxSp/sp; g.vy *= maxSp/sp; sp = maxSp; }
      g.px = g.x; g.py = g.y;
      g.x += g.vx*dt; g.y += g.vy*dt;
      return sp;
    }
    function drawTrail(g, sp){
      if(sp < 30) return;
      tctx.lineCap = 'round';
      tctx.strokeStyle = g.color;
      tctx.beginPath(); tctx.moveTo(g.px, g.py); tctx.lineTo(g.x, g.y);
      tctx.globalAlpha = Math.min(0.16, sp/7000); tctx.lineWidth = 7;   tctx.stroke();
      tctx.globalAlpha = Math.min(0.6,  sp/1800); tctx.lineWidth = 1.8; tctx.stroke();
      tctx.globalAlpha = 1;
    }

    let leaving = false, finished = false, allGoneAt = 0, lastAssignAt = 0;
    const startedAt = performance.now();

    /* ---------- one simulation step for one cursor ---------- */
    function step(g, now, dt, env){
      let sp = 0, targetRot = 0;

      if(g.state === 'work'){
        if(g.sub === 'wait'){
          if(now < g.startAt) return;
          startFlight(g, now);
        }
        const u = g.task;
        if(u.built && g.sub !== 'hold'){ g.sub = 'hold'; g.subStart = now; g.holdMs = 120; }

        if(g.sub === 'fly'){
          const T = startPoint(u);
          const t = clamp((now - g.subStart)/g.flyDur, 0, 1), e = 1 - Math.pow(1 - t, 3);   // ease-out: fast off the mark, soft landing
          const dxv = T.x - g.fsx, dyv = T.y - g.fsy, dist = Math.hypot(dxv, dyv) || 1;
          const arc = Math.sin(Math.PI*e)*Math.min(50, g.flyDist*0.04)*g.arcSign;           // barely-there curve so it feels human
          const nx = g.fsx + dxv*e - (dyv/dist)*arc, ny = g.fsy + dyv*e + (dxv/dist)*arc;
          g.vx = clamp((nx - g.x)/Math.max(dt, 0.001), -3500, 3500);
          g.vy = clamp((ny - g.y)/Math.max(dt, 0.001), -3500, 3500);
          g.px = g.x; g.py = g.y; g.x = nx; g.y = ny;
          sp = Math.hypot(g.vx, g.vy);
          targetRot = clamp(g.vx*0.012, -16, 16);
          if(t >= 1) beginAct(g, now);
        }
        else if(g.sub === 'act'){
          runAct(g, now, dt);
          sp = Math.hypot(g.vx, g.vy);
        }
        else if(g.sub === 'hold'){
          g.vx = 0; g.vy = 0;
          if(g.inDoc){ g.x = g.plx + LR.left; g.y = g.ply + LR.top; }
          g.px = g.x; g.py = g.y;
          if(g.sel.classList.contains('on')){
            const rr = (g.plan.type === 'type' ? (u.typeEl || u.el) : u.el).getBoundingClientRect();
            if(g.plan.type === 'type') setSelection(g, rr.left - 4, rr.top - 3, rr.width + 8, rr.height + 6);   // same padding as while typing
            else setSelection(g, rr.left, rr.top, rr.width, rr.height);
          }
          if(now - g.subStart > g.holdMs){
            if(g.plan.type === 'type' || g.plan.type === 'pop') ripple(g.x, g.y, g.color);
            if(g.caret){ g.caret.remove(); g.caret = null; }
            g.root.classList.remove('press');
            g.sel.classList.remove('on');
            exitDoc(g);
            g.task = null; g.plan = null; g.sub = null; g.state = 'flock';
            const a = Math.atan2(env.wp.y - g.y, env.wp.x - g.x) + (Math.random() - 0.5)*0.9;
            g.vx = Math.cos(a)*190; g.vy = Math.sin(a)*190;
          }
        }
      }
      else if(g.state === 'flock' || g.state === 'leave'){
        let ax = 0, ay = 0;
        const group = g.state === 'leave' ? env.leavers : env.flockers;

        /* separation: don't stack on neighbours */
        for(const o of group){
          if(o === g) continue;
          const dx = g.x - o.x, dy = g.y - o.y, d = Math.hypot(dx, dy);
          if(d > 0.5 && d < 54){
            const f = (54 - d)/54*600;
            ax += dx/d*f; ay += dy/d*f;
          }
        }

        if(g.state === 'flock'){
          if(group.length > 1){
            ax += (env.cx - g.x)*0.4 + (env.avx - g.vx)*1.6;   // cohesion + alignment
            ay += (env.cy - g.y)*0.4 + (env.avy - g.vy)*1.6;
          }
          const wdx = env.wp.x - g.x, wdy = env.wp.y - g.y, wd = Math.hypot(wdx, wdy) || 1;
          ax += wdx/wd*120; ay += wdy/wd*120;                     // the flock chases a slow-moving waypoint
          const m = 90;                                           // soft walls
          if(g.x < m) ax += (m - g.x)*5;
          if(g.x > env.W - m) ax -= (g.x - (env.W - m))*5;
          if(g.y < m) ay += (m - g.y)*5;
          if(g.y > env.H - m) ay -= (g.y - (env.H - m))*5;
          ax += Math.sin(now/420 + g.phase)*22;                   // a little wing-flutter
          ay += Math.cos(now/460 + g.phase*1.3)*22;
        } else {
          const ex = env.W + 420 - g.x, ey = -320 - g.y, ed = Math.hypot(ex, ey) || 1;
          ax += ex/ed*800; ay += ey/ed*800;                       // everyone peels off toward the same corner
          if(group.length > 1){
            ax += (env.avx - g.vx)*1.2; ay += (env.avy - g.vy)*1.2;
          }
        }

        g.vx += ax*dt; g.vy += ay*dt;
        const maxSp = g.state === 'leave' ? 900 : 270;
        sp = Math.hypot(g.vx, g.vy);
        if(g.state === 'flock' && sp < 130){
          if(sp < 1){ const a = Math.random()*6.28; g.vx = Math.cos(a)*130; g.vy = Math.sin(a)*130; }
          else { g.vx *= 130/sp; g.vy *= 130/sp; }
        }
        sp = integrate(g, dt, maxSp);
        targetRot = Math.atan2(g.vy, g.vx)*180/Math.PI + ARROW_FRONT;

        if(g.state === 'leave' && (g.x > env.W + 60 || g.y < -60)){
          g.gone = true;
          g.root.style.display = 'none';
        }
      }

      drawTrail(g, sp);

      const diff = ((targetRot - g.rot + 540) % 360) - 180;
      g.rot += diff*Math.min(1, dt*6);
      g.arrow.style.transform = 'rotate(' + g.rot.toFixed(1) + 'deg)';
      g.root.style.transform = g.inDoc
        ? 'translate3d(' + (g.x - LR.left).toFixed(1) + 'px,' + (g.y - LR.top).toFixed(1) + 'px,0)'
        : 'translate3d(' + g.x.toFixed(1) + 'px,' + g.y.toFixed(1) + 'px,0)';
    }

    function cleanup(){
      finished = true;
      window.removeEventListener('resize', sizeCanvas);
      layer.remove();
      docLayer.remove();
      trailCanvas.remove();
    }

    /* ---------- main loop ---------- */
    let lastT = performance.now();
    function frame(now){
      if(finished) return;
      requestAnimationFrame(frame);
      try { tick(now); }
      catch(err){ console.error('cursor flock error, revealing page', err); revealAllNow(); cleanup(); }
    }
    function tick(now){
      const dt = Math.min(0.05, (now - lastT)/1000);
      lastT = now;
      const W = window.innerWidth, H = window.innerHeight;
      const lb = docLayer.getBoundingClientRect();     // where the page-anchored layer is right now
      LR.left = lb.left; LR.top = lb.top;

      if(W < 700){            // tiny viewport: skip the show, just make sure everything is visible
        revealAllNow();
        cleanup();
        return;
      }

      tctx.globalCompositeOperation = 'destination-out';
      tctx.fillStyle = 'rgba(0,0,0,0.09)';
      tctx.fillRect(0, 0, W, H);
      tctx.globalCompositeOperation = 'source-over';

      if(!leaving){
        /* queue anything that has scrolled into view; anything scrolled past appears instantly */
        for(const u of units){
          if(u.built || u.queued) continue;
          const r = u.el.getBoundingClientRect();
          if(r.width < 2 && r.height < 2) continue;
          if(r.bottom < 0) finalizeUnit(u, false);
          else if(r.top < H*0.95){ u.queued = true; u.queuedAt = now; }
        }
        /* hand waiting units to the nearest free bird, one at a time */
        for(const u of units){
          if(!u.queued || u.taken || u.built) continue;
          if(now - lastAssignAt < 150) break;
          if(!u.plan) u.plan = pickAction(u);
          const sp = startPoint(u);
          let best = null, bd = 1e9;
          for(const g of ghosts){
            if(g.state !== 'flock') continue;
            const d = Math.hypot(g.x - sp.x, g.y - sp.y);
            if(d < bd){ bd = d; best = g; }
          }
          if(best){
            best.state = 'work'; best.task = u; best.plan = u.plan;
            startFlight(best, now);
            u.taken = true;
            lastAssignAt = now;
            break;
          }
        }
        /* safety nets so nothing is ever left hidden */
        for(const u of units){
          if(u.built) continue;
          if(!u.taken && u.queued){
            const rr = u.el.getBoundingClientRect();
            const waited = now - u.queuedAt;
            if((rr.top < H*0.85 && waited > 2400) || waited > 5000) finalizeUnit(u, true);
          }
          if(u.hero && now - startedAt > 14000) finalizeUnit(u, true);
        }
        /* whole page seen and animated in -> the flock leaves */
        if(units.every(u => u.built) && ghosts.every(g => g.state !== 'work')){
          leaving = true;
          ghosts.forEach(g => { g.state = 'leave'; g.sel.classList.remove('on'); });
        }
      }

      const flockers = ghosts.filter(g => g.state === 'flock');
      const leavers = ghosts.filter(g => g.state === 'leave');
      const env = {W, H, flockers, leavers, cx:0, cy:0, avx:0, avy:0,
        wp: { x: W*(0.5 + 0.33*Math.sin(now/1000*0.3)), y: H*(0.5 + 0.28*Math.sin(now/1000*0.4 + 1.3)) }};
      const grp = leaving ? leavers : flockers;
      if(grp.length){
        for(const g of grp){ env.cx += g.x; env.cy += g.y; env.avx += g.vx; env.avy += g.vy; }
        env.cx /= grp.length; env.cy /= grp.length; env.avx /= grp.length; env.avy /= grp.length;
      }

      for(const g of ghosts){ if(!g.gone) step(g, now, dt, env); }

      if(leaving && ghosts.every(g => g.gone)){
        if(!allGoneAt) allGoneAt = now;
        if(now - allGoneAt > 1000) cleanup();     // let the last trails fade out first
      }
    }
    requestAnimationFrame(frame);
  }
})();
</script>
</body>
</html>
