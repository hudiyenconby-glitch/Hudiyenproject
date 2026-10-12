<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>HUDİYEN · Mimarlık Ofisi</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,500&family=Schibsted+Grotesk:wght@400;600;800&display=swap" rel="stylesheet">
<script>document.documentElement.className="js";try{if(sessionStorage.getItem("hdy"))document.documentElement.className+=" seen";else sessionStorage.setItem("hdy","1")}catch(e){}</script>
<style>
/* ===== LOGO YAZI TİPİ: 'CheckFor' dosyanız varsa aşağıdaki @font-face satırının yorumunu kaldırıp url'yi yazın =====
@font-face{font-family:'CheckFor';src:url('BURAYA-FONT-DOSYASI-URL.woff2') format('woff2');font-display:swap}
*/
:root{--ff-logo:'CheckFor','Playfair Display','Iowan Old Style',Georgia,serif;--bg:#f4f0e9;--ink:#1c1b18;--mute:#7a7467;--line:#ddd5c7;--acc:#2f4a3a;--stone:#e6dfd2;--l1:#1c1b18;--l2:#6b665b;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
*{box-sizing:border-box}html{scroll-behavior:smooth;scroll-padding-top:80px}
body{margin:0;background:var(--bg);color:var(--ink);font-family:'Schibsted Grotesk',system-ui,'Segoe UI',sans-serif;line-height:1.6;overflow-x:hidden}
a{color:inherit}
.serif{font-family:'Playfair Display','Iowan Old Style',Georgia,serif}
/* preloader */
.pre{position:fixed;inset:0;z-index:100;background:#1c1b18;color:#f4f0e9;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:28px;animation:lift 1s cubic-bezier(.7,0,.2,1) 3.2s both}
.seen .pre{display:none}
@keyframes lift{to{transform:translateY(-100%);visibility:hidden}}
.pl-logo{width:min(34vw,160px);height:auto}
.pl-logo circle,.pl-logo line{fill:none;stroke:#f4f0e9}
.pl-logo .r2,.pl-logo .b2{stroke:#9a958b}
.pl-logo .b{stroke-width:49.5}
.pl-logo circle{stroke-dasharray:1;stroke-dashoffset:0;animation:draw 1.4s cubic-bezier(.6,0,.2,1) both}
.pl-logo .r2{animation-delay:.15s}.pl-logo .r3{animation-delay:.3s}
.pl-logo .b{animation:slide 1.1s cubic-bezier(.2,.8,.2,1) both}
.pl-logo .b1{animation-delay:.7s}.pl-logo .b2{animation-delay:.85s}.pl-logo .b3{animation-delay:1s}
.plw{font-family:var(--ff-logo);font-size:clamp(30px,8vw,54px);font-weight:700;letter-spacing:.32em;padding-left:.32em;line-height:1}
.plw span{display:inline-block;animation:rise .6s cubic-bezier(.2,.8,.2,1) both;animation-delay:calc(1.5s + var(--i)*.07s)}
.pltag{font-family:'Playfair Display',Georgia,serif;font-style:italic;color:#bdb6a8;animation:fade .8s 2.2s both}
@keyframes draw{from{stroke-dashoffset:1}to{stroke-dashoffset:0}}
@keyframes slide{from{transform:translate(-460px,460px);opacity:0}to{transform:none;opacity:1}}
@keyframes rise{from{opacity:0;transform:translateY(.5em)}to{opacity:1;transform:none}}
@keyframes fade{from{opacity:0}to{opacity:1}}
/* header */
.hd{position:fixed;top:0;left:0;right:0;z-index:50;display:flex;align-items:center;justify-content:space-between;gap:14px;padding:calc(14px + env(safe-area-inset-top,0px)) 24px 14px;background:color-mix(in srgb,var(--bg) 84%,transparent);backdrop-filter:blur(10px);-webkit-backdrop-filter:blur(10px);border-bottom:1px solid transparent;transition:border-color .3s}
.hd.sc{border-bottom-color:var(--line)}
.hd-logo{display:flex;align-items:center;gap:12px;text-decoration:none}
.hd-logo svg{width:36px;height:36px}
.hd-logo b{font-family:var(--ff-logo);font-size:19px;letter-spacing:.3em;font-weight:700}
.hd nav{display:flex;align-items:center;gap:26px}
.hd nav a{text-decoration:none;font-size:14px;font-weight:600;color:var(--mute);transition:color .2s}
.hd nav a:hover{color:var(--ink)}
.hd nav a.cur{color:var(--ink)}
.pill{display:inline-flex;align-items:center;gap:8px;border:1.5px solid var(--ink);border-radius:999px;padding:9px 18px;font-size:14px;font-weight:700;text-decoration:none;color:var(--ink);background:transparent;transition:background .25s,color .25s}
.pill:hover{background:var(--ink);color:var(--bg)}
.pill:focus-visible,.hd a:focus-visible,.card:focus-visible,.chip:focus-visible,.x:focus-visible{outline:3px solid var(--acc);outline-offset:3px}
.hd nav .pill{color:var(--ink)}.hd nav .pill:hover{color:var(--bg)}
@media(max-width:820px){.hd nav a:not(.pill){display:none}.hd{padding-left:16px;padding-right:16px}.hd-logo b{font-size:16px}}
/* hero */
.hero{position:relative;min-height:100vh;min-height:100svh;display:flex;flex-direction:column;justify-content:flex-end;padding:120px 24px 64px;overflow:hidden}
.st{position:absolute;width:46px;height:190vmax;top:-45vmax;background:var(--ink);transform:rotate(45deg);opacity:.06;animation:drift 22s ease-in-out infinite alternate}
.st:nth-child(1){left:42%}.st:nth-child(2){left:56%;opacity:.045;animation-delay:-6s}.st:nth-child(3){left:76%;animation-delay:-12s}
@keyframes drift{to{transform:rotate(45deg) translateY(60px)}}
.hero>*:not(.st){position:relative;max-width:1180px;width:100%;margin-left:auto;margin-right:auto}
.eyebrow{font-size:13px;color:var(--mute);font-weight:600;margin-bottom:18px}
.hero h1{font-family:'Playfair Display','Iowan Old Style',Georgia,serif;font-weight:600;font-size:clamp(40px,8.2vw,112px);line-height:1.02;letter-spacing:-.02em;margin:0 0 28px;max-width:14ch}
.hero h1 em{font-weight:500}
.hero p{max-width:46ch;color:var(--mute);font-size:18px;margin:0 auto 30px 0}
.ri{animation:rise 1s cubic-bezier(.2,.8,.2,1) both;animation-delay:calc(3.5s + var(--d,0)*.14s)}
.seen .ri{animation-delay:calc(.1s + var(--d,0)*.14s)}
.cue{display:flex;gap:14px;align-items:center;flex-wrap:wrap}
.btn{display:inline-flex;align-items:center;gap:8px;background:var(--ink);color:var(--bg);border-radius:999px;padding:13px 26px;font-weight:700;text-decoration:none;font-size:15px;transition:transform .2s,background .2s}
.btn:hover{background:var(--acc);transform:translateY(-2px)}
/* sections */
section{padding:110px 24px}
.in{max-width:1180px;margin:0 auto}
.num{font-size:13px;font-weight:700;color:var(--mute);letter-spacing:.08em;display:block;margin-bottom:14px}
h2{font-family:'Playfair Display','Iowan Old Style',Georgia,serif;font-weight:600;font-size:clamp(30px,5vw,58px);line-height:1.08;letter-spacing:-.015em;margin:0 0 36px;max-width:18ch}
.js .rv{opacity:0;transform:translateY(28px);transition:opacity .9s cubic-bezier(.2,.8,.2,1),transform .9s cubic-bezier(.2,.8,.2,1)}
.js .rv.on{opacity:1;transform:none}
/* works */
.chips{display:flex;gap:8px;flex-wrap:wrap;margin:0 0 30px}
.chip{font:inherit;font-size:14px;font-weight:600;border:1.5px solid var(--line);background:transparent;color:var(--ink);padding:7px 16px;border-radius:999px;cursor:pointer;transition:all .2s}
.chip:hover{border-color:var(--ink)}
.chip[aria-pressed=true]{background:var(--ink);color:var(--bg);border-color:var(--ink)}
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:26px}
@media(max-width:960px){.grid{grid-template-columns:repeat(2,1fr)}}
@media(max-width:600px){.grid{grid-template-columns:1fr}section{padding:80px 18px}}
.card{all:unset;box-sizing:border-box;cursor:pointer;display:block}
.thumb{position:relative;aspect-ratio:4/3;overflow:hidden;border-radius:6px;background:var(--stone)}
.thumb svg,.thumb img{width:100%;height:100%;object-fit:cover;display:block;transition:transform 1.1s cubic-bezier(.2,.8,.2,1)}
.card:hover .thumb svg,.card:hover .thumb img{transform:scale(1.07)}
.thumb .more{position:absolute;left:14px;bottom:14px;background:var(--bg);color:var(--ink);font-size:13px;font-weight:700;border-radius:999px;padding:6px 14px;opacity:0;transform:translateY(8px);transition:all .35s}
.card:hover .more,.card:focus-visible .more{opacity:1;transform:none}
.cm{display:flex;justify-content:space-between;gap:12px;align-items:baseline;padding-top:14px}
.cm h3{font-family:'Playfair Display',Georgia,serif;font-weight:600;font-size:21px;margin:0;line-height:1.2}
.cm span{font-size:13px;color:var(--mute);white-space:nowrap}
.cs{font-size:14px;color:var(--mute);margin:2px 0 0}
/* approach */
.app{display:grid;grid-template-columns:repeat(3,1fr);gap:0;border-top:1px solid var(--line)}
@media(max-width:820px){.app{grid-template-columns:1fr}}
.app div{padding:32px 28px 36px 0;border-bottom:1px solid var(--line)}
.app b{font-size:13px;color:var(--mute)}
.app h3{font-family:'Playfair Display',Georgia,serif;font-size:26px;font-weight:600;margin:10px 0 10px}
.app p{margin:0;color:var(--mute);max-width:34ch}
/* cta */
.cta{background:var(--ink);color:var(--bg);text-align:center}
.cta h2{margin-left:auto;margin-right:auto;max-width:20ch}
.cta p{color:#bdb6a8;max-width:46ch;margin:-12px auto 30px}
.cta .btn{background:var(--bg);color:var(--ink)}.cta .btn:hover{background:#fff}
/* contact */
.ct{display:grid;grid-template-columns:1fr 1fr;gap:30px}
@media(max-width:720px){.ct{grid-template-columns:1fr}}
.ct h4{font-size:13px;color:var(--mute);margin:0 0 6px;font-weight:600}
.ct a,.ct p{font-family:'Playfair Display',Georgia,serif;font-size:24px;margin:0 0 22px;display:block;text-decoration:none;line-height:1.3}
.ct a:hover{color:var(--acc)}
footer{padding:26px 24px calc(34px + env(safe-area-inset-bottom,0px));border-top:1px solid var(--line);color:var(--mute);font-size:13px;display:flex;justify-content:space-between;gap:10px;flex-wrap:wrap;max-width:1180px;margin:0 auto}
/* modal */
.md{position:fixed;inset:0;z-index:80;background:rgba(20,19,16,.6);display:none;align-items:center;justify-content:center;padding:18px}
.md.on{display:flex;animation:fade .3s}
.mb{background:var(--bg);border-radius:10px;max-width:920px;width:100%;max-height:92vh;overflow:auto;display:grid;grid-template-columns:1.1fr 1fr;animation:rise .45s cubic-bezier(.2,.8,.2,1)}
@media(max-width:720px){.mb{grid-template-columns:1fr}}
.mb .thumb{border-radius:0;height:100%;min-height:260px;aspect-ratio:auto}
.mi{padding:30px 28px;position:relative}
.mi h3{font-family:'Playfair Display',Georgia,serif;font-size:30px;font-weight:600;margin:0 0 6px;line-height:1.15;padding-right:36px}
.mi dl{display:grid;grid-template-columns:auto 1fr;gap:6px 18px;margin:18px 0;font-size:14px}
.mi dt{color:var(--mute)}.mi dd{margin:0;font-weight:600}
.x{position:absolute;top:14px;right:14px;width:38px;height:38px;border-radius:50%;border:1.5px solid var(--line);background:var(--bg);font-size:20px;cursor:pointer;color:var(--ink)}
.prog{position:fixed;top:0;left:0;height:3px;width:100%;background:var(--acc);transform:scaleX(0);transform-origin:0 50%;z-index:60}
.cv{position:fixed;inset:0;z-index:90;background:#1c1b18;transform:translateY(100%);transition:transform .6s cubic-bezier(.7,0,.2,1);pointer-events:none}.cv.on{transform:none}
.w{display:inline-block;overflow:hidden;vertical-align:top;padding-bottom:.14em;margin-bottom:-.14em}
.w>b{display:inline-block;font-weight:inherit}
.js .w>b{transform:translateY(108%);transition:transform 1.05s cubic-bezier(.2,.8,.2,1);transition-delay:calc(var(--k)*.075s)}
.js .sp.on .w>b,.js .sp.go .w>b{transform:none}
.mq{overflow:hidden;border-block:1px solid var(--line);padding:22px 0;white-space:nowrap}
.mt{display:inline-flex;animation:mq 38s linear infinite}
.mt span{font-family:'Playfair Display',Georgia,serif;font-style:italic;font-size:clamp(28px,5vw,56px);line-height:1.2}
.mt span::after{content:"•";font-style:normal;color:var(--mute);margin:0 44px}
@keyframes mq{to{transform:translateX(-50%)}}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;border-top:1px solid var(--line);padding-top:34px}
.stats b{display:block;font-family:'Playfair Display',Georgia,serif;font-size:clamp(42px,7vw,88px);font-weight:600;line-height:1;font-variant-numeric:lining-nums}
.stats span{color:var(--mute);font-size:14px}
.js .card .thumb{clip-path:inset(0 0 100% 0);transition:clip-path 1.3s cubic-bezier(.2,.8,.2,1)}
.js .card.on .thumb{clip-path:inset(0)}
.thumb svg,.thumb img{transform:translateY(var(--py,0px)) scale(1.14);transition:transform .5s ease-out}
.card:hover .thumb svg,.card:hover .thumb img{transform:translateY(var(--py,0px)) scale(1.21)}
.btn,.pill{will-change:transform}
@media (prefers-reduced-motion:reduce){.w>b{transform:none!important}.js .card .thumb{clip-path:none}}
@media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important;scroll-behavior:auto!important}.pre{display:none}.js .rv{opacity:1;transform:none}}
</style>
</head>
<body>
<div class="prog" id="prog"></div><div class="cv" id="cv"></div>

<div class="pre" aria-hidden="true">
  <svg class="pl-logo" viewBox="0 0 1080 1080"><defs><clipPath id="cp"><rect width="1080" height="1080"/></clipPath></defs>
  <g clip-path="url(#cp)"><g transform="rotate(-90 540 540)">
    <circle class="r1" cx="540" cy="540" r="277" stroke-width="26" pathLength="1"/>
    <circle class="r2" cx="540" cy="540" r="252" stroke-width="24" pathLength="1"/>
    <circle class="r3" cx="540" cy="540" r="240" stroke-width="3" pathLength="1"/></g>
    <line class="b b1" x1="-150" y1="1083" x2="868.5" y2="64.5"/>
    <line class="b b2" x1="105.5" y1="974.5" x2="974.5" y2="105.5"/>
    <line class="b b3" x1="211" y1="1037.5" x2="1200" y2="48.5"/></g></svg>
  <div class="plw"><span style="--i:0">H</span><span style="--i:1">U</span><span style="--i:2">D</span><span style="--i:3">İ</span><span style="--i:4">Y</span><span style="--i:5">E</span><span style="--i:6">N</span></div>
  <div class="pltag">Mimarlık Ofisi</div>
</div>

<svg width="0" height="0" style="position:absolute" aria-hidden="true"><defs>
  <symbol id="mk" viewBox="0 0 1080 1080"><clipPath id="cq"><rect width="1080" height="1080"/></clipPath>
  <g clip-path="url(#cq)" fill="none"><circle cx="540" cy="540" r="277" stroke="var(--l1)" stroke-width="26"/><circle cx="540" cy="540" r="252" stroke="var(--l2)" stroke-width="24"/><circle cx="540" cy="540" r="240" stroke="var(--l1)" stroke-width="3"/>
  <line x1="-150" y1="1083" x2="868.5" y2="64.5" stroke="var(--l1)" stroke-width="49.5"/><line x1="105.5" y1="974.5" x2="974.5" y2="105.5" stroke="var(--l2)" stroke-width="49.5"/><line x1="211" y1="1037.5" x2="1200" y2="48.5" stroke="var(--l1)" stroke-width="49.5"/></g></symbol>
</defs></svg>

<header class="hd" id="hd">
  <a class="hd-logo" href="#top" aria-label="HUDİYEN"><svg aria-hidden="true"><use href="#mk"/></svg><b>HUDİYEN</b></a>
  <nav>
    <a href="#works">Çalışmalarımız</a>
    <a href="#approach">Yaklaşım</a>
    <a href="#contact">İletişim</a>
    <a class="pill" data-url="durum" target="_top" href="hudiyen-proje-durumu.html">Proje Durumu Sorgula <span aria-hidden="true">→</span></a>
  </nav>
</header>

<main id="top">
<div class="hero">
  <i class="st"></i><i class="st"></i><i class="st"></i>
  <div class="eyebrow ri" style="--d:0">Mimarlık · İç Mimari</div>
  <h1 class="sp" id="h1">Yaşamak için <em>tasarlanmış</em> mekânlar.</h1>
  <p class="ri" style="--d:2">Fikirden ruhsata, uygulama projesinden teslime; her aşamayı titizlikle yürütüyoruz.</p>
  <div class="cue ri" style="--d:3"><a class="btn" href="#works">Çalışmalarımızı inceleyin</a><a class="pill" data-url="durum" target="_top" href="hudiyen-proje-durumu.html">Proje Durumu Sorgula →</a></div>
</div>

<div class="mq" aria-hidden="true"><div class="mt" id="mq2"></div></div>
<section style="padding-bottom:0"><div class="in"><div class="stats" id="stats"></div></div></section>

<section id="works"><div class="in">
  <span class="num rv">01</span>
  <h2 class="rv sp">Seçilmiş çalışmalar</h2>
  <div class="chips rv" id="chips"></div>
  <div class="grid" id="grid"></div>
</div></section>

<section id="approach" style="padding-top:20px"><div class="in">
  <span class="num rv">02</span>
  <h2 class="rv sp">Her aşamada yanınızdayız</h2>
  <div class="app">
    <div class="rv"><b>01</b><h3>Tasarım</h3><p>Arsanın ve ihtiyacın okunmasıyla başlayan, mimari ve iç mekân tasarım süreci.</p></div>
    <div class="rv"><b>02</b><h3>Ruhsat ve dokümantasyon</h3><p>Proje çizimleri, statik inceleme ve ruhsat süreçlerinin eksiksiz takibi.</p></div>
    <div class="rv"><b>03</b><h3>Uygulama, metraj ve keşif</h3><p>Uygulama projeleri, metraj ve keşif çalışmalarıyla şantiyeye hazır paket.</p></div>
  </div>
</div></section>

<section class="cta"><div class="in">
  <h2 class="rv sp">Projeniz hangi aşamada?</h2>
  <p class="rv">Ada ve parsel numaranızı yazın; ilerleme yüzdesini ve aşamalara ait dosyaları görün.</p>
  <a class="btn rv" data-url="durum" target="_top" href="hudiyen-proje-durumu.html">Proje Durumu Sorgula →</a>
</div></section>

<section id="contact"><div class="in">
  <span class="num rv">03</span>
  <h2 class="rv sp">İletişim</h2>
  <div class="ct rv">
    <div><h4>Telefon</h4><a id="tel" href="#">—</a><h4>E-posta</h4><a id="mail" href="#">—</a></div>
    <div><h4>Adres</h4><p id="adr">—</p></div>
  </div>
</div></section>
</main>

<footer><span>© 2026 HUDİYEN. Tüm hakları saklıdır.</span><span>Mimarlık Ofisi</span></footer>

<div class="md" id="md" role="dialog" aria-modal="true" aria-labelledby="mt"><div class="mb" id="mb"></div></div>

<script>
/* ====== BURAYI DÜZENLEYİN ====== */
var URLS={durum:"hudiyen-proje-durumu.html"};   /* Wix'te TAM adres yazın: "https://www.siteniz.com/proje-durumu" (kısa "/proje-durumu" embed içinde ÇALIŞMAZ) */
var OFIS={tel:"0 (5XX) XXX XX XX",mail:"info@alanadiniz.com",adres:"Ofis adresinizi buraya yazın, Edirne"};
/* img: Wix Medya'dan kopyaladığınız görsel adresi. Boş bırakılırsa çizim görünür. */
var WORKS=[
 {ad:"Örnek Konut Projesi A",tur:"Konut",yer:"Edirne",yil:2025,alan:"1.240 m²",durum:"Yapım aşamasında",img:"",ac:"Örnek açıklama: ruhsat, uygulama projesi ve metraj dahil tüm aşamalar ofisimizce yürütülmüştür."},
 {ad:"Öğrenci Yurdu İç Mekân",tur:"İç Mekân",yer:"Edirne",yil:2026,alan:"3.800 m²",durum:"Uygulama",img:"",ac:"Örnek açıklama: odalar, ortak alanlar ve etüt salonlarının iç mekân tasarımı."},
 {ad:"Örnek Villa B",tur:"Konut",yer:"Edirne",yil:2024,alan:"420 m²",durum:"Tamamlandı",img:"",ac:"Örnek açıklama: doğal malzemeli, bahçe ile bütünleşen tek aile konutu."},
 {ad:"Örnek Ofis Tadilatı",tur:"Ticari",yer:"Edirne",yil:2024,alan:"260 m²",durum:"Tamamlandı",img:"",ac:"Örnek açıklama: çalışma alanlarının yeniden kurgulanması ve aydınlatma tasarımı."},
 {ad:"Örnek Okul Binası",tur:"Eğitim",yer:"Edirne",yil:2025,alan:"2.150 m²",durum:"Tamamlandı",img:"",ac:"Örnek açıklama: sınıf, laboratuvar ve ortak alan kurgusu."},
 {ad:"Örnek Daire İç Mimarisi",tur:"İç Mekân",yer:"Edirne",yil:2026,alan:"145 m²",durum:"Yapım aşamasında",img:"",ac:"Örnek açıklama: mobilya, mutfak ve aydınlatma detaylarıyla anahtar teslim iç mekân."}
];
/* Rakamlar: ÖRNEK değerlerdir, kendi rakamlarınızla değiştirin */
var STATS=[{n:120,s:"+",t:"Tamamlanan proje"},{n:15,s:"",t:"Yıllık deneyim"},{n:40,s:"+",t:"Ruhsat dosyası"}];
/* ================================= */

var $=function(i){return document.getElementById(i)};
document.querySelectorAll("[data-url]").forEach(function(a){a.href=URLS[a.dataset.url]});
$("tel").textContent=OFIS.tel;$("tel").href="tel:"+OFIS.tel.replace(/[^+\d]/g,"");
$("mail").textContent=OFIS.mail;$("mail").href="mailto:"+OFIS.mail;$("adr").textContent=OFIS.adres;

var TONES=["#cfc5b3","#b9ad98","#a39682","#8d826f"],
 BG=[["#f1e8d8","#d8ccb6"],["#e6ece3","#c6d3c5"],["#efe5dc","#d5c2b2"],["#e9e6df","#cfc9bd"]];
function art(i){
  var s=i*97+13;function r(){s=(s*9301+49297)%233280;return s/233280}
  var bg=BG[i%4],o='<svg viewBox="0 0 400 300" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Örnek çizim"><defs><linearGradient id="g'+i+'" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="'+bg[0]+'"/><stop offset="1" stop-color="'+bg[1]+'"/></linearGradient></defs><rect width="400" height="300" fill="url(#g'+i+')"/>';
  o+='<circle cx="'+(60+r()*280)+'" cy="'+(50+r()*30)+'" r="'+(18+r()*14)+'" fill="#fff" opacity=".55"/>';
  var n=3+Math.floor(r()*2),x=30;
  for(var k=0;k<n;k++){var w=70+r()*50,h=90+r()*110,y=240-h;
    o+='<rect x="'+x+'" y="'+y+'" width="'+w+'" height="'+h+'" fill="'+TONES[k%4]+'"/>';
    for(var l=y+16;l<236;l+=20)o+='<line x1="'+(x+8)+'" y1="'+l+'" x2="'+(x+w-8)+'" y2="'+l+'" stroke="#fff" stroke-opacity=".35" stroke-width="2"/>';
    x+=w+8+r()*10}
  return o+'<rect y="240" width="400" height="60" fill="#1c1b18" opacity=".12"/><line x1="0" y1="240" x2="400" y2="240" stroke="#1c1b18" stroke-opacity=".5"/></svg>';
}
function thumb(w,i){return w.img?'<img src="'+w.img+'" alt="'+w.ad+'" loading="lazy">':art(i)}

var cat="Hepsi";
function chips(){
  var t=["Hepsi"];WORKS.forEach(function(w){if(t.indexOf(w.tur)<0)t.push(w.tur)});
  $("chips").innerHTML=t.map(function(c){return '<button class="chip" aria-pressed="'+(c===cat)+'" data-c="'+c+'">'+c+'</button>'}).join("");
  document.querySelectorAll(".chip").forEach(function(b){b.onclick=function(){cat=b.dataset.c;chips();grid()}});
}
function grid(){
  var h="";
  WORKS.forEach(function(w,i){if(cat!=="Hepsi"&&w.tur!==cat)return;
    h+='<button class="card rv" data-i="'+i+'" aria-label="'+w.ad+' detayını aç"><div class="thumb">'+thumb(w,i)+'<span class="more">İncele</span></div><div class="cm"><h3>'+w.ad+'</h3><span>'+w.yil+'</span></div><p class="cs">'+w.tur+' · '+w.yer+'</p></button>'});
  $("grid").innerHTML=h;
  document.querySelectorAll(".card").forEach(function(c,k){c.onclick=function(){open(+c.dataset.i)};setTimeout(function(){c.classList.add("on")},60*k)});
}
function open(i){
  var w=WORKS[i];
  $("mb").innerHTML='<div class="thumb">'+thumb(w,i)+'</div><div class="mi"><button class="x" id="x" aria-label="Kapat">×</button><h3 id="mt">'+w.ad+'</h3><span class="cs">'+w.tur+'</span><dl><dt>Konum</dt><dd>'+w.yer+'</dd><dt>Yıl</dt><dd>'+w.yil+'</dd><dt>Alan</dt><dd>'+w.alan+'</dd><dt>Durum</dt><dd>'+w.durum+'</dd></dl><p>'+w.ac+'</p></div>';
  $("md").classList.add("on");$("x").focus();$("x").onclick=close;
}
function close(){$("md").classList.remove("on")}
$("md").onclick=function(e){if(e.target===$("md"))close()};
document.addEventListener("keydown",function(e){if(e.key==="Escape")close()});
chips();grid();

var io=("IntersectionObserver" in window)?new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting){e.target.classList.add("on");io.unobserve(e.target)}})},{threshold:.12}):null;
document.querySelectorAll(".rv:not(.card)").forEach(function(e){io?io.observe(e):e.classList.add("on")});
addEventListener("scroll",function(){$("hd").classList.toggle("sc",scrollY>40)},{passive:true});

/* ---- animasyonlar ---- */
function split(el){var k=0;(function walk(n){Array.from(n.childNodes).forEach(function(c){if(c.nodeType===3){var f=document.createDocumentFragment();c.textContent.split(/(\s+)/).forEach(function(t){if(!t)return;if(/^\s+$/.test(t)){f.appendChild(document.createTextNode(" "));return}var w=document.createElement("span");w.className="w";var b=document.createElement("b");b.textContent=t;b.style.setProperty("--k",k++);w.appendChild(b);f.appendChild(w)});n.replaceChild(f,c)}else if(c.nodeType===1)walk(c)})})(el)}
document.querySelectorAll(".sp").forEach(split);
setTimeout(function(){$("h1").classList.add("go")},document.documentElement.classList.contains("seen")?150:3600);

var WD=["Mimarlık","İç Mimari","Ruhsat","Metraj","Keşif","Uygulama Projesi"],mh=WD.map(function(w){return "<span>"+w+"</span>"}).join("");
$("mq2").innerHTML=mh+mh+mh+mh;

$("stats").innerHTML=STATS.map(function(s){return '<div class="stat rv"><b data-to="'+s.n+'" data-s="'+s.s+'">0</b><span>'+s.t+'</span></div>'}).join("");
function count(b){if(b.dataset.d)return;b.dataset.d=1;var to=+b.dataset.to,sf=b.dataset.s,t0=null;function f(t){if(!t0)t0=t;var k=Math.min((t-t0)/1700,1),e=1-Math.pow(1-k,3);b.textContent=Math.round(to*e)+(k>=1?sf:"");if(k<1)requestAnimationFrame(f)}requestAnimationFrame(f)}
var io2=("IntersectionObserver" in window)?new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting){e.target.classList.add("on");count(e.target.querySelector("b"));io2.unobserve(e.target)}})},{threshold:.4}):null;
document.querySelectorAll(".stat").forEach(function(e){if(io2)io2.observe(e);else{e.classList.add("on");var b=e.querySelector("b");b.textContent=b.dataset.to+b.dataset.s}});

var tk=false;
function frame(){tk=false;
  var h=document.documentElement.scrollHeight-innerHeight;$("prog").style.transform="scaleX("+(h>0?scrollY/h:0)+")";
  document.querySelectorAll(".card .thumb").forEach(function(t){var r=t.getBoundingClientRect();if(r.bottom<0||r.top>innerHeight)return;var d=(r.top+r.height/2-innerHeight/2)*-.05;t.style.setProperty("--py",Math.max(-18,Math.min(18,d))+"px")});
}
function req(){if(!tk){tk=true;requestAnimationFrame(frame)}}
addEventListener("scroll",req,{passive:true});addEventListener("resize",req);setTimeout(req,300);

/* sayfa geçiş animasyonu */
document.querySelectorAll("[data-url]").forEach(function(a){a.addEventListener("click",function(e){
  if(e.ctrlKey||e.metaKey||e.shiftKey)return;e.preventDefault();$("cv").classList.add("on");
  setTimeout(function(){try{window.open(a.href,"_top")}catch(x){location.href=a.href}setTimeout(function(){$("cv").classList.remove("on")},1500)},620)})});

/* güvenlik: perde takılırsa kaldır */
setTimeout(function(){var p=document.querySelector(".pre");if(p)p.style.display="none"},4800);

/* güvenlik: kaydırma/boyut ne olursa olsun içerik görünür olsun */
function reveal(){document.querySelectorAll(".rv:not(.on),.stat:not(.on)").forEach(function(e){var r=e.getBoundingClientRect();if(r.top<innerHeight*.95&&r.bottom>0){e.classList.add("on");if(e.classList.contains("stat"))count(e.querySelector("b"))}})}
addEventListener("scroll",reveal,{passive:true});addEventListener("resize",reveal);addEventListener("load",reveal);
var rt=setInterval(reveal,400);setTimeout(function(){clearInterval(rt)},15000);reveal();
</script>
</body>
</html>
