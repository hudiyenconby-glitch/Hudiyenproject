<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<meta name="color-scheme" content="light dark">
<title>Hudiyen Project | Çalışmalarımız ve Proje Durumu</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,300;12..96,500;12..96,700&family=Manrope:wght@400;500;600&family=Syncopate:wght@700&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#f5f5f3; --bg2:#ebebe8; --card:#ffffff; --fg:#000000; --muted:#5f5f5c;
  --line:rgba(0,0,0,.14); --line2:#d9d9d5; --gray:#4d4d4d; --blue:#2447d8; --blue-soft:rgba(36,71,216,.12);
  --display:"Bricolage Grotesque","Helvetica Neue",Arial,sans-serif;
  --body:"Manrope","Helvetica Neue",Arial,sans-serif;
  --logo:"CheckFor","Syncopate","Helvetica Neue",Arial,sans-serif;
  box-sizing:border-box;
  padding-top:env(safe-area-inset-top,0px);
  padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){
    --bg:#0e0e0e; --bg2:#171717; --card:#1b1b1b; --fg:#f4f4f1; --muted:#9a9a95;
    --line:rgba(255,255,255,.16); --line2:#303030; --gray:#9b9b9b; --blue:#6f8bff; --blue-soft:rgba(111,139,255,.16);
  }
}
:root[data-theme="dark"]{
  --bg:#0e0e0e; --bg2:#171717; --card:#1b1b1b; --fg:#f4f4f1; --muted:#9a9a95;
  --line:rgba(255,255,255,.16); --line2:#303030; --gray:#9b9b9b; --blue:#6f8bff; --blue-soft:rgba(111,139,255,.16);
}
*,*::before,*::after{box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:calc(env(safe-area-inset-top,0px) + 80px)}
body{margin:0;background:var(--bg);color:var(--fg);font-family:var(--body);font-size:16px;line-height:1.6;-webkit-font-smoothing:antialiased;overflow-x:hidden}
a{color:inherit}
button,input{font:inherit;color:inherit}
:focus-visible{outline:2px solid var(--blue);outline-offset:3px}
h1,h2,h3{font-family:var(--display);font-weight:300;letter-spacing:-.02em;line-height:1.05;margin:0}

/* header */
.top{position:sticky;top:env(safe-area-inset-top,0px);z-index:30;display:flex;align-items:center;justify-content:space-between;gap:16px;padding:12px clamp(16px,4vw,48px);background:color-mix(in srgb,var(--bg) 88%,transparent);backdrop-filter:blur(10px);border-bottom:1px solid var(--line)}
.brand{display:flex;align-items:center;gap:12px;text-decoration:none}
.brand .logo{width:38px;height:38px;flex:none}
.word{font-family:var(--logo);font-weight:700;font-size:15px;letter-spacing:.14em}
nav{display:flex;align-items:center;gap:6px}
nav a{text-decoration:none;font-weight:500;font-size:14px;padding:9px 14px;border-radius:999px;transition:background .2s,color .2s}
nav a:hover{background:var(--bg2)}
nav a.on{background:var(--bg2)}
nav a.cta{background:var(--fg);color:var(--bg)}
nav a.cta:hover{background:var(--blue);color:#fff}
.brand{flex:none}
.brand [data-logo]{display:block;flex:none;line-height:0}
@media (max-width:560px){.top{flex-wrap:wrap;row-gap:8px;padding-top:10px;padding-bottom:10px}.word{font-size:13px}nav{width:100%}nav a{flex:1;text-align:center;padding:8px 6px;font-size:13px;white-space:nowrap}}

/* logo drawing */
.logo{display:block;color:var(--fg)}
.logo .p{stroke-dasharray:1;stroke-dashoffset:0}
.logo.draw .p{stroke-dashoffset:1;animation:draw 1.5s cubic-bezier(.65,0,.25,1) forwards}
.logo.draw .c1{animation-delay:.1s}.logo.draw .c2{animation-delay:.35s}.logo.draw .c3{animation-delay:.55s}
.logo.draw .b1{animation-delay:.75s}.logo.draw .b2{animation-delay:.95s}.logo.draw .b3{animation-delay:1.15s}
@keyframes draw{to{stroke-dashoffset:0}}

/* pages */
.page{display:none}
.page.active{display:block;animation:pagein .6s cubic-bezier(.2,.7,.2,1)}
@keyframes pagein{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:none}}

/* hero */
.hero{position:relative;min-height:calc(100vh - 140px);min-height:calc(100svh - 140px);display:grid;grid-template-columns:1.1fr .9fr;align-items:center;gap:24px;padding:clamp(32px,6vw,80px) clamp(16px,4vw,48px);overflow:hidden}
.hero::before{content:"";position:absolute;inset:-50%;background:repeating-linear-gradient(135deg,transparent 0 46px,var(--line) 46px 47px);opacity:.55;animation:drift 40s linear infinite;pointer-events:none}
@keyframes drift{to{transform:translate(47px,47px)}}
.hero>*{position:relative}
.hero h1{font-size:clamp(40px,7vw,104px);max-width:11ch}
.hero p{max-width:46ch;color:var(--muted);font-size:clamp(16px,1.6vw,19px);margin:24px 0 32px}
.btns{display:flex;flex-wrap:wrap;gap:12px}
.btn{display:inline-flex;align-items:center;gap:8px;padding:14px 24px;border-radius:999px;border:1px solid var(--fg);background:transparent;font-weight:600;font-size:15px;cursor:pointer;text-decoration:none;transition:background .2s,color .2s,border-color .2s}
.btn:hover{background:var(--fg);color:var(--bg)}
.btn.solid{background:var(--fg);color:var(--bg)}
.btn.solid:hover{background:var(--blue);border-color:var(--blue);color:#fff}
.hero-logo{justify-self:end;width:min(100%,520px);aspect-ratio:1}
.hero-logo .logo{width:100%;height:100%}
@media (max-width:820px){.hero{grid-template-columns:1fr;min-height:0}.hero-logo{justify-self:center;width:min(70%,340px);order:-1}}

/* section heads */
.wrap{padding:clamp(48px,8vw,110px) clamp(16px,4vw,48px)}
.head{display:flex;flex-wrap:wrap;align-items:end;justify-content:space-between;gap:20px;margin-bottom:36px}
.head h2{font-size:clamp(32px,5vw,64px)}
.filters{display:flex;flex-wrap:wrap;gap:8px}
.filters button{border:1px solid var(--line);background:transparent;border-radius:999px;padding:8px 16px;font-size:14px;font-weight:500;cursor:pointer;transition:all .2s}
.filters button:hover{border-color:var(--fg)}
.filters button[aria-pressed="true"]{background:var(--fg);color:var(--bg);border-color:var(--fg)}

/* works grid */
.grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:clamp(24px,3vw,44px) clamp(14px,2vw,28px)}
.work{display:block;width:100%;text-align:left;background:none;border:0;padding:0;cursor:pointer}


.work.hide{display:none}
.art{position:relative;aspect-ratio:4/3;background:var(--bg2);overflow:hidden;border:1px solid var(--line)}

.art svg{position:absolute;inset:0;width:100%;height:100%;stroke:var(--fg);stroke-width:1.4;fill:none;stroke-linejoin:round;transition:transform .8s cubic-bezier(.2,.7,.2,1)}
.art .solid{fill:var(--bg2)}
.art .sun{fill:var(--blue);stroke:none}
.art .thin{stroke-width:.8;opacity:.6}
.art img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;transition:transform .8s cubic-bezier(.2,.7,.2,1)}
.work:hover .art svg,.work:hover .art img{transform:scale(1.06)}
.work .art::after{content:"Detayı gör";position:absolute;left:12px;bottom:12px;background:var(--fg);color:var(--bg);font-size:13px;font-weight:600;padding:6px 12px;opacity:0;transform:translateY(6px);transition:opacity .3s,transform .3s}
.work:hover .art::after,.work:focus-visible .art::after{opacity:1;transform:none}
.work .meta{display:flex;justify-content:space-between;align-items:flex-start;gap:12px;padding:14px 2px 16px;border-bottom:1px solid var(--line)}
.work h3{font-size:22px;font-weight:500}
.work .sub{display:block;color:var(--muted);font-size:14px;margin-top:2px}
@media (max-width:1000px){.grid{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media (max-width:560px){.grid{grid-template-columns:1fr}}


/* call band */
.band{margin:0 clamp(16px,4vw,48px) clamp(48px,8vw,100px);padding:clamp(28px,5vw,64px);background:var(--fg);color:var(--bg);display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;gap:24px}
.band h2{font-size:clamp(28px,4vw,52px);max-width:18ch}
.band .btn{border-color:var(--bg);color:var(--bg)}
.band .btn:hover{background:var(--bg);color:var(--fg)}

/* modal */
.modal{position:fixed;inset:0;z-index:50;display:none;align-items:center;justify-content:center;padding:20px;background:rgba(0,0,0,.6);backdrop-filter:blur(4px)}
.modal.open{display:flex;animation:fade .25s}
@keyframes fade{from{opacity:0}}
.sheet{position:relative;width:min(960px,100%);max-height:100%;overflow:auto;background:var(--bg);display:grid;grid-template-columns:1.2fr 1fr;animation:pop .35s cubic-bezier(.2,.8,.2,1)}
@keyframes pop{from{transform:translateY(24px) scale(.98);opacity:0}}
.sheet .art{border:0;height:100%;min-height:280px;aspect-ratio:auto}
.sheet .info{padding:clamp(20px,3vw,40px)}
.sheet h3{font-size:32px;font-weight:500;margin-bottom:12px}
.sheet p{color:var(--muted)}
.sheet dl{display:grid;grid-template-columns:auto 1fr;gap:8px 20px;margin:20px 0 0;font-size:14px}
.sheet dt{color:var(--muted)}.sheet dd{margin:0;font-weight:600}
.x{position:absolute;top:10px;right:10px;width:40px;height:40px;border-radius:50%;border:1px solid var(--line);background:var(--bg);cursor:pointer;font-size:18px;z-index:2}
[hidden]{display:none!important}
.gal{display:flex;flex-direction:column;background:var(--bg2);min-width:0}
.gal .main{display:block;width:100%;aspect-ratio:16/10;object-fit:contain;background:var(--bg2);cursor:zoom-in}
.gal .cap{margin:0;padding:8px 14px;font-size:13px;color:var(--muted);display:flex;justify-content:space-between;gap:12px}
.gal .thumbs{display:flex;gap:6px;padding:0 8px 8px}
.gal .thumbs button{flex:1;min-width:0;padding:0;border:2px solid transparent;background:none;cursor:pointer;aspect-ratio:4/3;overflow:hidden;opacity:.65;transition:opacity .2s,border-color .2s}
.gal .thumbs button:hover{opacity:1}
.gal .thumbs button[aria-pressed="true"]{border-color:var(--blue);opacity:1}
.gal .thumbs img{display:block;width:100%;height:100%;object-fit:cover}
.lb{position:fixed;inset:0;z-index:60;display:none;align-items:center;justify-content:center;padding:12px;background:rgba(0,0,0,.94);cursor:zoom-out}
.lb.open{display:flex;animation:fade .2s}
.lb img{max-width:100%;max-height:100%;object-fit:contain}
@media (max-width:720px){.sheet{grid-template-columns:1fr}.sheet .art{min-height:0;aspect-ratio:4/3;height:auto}}

/* status page */
.status{background-image:linear-gradient(var(--line) 1px,transparent 1px),linear-gradient(90deg,var(--line) 1px,transparent 1px);background-size:48px 48px;background-position:-1px -1px}
.status .inner{max-width:1120px;margin:0 auto}
.status h1{font-size:clamp(36px,6vw,80px);margin-bottom:12px}
.status .lead{color:var(--muted);max-width:52ch;margin:0 0 32px}
.query{display:flex;flex-wrap:wrap;gap:12px;align-items:end;background:var(--card);border:1px solid var(--line);padding:clamp(16px,3vw,28px)}
.field{display:flex;flex-direction:column;gap:6px;flex:1 1 140px}
.field label{font-size:13px;color:var(--muted);font-weight:600}
.field input{height:52px;padding:0 14px;border:1px solid var(--line);background:var(--bg);font-family:var(--display);font-size:24px;font-weight:500;width:100%;border-radius:0}
.field input:focus{border-color:var(--blue);outline:none;box-shadow:0 0 0 3px var(--blue-soft)}
.query .btn{height:52px;flex:0 0 auto}
.hint{width:100%;font-size:13px;color:var(--muted);margin:2px 0 0}
.hint button{background:none;border:0;padding:0;font-weight:700;text-decoration:underline;cursor:pointer}
.err{width:100%;color:#c62828;font-size:14px;font-weight:600;margin:0}
:root[data-theme="dark"] .err{color:#ff8a80}
@media (prefers-color-scheme: dark){:root:not([data-theme="light"]) .err{color:#ff8a80}}

.loader{display:none;align-items:center;gap:16px;margin-top:32px;color:var(--muted);font-weight:600}
.loader.on{display:flex}
.scan{width:44px;height:44px;position:relative;overflow:hidden}
.scan i{position:absolute;left:-10px;width:70px;height:7px;background:var(--fg);transform:rotate(-45deg);transform-origin:left center;animation:slide 1s ease-in-out infinite}
.scan i:nth-child(1){top:40px}.scan i:nth-child(2){top:56px;background:var(--gray);animation-delay:.15s}.scan i:nth-child(3){top:72px;animation-delay:.3s}
@keyframes slide{0%,100%{opacity:.2;transform:rotate(-45deg) translateX(-12px)}50%{opacity:1;transform:rotate(-45deg) translateX(8px)}}

.result{margin-top:32px}
.result .chips{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:16px}
.result .chips button{border:1px solid var(--line);background:var(--card);padding:8px 14px;border-radius:999px;font-size:14px;cursor:pointer}
.result .chips button[aria-pressed="true"]{background:var(--fg);color:var(--bg);border-color:var(--fg)}
.panel{display:grid;grid-template-columns:minmax(260px,380px) 1fr;background:var(--card);border:1px solid var(--line)}
@media (max-width:860px){.panel{grid-template-columns:1fr}}
.dial{padding:clamp(20px,3vw,36px);border-right:1px solid var(--line);display:flex;flex-direction:column;align-items:center;gap:20px}
@media (max-width:860px){.dial{border-right:0;border-bottom:1px solid var(--line)}}
.donut{position:relative;width:min(100%,300px);aspect-ratio:1}
.donut svg{width:100%;height:100%;transform:rotate(-90deg)}
.donut .track{stroke:var(--line2)}
.donut .prog{stroke:var(--blue);transition:stroke-dashoffset 1.8s cubic-bezier(.2,.7,.2,1)}
.donut .tick{stroke:var(--line);stroke-width:1}
.donut .mid{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center}
.donut .big{font-family:var(--display);font-weight:300;font-size:clamp(56px,9vw,76px);letter-spacing:-.04em;line-height:1}
.donut .big small{font-size:.45em;margin-left:2px}
.donut .cap{font-size:14px;color:var(--muted)}
.legend{width:100%;display:grid;grid-template-columns:1fr 1fr;gap:12px}
.legend div{border:1px solid var(--line);padding:12px 14px}
.legend b{display:block;font-family:var(--display);font-size:28px;font-weight:500;line-height:1.1}
.legend span{font-size:13px;color:var(--muted);display:flex;align-items:center;gap:8px}
.legend span::before{content:"";width:10px;height:10px;background:var(--blue)}
.legend div+div span::before{background:var(--line2)}
.detail{padding:clamp(20px,3vw,36px)}
.detail .ttl{display:flex;flex-wrap:wrap;justify-content:space-between;gap:12px;margin-bottom:6px}
.detail h2{font-size:clamp(26px,3.4vw,40px);font-weight:500}
.tag{display:inline-block;background:var(--fg);color:var(--bg);font-weight:700;font-size:14px;padding:6px 12px;height:fit-content}
.where{color:var(--muted);font-size:14px;margin:0 0 24px}
.stages{list-style:none;margin:0;padding:0}
.stage{display:grid;grid-template-columns:36px 1fr 48px;gap:14px;align-items:start;padding:14px 0;border-top:1px solid var(--line);opacity:0;transform:translateX(-12px);transition:opacity .5s,transform .5s}
.go .stage{opacity:1;transform:none;transition-delay:calc(var(--i)*110ms)}
.dot{width:32px;height:32px;border-radius:50%;border:1.5px solid var(--line2);display:grid;place-items:center;font-size:13px;font-weight:700;color:var(--muted)}
.done .dot{background:var(--fg);border-color:var(--fg);color:var(--bg)}
.active .dot{border-color:var(--blue);color:var(--blue);box-shadow:0 0 0 0 var(--blue-soft);animation:pulse 2s infinite}
@keyframes pulse{70%{box-shadow:0 0 0 9px transparent}100%{box-shadow:0 0 0 0 transparent}}
.srow{display:flex;flex-wrap:wrap;justify-content:space-between;gap:4px 12px;margin-bottom:8px}
.srow b{font-weight:600}
.state{font-size:13px;color:var(--muted)}
.active .state{color:var(--blue);font-weight:700}
.done .state{color:var(--fg);font-weight:600}
.bar{height:6px;background:var(--line2);overflow:hidden}
.bar i{display:block;height:100%;width:0;background:var(--fg);transition:width 1.4s cubic-bezier(.2,.7,.2,1);transition-delay:calc(var(--i)*110ms + 200ms)}
.active .bar i{background:var(--blue)}
.go .bar i{width:calc(var(--p)*1%)}
.spct{font-family:var(--display);font-weight:500;text-align:right;padding-top:4px}
.docs{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px}
.doc{display:inline-flex;align-items:center;gap:8px;padding:5px 12px 5px 5px;border:1px solid var(--line);font-size:13px;font-weight:600;text-decoration:none;transition:border-color .2s,background .2s}
.doc:hover{border-color:var(--fg);background:var(--bg2)}
.doc em{font-style:normal;font-size:11px;font-weight:700;letter-spacing:.04em;background:var(--fg);color:var(--bg);padding:3px 7px}
.doc.dwg em{background:var(--blue);color:#fff}
.pay{margin-top:28px;padding-top:24px;border-top:1px solid var(--line)}
.pay h3{font-size:26px;font-weight:500;margin-bottom:16px}
.sum{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:10px;margin-bottom:16px}
.sum div{border:1px solid var(--line);padding:12px 14px;min-width:0}
.sum span{display:block;font-size:13px;color:var(--muted)}
.sum b{display:block;font-family:var(--display);font-size:clamp(18px,2.2vw,23px);font-weight:500;line-height:1.25;overflow-wrap:anywhere}
.sum .paid b{color:var(--blue)}
.split{height:10px;background:var(--line2);overflow:hidden;margin-bottom:6px}
.split i{display:block;height:100%;width:0;background:var(--blue);transition:width 1.6s cubic-bezier(.2,.7,.2,1) .3s}
.go .split i{width:calc(var(--p)*1%)}
.splitcap{display:flex;justify-content:space-between;font-size:13px;color:var(--muted);margin-bottom:20px}
.items{list-style:none;margin:0;padding:0}
.pitem{padding:14px 0;border-top:1px solid var(--line);opacity:0;transform:translateY(8px);transition:opacity .5s,transform .5s}
.go .pitem{opacity:1;transform:none;transition-delay:calc(var(--i)*90ms + 400ms)}
.pitem .row{display:flex;flex-wrap:wrap;justify-content:space-between;gap:4px 12px;margin-bottom:8px}
.pitem .row b{font-weight:600}
.pitem .row span{font-size:13px;color:var(--muted)}
.pitem .bar i{background:var(--blue)}
.pm{display:flex;flex-wrap:wrap;gap:4px 18px;margin-top:8px;font-size:14px;color:var(--muted)}
.pm b{color:var(--fg);font-weight:600}
@media (max-width:560px){.sum{grid-template-columns:1fr}}
.note{margin-top:20px;padding:16px;background:var(--bg2);font-size:14px}
.note b{display:block;margin-bottom:4px}
.upd{margin-top:14px;font-size:13px;color:var(--muted)}
.empty{margin-top:32px;padding:28px;border:1px dashed var(--muted);background:var(--card)}
.empty h2{font-size:26px;font-weight:500;margin-bottom:8px}
.empty p{margin:0;color:var(--muted)}

/* footer */
footer{border-top:1px solid var(--line);padding:clamp(32px,5vw,56px) clamp(16px,4vw,48px);display:flex;flex-wrap:wrap;justify-content:space-between;gap:28px}
footer .brand .logo{width:44px;height:44px}
footer address{font-style:normal;color:var(--muted);font-size:15px;line-height:1.9}
footer address a{text-decoration:none;color:var(--fg);font-weight:600}
footer small{width:100%;color:var(--muted)}

@media (prefers-reduced-motion:reduce){
  *,*::before,*::after{animation-duration:.01ms!important;animation-iteration-count:1!important;transition-duration:.01ms!important;transition-delay:0ms!important}
  html{scroll-behavior:auto}
}
</style>
</head>
<body>

<header class="top">
  <a class="brand" href="#/" aria-label="Ana sayfa"><span data-logo></span><span class="word">HUDİYEN PROJECT</span></a>
  <nav aria-label="Ana menü">
    <a href="#/" data-nav="home">Çalışmalarımız</a>
    <a href="#/proje-durumu" data-nav="status" class="cta">Proje durumu sorgula</a>
  </nav>
</header>

<main>
<!-- SAYFA 1: ÇALIŞMALAR -->
<section id="page-home" class="page">
  <div class="hero">
    <div>
      <h1>Sade çizgiler, ölçülü mekânlar.</h1>
      <p>Konuttan ticari yapıya, restorasyondan iç mekâna kadar projeleri tasarım masasından iskâna kadar takip eden bir mimarlık ofisiyiz.</p>
      <div class="btns">
        <button class="btn solid" id="toWorks" type="button">Çalışmalarımızı gör</button>
        <a class="btn" href="#/proje-durumu">Proje durumunu sorgula</a>
      </div>
    </div>
    <div class="hero-logo" data-logo="draw" role="img" aria-label="Ofis logosu"></div>
  </div>

  <div class="wrap" id="works">
    <div class="head">
      <h2>Çalışmalarımız</h2>
      <div class="filters" role="group" aria-label="Proje türü">
        <button type="button" aria-pressed="true" data-f="all">Tümü</button>
        <button type="button" aria-pressed="false" data-f="Konut">Konut</button>
        <button type="button" aria-pressed="false" data-f="Ticari">Ticari</button>
        <button type="button" aria-pressed="false" data-f="Restorasyon">Restorasyon</button>
      </div>
    </div>
    <div class="grid" id="grid"></div>
  </div>

  <div class="band">
    <h2>Projeniz hangi aşamada, tek sorguda görün.</h2>
    <a class="btn" href="#/proje-durumu">Ada ve parsel ile sorgula</a>
  </div>
</section>

<!-- SAYFA 2: PROJE DURUMU -->
<section id="page-status" class="page">
  <div class="wrap status">
    <div class="inner">
      <h1>Proje durumu</h1>
      <p class="lead">Ada ve parsel numaranızı yazın, projenizin hangi aşamada olduğunu ve tamamlanmasına ne kadar kaldığını görün. Tamamlanan aşamaların belgelerini PDF ve DWG olarak indirebilir, ödeme durumunuzu da buradan takip edebilirsiniz.</p>

      <form class="query" id="q" novalidate>
        <div class="field"><label for="ada">Ada</label><input id="ada" inputmode="numeric" autocomplete="off" placeholder="604" maxlength="6"></div>
        <div class="field"><label for="parsel">Parsel</label><input id="parsel" inputmode="numeric" autocomplete="off" placeholder="44" maxlength="6"></div>
        <button class="btn solid" type="submit">Sorgula</button>
        <p class="hint">Örnek için <button type="button" id="demo">604 ada 44 parsel</button> deneyin.</p>
        <p class="err" id="err" role="alert" hidden></p>
      </form>

      <div class="loader" id="loader" aria-live="polite"><div class="scan"><i></i><i></i><i></i></div><span>Proje kaydı aranıyor</span></div>
      <div class="result" id="result" aria-live="polite"></div>
    </div>
  </div>
</section>
</main>

<footer>
  <div>
    <a class="brand" href="#/"><span data-logo></span><span class="word">HUDİYEN PROJECT</span></a>
  </div>
  <address>
    İstanbul, Türkiye<br>
    <a href="tel:+902120000000">0 (212) 000 00 00</a><br>
    <a href="mailto:info@ofisadiniz.com">info@ofisadiniz.com</a>
  </address>
  <small>© <span id="yr"></span> Hudiyen Project. Tüm hakları saklıdır.</small>
</footer>

<div class="modal" id="modal" role="dialog" aria-modal="true" aria-labelledby="mTitle">
  <div class="sheet">
    <button class="x" id="mClose" type="button" aria-label="Kapat">✕</button>
    <div class="art" id="mArt"></div>
    <div class="gal" id="mGal" hidden></div>
    <div class="info">
      <h3 id="mTitle"></h3>
      <p id="mDesc"></p>
      <dl id="mDl"></dl>
    </div>
  </div>
</div>

<div class="lb" id="lb" role="dialog" aria-label="Görseli büyüt"><img id="lbImg" alt=""></div>

<script>const IMGS={"persp": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "on": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "yan": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "mafta": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "saha": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "a_persp": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "a_on": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "a_kose": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "a_balkon": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "a_zemin": "data:...GÖRSEL_VERİSİ_ÇIKARILDI...", "a_afis": "data:...GÖRSEL_VERİSİ_ÇIKARILDI..."};</script>
<script>
/* ============ VERİLER (burayı kendi bilgilerinize göre düzenleyin) ============ */

// Proje durumu aşamaları ve ağırlıkları (toplam 100)
const STAGES = [
  {n:"Sözleşme ve ön görüşme", w:5},
  {n:"İmar durumu ve rölöve", w:10},
  {n:"Avan proje", w:20},
  {n:"Uygulama projesi (mimari)", w:20},
  {n:"Statik, mekanik ve elektrik projeleri", w:20},
  {n:"Belediye onayı ve ruhsat", w:15},
  {n:"Şantiye takibi ve iskân", w:10}
];

// Ödeme kalemleri. Projelerde pay:[[alınan, toplam], ...] bu sırayla yazılır (TL). Projede olmayan kalem için null yazın. Kalan tutar otomatik hesaplanır.
const PAY_ITEMS = ["Harita", "Mimari proje", "Elektrik projesi", "Mekanik projesi", "Statik proje", "Zemin etüdü", "Belediye harçları"];

// Her projede aşamaların ilerlemesi 0–100 arası yazılır (sırası STAGES ile aynı)
// docs: indirilebilir belgeler. Anahtar aşama numarasıdır (0'dan başlar: 0=Sözleşme, 1=İmar ve rölöve, 2=Avan proje ...).
// Belgeler sadece o aşama %100 olunca görünür. f: dosyanın index.html'e göre yolu (pdf veya dwg).
const PROJECTS = [
  {ada:604, parsel:44, mahalle:"Örnek Mah. / Kadıköy", title:"Yıldız Evleri, 6 katlı konut",
   stages:[100,100,100,70,40,0,0], updated:"2026-10-05",
   docs:{1:[{n:"Rölöve",f:"belgeler/604-44-k7x2m9/rolove.pdf"},{n:"Rölöve",f:"belgeler/604-44-k7x2m9/rolove.dwg"}],2:[{n:"Avan proje",f:"belgeler/604-44-k7x2m9/avan-proje.pdf"},{n:"Avan proje",f:"belgeler/604-44-k7x2m9/avan-proje.dwg"}]},
   pay:[[4000,4000],[60000,120000],[10000,25000],[0,25000],[20000,60000],[15000,15000],[30000,85000]],
   note:"Statik proje için mühendis ile koordinasyon sürüyor. Uygulama paftaları bu hafta tamamlanacak."},
  {ada:112, parsel:7, mahalle:"Bahçe Mah. / Üsküdar", title:"Bahçe Villa",
   stages:[100,100,100,100,100,100,35], updated:"2026-10-09",
   docs:{3:[{n:"Uygulama projesi",f:"belgeler/112-7-p4w8q1/uygulama.pdf"},{n:"Uygulama projesi",f:"belgeler/112-7-p4w8q1/uygulama.dwg"}],5:[{n:"Yapı ruhsatı",f:"belgeler/112-7-p4w8q1/ruhsat.pdf"}]},
   pay:[[3000,3000],[90000,90000],[20000,20000],[20000,20000],[45000,45000],[12000,12000],[40000,60000]],
   note:"Ruhsat alındı, kaba inşaat denetimleri devam ediyor."},
  {ada:2310, parsel:15, mahalle:"Çarşı Mah. / Beşiktaş", title:"Çarşı İş Merkezi",
   stages:[100,60,0,0,0,0,0], updated:"2026-10-02",
   pay:[[5000,8000],[30000,150000],[0,30000],[0,30000],[0,70000],null,[0,120000]],
   note:"Rölöve çalışması sürüyor, imar durumu belgesi bekleniyor."}
];

// Çalışmalarımız (kind: çizim tipi. Gerçek fotoğraf eklemek için bana gönderin)
const WORKS = [
  {title:"Eski TOKİ Dış Cephe Çalışması", type:"Konut", loc:"Eski TOKİ", year:2025, area:"4.800 m²", kind:"stepped",
   imgs:["persp","on","yan","saha","mafta"], caps:["Perspektif görünüm","Ön cephe","Yan cephe","Şantiye görünümü","Dış cephe malzeme maftası"],
   extra:[["Blok","2 blok"],["Durum","Devam ediyor"],["Ortak çalışma","Talha Çelebi"]],
   desc:"Eski TOKİ bölgesinde 2025 başında başlayan, 2 bloktan oluşan konut projesinin dış cephe çalışması. Açık bej traverten görünümlü kompozit paneller, dikey antrasit aksamlar, cam korkuluklu balkonlar ve alüminyum doğrama ile sade ve modern bir cephe kurgusu hazırlandı. Şantiyede cephe uygulamaları sürmektedir. Çalışma Talha Çelebi ile birlikte yürütülmektedir."},
  {title:"Artabel Kooperatifi Dış Cephe Çalışması", type:"Konut", loc:"Kimyalar Mevkii", year:2026, area:"9.000 m²", kind:"tower",
   imgs:["a_persp","a_on","a_kose","a_balkon","a_zemin","a_afis"], caps:["Perspektif görünüm","Ön cephe","Köşe ve ticari alan görünümü","Balkon ve cam korkuluk detayı","Zemin kat ticari alan detayı","Tanıtım afişi"],
   extra:[["Kooperatif","Artabel"],["Çalışma","Dış cephe"]],
   desc:"Kimyalar mevkiinde, 9.000 m² alan üzerindeki Artabel Kooperatifi için 2026 yılında hazırlanan dış cephe çalışması. Tuğla görünümlü yüzeyler, beyaz sıva ve koyu gri aksamlar, cam korkuluklu balkonlar ve zemin kattaki ticari alanlarla modern bir cephe kurgusu oluşturuldu."},
  {title:"Deniz Ofis Kulesi", type:"Ticari", loc:"Ataşehir", year:2024, area:"12.400 m²", kind:"tower", desc:"Dikey kütleli, esnek plan kurgusuna sahip ofis yapısı. Giydirme cephe sistemi ile enerji tasarrufu hedeflendi."},
  {title:"Sahil Villa", type:"Konut", loc:"Çeşme", year:2025, area:"380 m²", kind:"villa", desc:"Konsol çıkmalı üst kat ve geniş cam yüzeylerle bahçeye açılan, sade malzemeli tek aile konutu."},
  {title:"Çarşı Alışveriş Hanı", type:"Ticari", loc:"Beşiktaş", year:2023, area:"6.200 m²", kind:"commercial", desc:"Sürekli cephe düzeni ve geniş vitrin aksıyla cadde dokusuna uyum sağlayan ticari yapı."},
  {title:"Taş Konak Restorasyonu", type:"Restorasyon", loc:"Safranbolu", year:2024, area:"540 m²", kind:"heritage", desc:"Özgün taş ve ahşap detayları korunarak yeniden işlevlendirilen tescilli konak."}
];

/* ============ LOGO ============ */
function logoSVG(draw){
  return `<svg class="logo ${draw?'draw':''}" viewBox="0 0 1080 1080" role="img" aria-label="Logo">
  <g fill="none" stroke-linecap="butt">
    <circle class="p c1" pathLength="1" cx="540" cy="540" r="276.5" stroke="currentColor" stroke-width="27"/>
    <circle class="p c2" pathLength="1" cx="540" cy="540" r="251.5" stroke="var(--gray)" stroke-width="23"/>
    <circle class="p c3" pathLength="1" cx="540" cy="540" r="238" stroke="currentColor" stroke-width="4"/>
    <line class="p b1" pathLength="1" x1="868.5" y1="64.5" x2="-20" y2="953" stroke="currentColor" stroke-width="50"/>
    <line class="p b2" pathLength="1" x1="974.5" y1="105.5" x2="105" y2="975" stroke="var(--gray)" stroke-width="50"/>
    <line class="p b3" pathLength="1" x1="1100" y1="148" x2="210.5" y2="1037.5" stroke="currentColor" stroke-width="50"/>
  </g></svg>`;
}
document.querySelectorAll('[data-logo]').forEach(el=>{el.innerHTML = logoSVG(el.dataset.logo==='draw');});

/* ============ ÇİZİMLER ============ */
function art(kind){
  const r=(x,y,w,h,c='solid')=>`<rect class="${c}" x="${x}" y="${y}" width="${w}" height="${h}"/>`;
  const l=(a,b,c,d,k='')=>`<line class="${k}" x1="${a}" y1="${b}" x2="${c}" y2="${d}"/>`;
  let s='<circle class="sun" cx="342" cy="52" r="14"/>';
  const G=252;
  if(kind==='tower'){
    s+=r(100,222,200,30)+r(140,40,120,182)+l(200,40,200,16);
    for(let i=0;i<9;i++)for(let j=0;j<4;j++)s+=r(150+j*27,50+i*19,17,10,'thin');
    for(let j=0;j<7;j++)s+=r(108+j*27,230,19,14,'thin');
  }else if(kind==='villa'){
    s+=r(60,176,190,76)+r(120,120,210,56)+l(112,120,338,120)+l(60,176,250,176);
    s+=r(76,192,96,60,'thin')+l(108,192,108,252,'thin')+l(140,192,140,252,'thin');
    s+=r(136,134,170,28,'thin')+l(192,134,192,162,'thin')+l(248,134,248,162,'thin');
    s+=r(196,206,36,46,'thin');
    s+=`<circle cx="352" cy="214" r="22"/>`+l(352,236,352,252);
  }else if(kind==='stepped'){
    s+=r(60,160,280,92)+r(100,110,200,50)+r(140,62,120,48);
    [[60,160,280,92],[100,110,200,50],[140,62,120,48]].forEach(([x,y,w,h])=>{
      for(let yy=y+16;yy<y+h;yy+=16)s+=l(x,yy,x+w,yy,'thin');
      for(let xx=x+20;xx<x+w;xx+=26)s+=r(xx,y+4,14,9,'thin');
    });
    for(let xx=80;xx<330;xx+=38)s+=r(xx,224,20,28,'thin');
  }else if(kind==='commercial'){
    s+=r(50,108,300,144);
    for(let x=62;x<350;x+=16)s+=l(x,108,x,236,'thin');
    for(let y=144;y<236;y+=36)s+=l(50,y,350,y,'thin');
    s+=r(120,232,160,8)+r(150,236,100,16,'thin')+l(200,236,200,252,'thin');
    s+=l(50,108,350,108)+l(40,100,360,100);
  }else if(kind==='heritage'){
    s+=r(90,134,220,118)+`<polygon class="solid" points="76,134 200,70 324,134"/>`+r(256,84,16,36);
    [118,160,224,266].forEach(x=>{s+=`<path class="thin" d="M${x},192 v-30 a12,12 0 0 1 24,0 v30 z"/>`;});
    s+=`<path d="M184,252 v-44 a16,16 0 0 1 32,0 v44 z"/>`+l(120,222,150,222,'thin')+l(250,222,280,222,'thin');
    s+=`<circle cx="200" cy="108" r="9" class="thin"/>`;
  }else{ // mixed
    s+=r(50,118,140,134)+r(214,64,136,188)+r(190,170,24,12);
    for(let y=130;y<252;y+=12)s+=l(50,y,190,y,'thin');
    for(let i=0;i<10;i++)for(let j=0;j<4;j++)s+=r(224+j*30,76+i*17,18,9,'thin');
    s+=r(70,226,40,26,'thin');
  }
  s+=l(14,G,386,G);
  for(let x=24;x<386;x+=14)s+=l(x,G,x-8,G+8,'thin');
  return `<svg viewBox="0 0 400 300" preserveAspectRatio="xMidYMid meet" aria-hidden="true">${s}</svg>`;
}

/* ============ ÇALIŞMALAR ============ */
const grid=document.getElementById('grid');
grid.innerHTML=WORKS.map((w,i)=>`
  <button class="work" type="button" data-i="${i}" data-t="${w.type}" aria-label="${w.title} detayını aç">
    <div class="art">${w.imgs?`<img src="${src(w.imgs[0])}" alt="${w.title}" loading="lazy">`:art(w.kind)}</div>
    <div class="meta"><div><h3>${w.title}</h3><span class="sub">${w.type}, ${w.loc}</span></div><span class="sub">${w.year}</span></div>
  </button>`).join('');

document.querySelectorAll('.filters button').forEach(b=>b.addEventListener('click',()=>{
  document.querySelectorAll('.filters button').forEach(x=>x.setAttribute('aria-pressed',x===b));
  const f=b.dataset.f;
  grid.querySelectorAll('.work').forEach(w=>w.classList.toggle('hide',f!=='all'&&w.dataset.t!==f));
}));

const modal=document.getElementById('modal');let lastFocus=null;
// Görsel: IMGS içindeki anahtar ya da doğrudan dosya yolu (örn. gorseller/proje1.jpg)
function src(k){return (typeof IMGS!=='undefined'&&IMGS[k])||k;}
let curWork=null;
function renderGal(w,k){
  const g=document.getElementById('mGal');
  g.innerHTML=`<img class="main" src="${src(w.imgs[k])}" alt="${w.caps[k]}" data-zoom>
    <p class="cap"><span>${w.caps[k]}</span><span>Büyütmek için dokunun</span></p>
    <div class="thumbs">${w.imgs.map((m,j)=>`<button type="button" data-k="${j}" aria-pressed="${j===k}" aria-label="${w.caps[j]}"><img src="${src(m)}" alt=""></button>`).join('')}</div>`;
}
function openWork(i){
  const w=WORKS[i];lastFocus=document.activeElement;curWork=w;
  const mArt=document.getElementById('mArt'),gal=document.getElementById('mGal');
  if(w.imgs){mArt.hidden=true;gal.hidden=false;renderGal(w,0);}
  else{gal.hidden=true;mArt.hidden=false;mArt.innerHTML=art(w.kind);}
  document.getElementById('mTitle').textContent=w.title;
  document.getElementById('mDesc').textContent=w.desc;
  const rows=[["Tür",w.type],["Konum",w.loc],["Yıl",w.year],["Alan",w.area]].concat(w.extra||[]);
  document.getElementById('mDl').innerHTML=rows.map(r=>`<dt>${r[0]}</dt><dd>${r[1]}</dd>`).join('');
  modal.classList.add('open');document.getElementById('mClose').focus();
}
function closeWork(){modal.classList.remove('open');if(lastFocus)lastFocus.focus();}
grid.addEventListener('click',e=>{const b=e.target.closest('.work');if(b)openWork(+b.dataset.i);});
document.getElementById('mClose').addEventListener('click',closeWork);
modal.addEventListener('click',e=>{if(e.target===modal)closeWork();});
document.getElementById('mGal').addEventListener('click',e=>{
  const t=e.target.closest('.thumbs button');
  if(t&&curWork){renderGal(curWork,+t.dataset.k);return;}
  const m=e.target.closest('[data-zoom]');
  if(m){document.getElementById('lbImg').src=m.src;document.getElementById('lbImg').alt=m.alt;document.getElementById('lb').classList.add('open');}
});
document.getElementById('lb').addEventListener('click',()=>document.getElementById('lb').classList.remove('open'));
document.addEventListener('keydown',e=>{
  if(e.key!=='Escape')return;
  const lb=document.getElementById('lb');
  if(lb.classList.contains('open'))lb.classList.remove('open');
  else if(modal.classList.contains('open'))closeWork();
});
document.getElementById('toWorks').addEventListener('click',()=>document.getElementById('works').scrollIntoView({behavior:'smooth'}));

/* ============ PROJE DURUMU ============ */
const reduce=matchMedia('(prefers-reduced-motion: reduce)').matches;
const $=id=>document.getElementById(id);
const MONTHS=["Ocak","Şubat","Mart","Nisan","Mayıs","Haziran","Temmuz","Ağustos","Eylül","Ekim","Kasım","Aralık"];
const fmtDate=s=>{const d=new Date(s+'T00:00:00');return `${d.getDate()} ${MONTHS[d.getMonth()]} ${d.getFullYear()}`;};
const total=p=>Math.round(STAGES.reduce((a,s,i)=>a+s.w*p.stages[i]/100,0));

function countTo(el,to,dur=1800){
  if(reduce){el.textContent=to;return;}
  const t0=performance.now();
  (function f(t){const k=Math.min(1,(t-t0)/dur),e=1-Math.pow(1-k,3);el.textContent=Math.round(to*e);if(k<1)requestAnimationFrame(f);})(t0);
}

function ticks(){
  let s='';
  for(let i=0;i<60;i++){
    const a=i*6*Math.PI/180,r1=i%5===0?70:74,r2=80;
    s+=`<line class="tick" x1="${100+Math.cos(a)*r1}" y1="${100+Math.sin(a)*r1}" x2="${100+Math.cos(a)*r2}" y2="${100+Math.sin(a)*r2}"/>`;
  }
  return s;
}

const TL=n=>n.toLocaleString('tr-TR')+' ₺';
function moneyTo(el,to,dur=1800){
  if(reduce){el.textContent=TL(to);return;}
  const t0=performance.now();
  (function f(t){const k=Math.min(1,(t-t0)/dur),e=1-Math.pow(1-k,3);el.textContent=TL(Math.round(to*e));if(k<1)requestAnimationFrame(f);})(t0);
}

function payHtml(p){
  if(!p.pay)return '';
  const rows=PAY_ITEMS.map((n,i)=>({n,v:p.pay[i]})).filter(r=>r.v);
  if(!rows.length)return '';
  const tot=rows.reduce((a,r)=>a+r.v[1],0),paid=rows.reduce((a,r)=>a+r.v[0],0),left=tot-paid;
  const pc=tot?Math.round(paid/tot*100):0;
  const items=rows.map((r,i)=>{
    const a=r.v[0],t=r.v[1],l=Math.max(0,t-a),q=t?Math.round(a/t*100):0;
    const st=l<=0?'Tamamı ödendi':a>0?'Kısmi ödeme':'Ödeme bekleniyor';
    return `<li class="pitem" style="--i:${i}"><div class="row"><b>${r.n}</b><span>${st}</span></div>
      <div class="bar" role="progressbar" aria-valuenow="${q}" aria-valuemin="0" aria-valuemax="100" aria-label="${r.n} ödeme durumu"><i style="--p:${q}"></i></div>
      <div class="pm"><span>Ödenen <b>${TL(a)}</b></span><span>Kalan <b>${TL(l)}</b></span><span>Toplam <b>${TL(t)}</b></span></div></li>`;
  }).join('');
  return `<div class="pay"><h3>Ödemeler</h3>
    <div class="sum"><div><span>Toplam bedel</span><b data-money="${tot}">0 ₺</b></div><div class="paid"><span>Alınan ödeme</span><b data-money="${paid}">0 ₺</b></div><div><span>Kalan ödeme</span><b data-money="${left}">0 ₺</b></div></div>
    <div class="split" role="progressbar" aria-valuenow="${pc}" aria-valuemin="0" aria-valuemax="100" aria-label="Ödenen oran"><i style="--p:${pc}"></i></div>
    <div class="splitcap"><span>%${pc} ödendi</span><span>%${100-pc} kalan</span></div>
    <ul class="items">${items}</ul></div>`;
}

function docsHtml(p,i,v){
  const list=(p.docs&&p.docs[i])||[];
  if(v<100||!list.length)return '';
  return '<div class="docs">'+list.map(d=>{
    const ext=(d.f.split('.').pop()||'').toLowerCase();
    return `<a class="doc ${ext}" href="${encodeURI(d.f)}" download><em>${ext.toUpperCase()}</em>${d.n}</a>`;
  }).join('')+'</div>';
}

function panel(p){
  const done=total(p),left=100-done,C=2*Math.PI*88;
  const rows=STAGES.map((s,i)=>{
    const v=p.stages[i],cls=v>=100?'done':v>0?'active':'wait';
    const st=v>=100?'Tamamlandı':v>0?'Devam ediyor':'Bekliyor';
    return `<li class="stage ${cls}" style="--i:${i}">
      <span class="dot">${v>=100?'✓':i+1}</span>
      <div><div class="srow"><b>${s.n}</b><span class="state">${st}</span></div>
      <div class="bar" role="progressbar" aria-valuenow="${v}" aria-valuemin="0" aria-valuemax="100" aria-label="${s.n}"><i style="--p:${v}"></i></div>${docsHtml(p,i,v)}</div>
      <span class="spct">%${v}</span></li>`;
  }).join('');
  return `<div class="panel" id="panel">
    <div class="dial">
      <div class="donut">
        <svg viewBox="0 0 200 200" aria-hidden="true">
          ${ticks()}
          <circle class="track" cx="100" cy="100" r="88" fill="none" stroke-width="14"/>
          <circle class="prog" cx="100" cy="100" r="88" fill="none" stroke-width="14" stroke-dasharray="${C}" stroke-dashoffset="${C}" data-c="${C}" data-p="${done}"/>
        </svg>
        <div class="mid"><div class="big">%<span data-count="${done}">0</span></div><div class="cap">tamamlandı</div></div>
      </div>
      <div class="legend">
        <div><span>Tamamlanan</span><b>%<i data-count="${done}" style="font-style:normal">0</i></b></div>
        <div><span>Kalan</span><b>%<i data-count="${left}" style="font-style:normal">0</i></b></div>
      </div>
    </div>
    <div class="detail">
      <div class="ttl"><h2>${p.title}</h2><span class="tag">${p.ada} ada, ${p.parsel} parsel</span></div>
      <p class="where">${p.mahalle}</p>
      <ol class="stages">${rows}</ol>
      ${payHtml(p)}
      ${p.note?`<div class="note"><b>Ofis notu</b>${p.note}</div>`:''}
      <p class="upd">Son güncelleme: ${fmtDate(p.updated)}</p>
    </div>
  </div>`;
}

function animatePanel(){
  const pn=$('panel');if(!pn)return;
  const pr=pn.querySelector('.prog');
  requestAnimationFrame(()=>requestAnimationFrame(()=>{
    pn.classList.add('go');
    const C=+pr.dataset.c,p=+pr.dataset.p;
    pr.style.strokeDashoffset=C*(1-p/100);
    pn.querySelectorAll('[data-count]').forEach(el=>countTo(el,+el.dataset.count));
    pn.querySelectorAll('[data-money]').forEach(el=>moneyTo(el,+el.dataset.money));
  }));
}

function show(list,idx=0){
  const out=$('result');
  let chips='';
  if(list.length>1){
    chips='<div class="chips" role="group" aria-label="Eşleşen projeler">'+list.map((p,i)=>`<button type="button" data-k="${i}" aria-pressed="${i===idx}">${p.mahalle}</button>`).join('')+'</div>';
  }
  out.innerHTML=chips+panel(list[idx]);
  out.querySelectorAll('.chips button').forEach(b=>b.addEventListener('click',()=>show(list,+b.dataset.k)));
  animatePanel();
}

let timer=null;
function search(ada,parsel){
  const err=$('err');err.hidden=true;
  if(!ada||!parsel){err.textContent='Ada ve parsel numarasını sayı olarak yazın.';err.hidden=false;return;}
  $('result').innerHTML='';
  $('loader').classList.add('on');
  clearTimeout(timer);
  timer=setTimeout(()=>{
    $('loader').classList.remove('on');
    const list=PROJECTS.filter(p=>p.ada===ada&&p.parsel===parsel);
    if(!list.length){
      $('result').innerHTML=`<div class="empty"><h2>${ada} ada ${parsel} parsel için kayıt bulunamadı</h2><p>Numaraları kontrol edip tekrar deneyin. Sorun sürerse ofisimizi arayarak projenizin durumunu öğrenebilirsiniz.</p></div>`;
      return;
    }
    show(list);
  },reduce?0:1000);
}
$('q').addEventListener('submit',e=>{
  e.preventDefault();
  search(parseInt($('ada').value,10),parseInt($('parsel').value,10));
});
['ada','parsel'].forEach(id=>$(id).addEventListener('input',e=>{e.target.value=e.target.value.replace(/\D/g,'');}));
$('demo').addEventListener('click',()=>{$('ada').value=604;$('parsel').value=44;search(604,44);});

/* ============ SAYFA YÖNLENDİRME ============ */
function route(){
  const status=location.hash.startsWith('#/proje-durumu');
  $('page-home').classList.toggle('active',!status);
  $('page-status').classList.toggle('active',status);
  document.querySelectorAll('[data-nav]').forEach(a=>a.classList.toggle('on',a.dataset.nav===(status?'status':'home')&&a.dataset.nav!=='status'));
  document.title=status?'Proje Durumu | Hudiyen Project':'Çalışmalarımız | Hudiyen Project';
  window.scrollTo(0,0);
  if(status)setTimeout(()=>$('ada').focus({preventScroll:true}),50);
  else{ // logo çizimini yeniden başlat
    const h=document.querySelector('.hero-logo');h.innerHTML=logoSVG(true);
  }
}
addEventListener('hashchange',route);
$('yr').textContent=new Date().getFullYear();
route();
</script>
</body>
</html>
