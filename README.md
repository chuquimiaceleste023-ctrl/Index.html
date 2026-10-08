# Index.html
Página web de fresas con crema
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Fresas con crema</title>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Nunito:wght@400;600;800&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#ffe9ef; --card:#fff7f9; --ink:#6b1f36; --soft:#a9556e; --rose:#f7a8bd; --berry:#e5365f; --cream:#fff3dc;
  box-sizing:border-box;
  padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){--bg:#3a1523;--card:#4d1d2f;--ink:#ffe3ea;--soft:#f3b3c5;--rose:#c9647f;--berry:#ff6b8e;--cream:#5a2a3b}
}
:root[data-theme="dark"]{--bg:#3a1523;--card:#4d1d2f;--ink:#ffe3ea;--soft:#f3b3c5;--rose:#c9647f;--berry:#ff6b8e;--cream:#5a2a3b}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font-family:Nunito,system-ui,sans-serif;line-height:1.6}
header{text-align:center;padding:40px 20px 12px}
h1{font-family:Pacifico,cursive;font-weight:400;font-size:clamp(2.4rem,9vw,4.2rem);margin:0;color:var(--berry)}
header p{max-width:34em;margin:10px auto 0;color:var(--soft);font-size:1.05rem}
.carousel{max-width:760px;margin:24px auto;padding:0 16px;position:relative}
.viewport{overflow:hidden;border-radius:28px;background:var(--card);box-shadow:0 10px 30px rgba(229,54,95,.18)}
.track{display:flex;transition:transform .5s ease}
.slide{min-width:100%;margin:0}
.slide svg{display:block;width:100%;height:auto}
.slide figcaption{padding:16px 22px 22px;text-align:center}
.slide h2{margin:0 0 4px;font-family:Pacifico,cursive;font-weight:400;font-size:1.5rem;color:var(--berry)}
.slide p{margin:0;color:var(--soft)}
.btn{position:absolute;top:38%;width:44px;height:44px;border:0;border-radius:50%;background:var(--card);color:var(--berry);font-size:1.5rem;font-weight:800;cursor:pointer;box-shadow:0 4px 12px rgba(229,54,95,.3)}
.btn:hover{background:var(--berry);color:#fff}
.btn:focus-visible,.dot:focus-visible{outline:3px solid var(--berry);outline-offset:2px}
.prev{left:2px}.next{right:2px}
.dots{display:flex;justify-content:center;gap:10px;margin-top:16px}
.dot{width:12px;height:12px;border-radius:50%;border:0;background:var(--rose);opacity:.55;cursor:pointer;padding:0}
.dot[aria-current="true"]{background:var(--berry);opacity:1;transform:scale(1.25)}
.receta{max-width:760px;margin:28px auto 48px;padding:0 16px;display:grid;gap:16px;grid-template-columns:repeat(auto-fit,minmax(260px,1fr))}
.receta section{background:var(--card);border-radius:22px;padding:20px 24px}
.receta h3{margin:0 0 8px;font-family:Pacifico,cursive;font-weight:400;color:var(--berry)}
.receta ul,.receta ol{margin:0;padding-left:1.2em}
footer{text-align:center;padding:0 20px 36px;color:var(--soft)}
nav{display:flex;flex-wrap:wrap;justify-content:center;gap:8px;margin-top:18px}
nav a{padding:8px 16px;border-radius:999px;background:var(--card);color:var(--berry);font-weight:800;text-decoration:none;font-size:.95rem}
nav a:hover,nav a:focus-visible{background:var(--berry);color:#fff;outline:none}
.sec{max-width:760px;margin:0 auto 44px;padding:0 16px}
.sec>h2{font-family:Pacifico,cursive;font-weight:400;font-size:1.9rem;color:var(--berry);text-align:center;margin:0 0 16px}
.grid{display:grid;gap:16px;grid-template-columns:repeat(auto-fit,minmax(210px,1fr))}
.box{background:var(--card);border-radius:22px;padding:20px 22px}
.box h3{margin:0 0 6px;color:var(--ink);font-size:1.1rem}
.box p{margin:0;color:var(--soft)}
.ico{font-size:2rem;display:block;margin-bottom:6px}
.mv .box{border-top:6px solid var(--rose)}
.contact a{color:var(--berry);font-weight:800;text-decoration:none}
.contact a:hover{text-decoration:underline}
.hours{margin:0;padding:0;list-style:none;color:var(--soft)}
.hours li{display:flex;justify-content:space-between;gap:12px;padding:3px 0;border-bottom:1px dashed var(--rose)}
@media (prefers-reduced-motion:reduce){.track{transition:none}}
</style>
</head>
<body>
<header>
  <h1>Fresas con crema</h1>
  <p>El postre más rosadito y dulce: fresas frescas, crema suave y nada más.</p>
  <nav aria-label="Secciones">
    <a href="#como">Cómo lo hacemos</a><a href="#mision">Misión y visión</a><a href="#contacto">Contacto</a>
  </nav>
</header>

<div class="carousel" role="region" aria-roledescription="carrusel" aria-label="Galería de fresas con crema">
  <div class="viewport">
    <div class="track" id="track">

      <figure class="slide">
        <svg viewBox="0 0 600 380" role="img" aria-label="Copa de fresas con crema">
          <rect width="600" height="380" fill="#ffd3df"/>
          <circle cx="90" cy="70" r="40" fill="#ffe9ef" opacity=".7"/><circle cx="520" cy="110" r="55" fill="#ffe9ef" opacity=".6"/>
          <path d="M190 150h220l-30 150q-6 28-34 28h-92q-28 0-34-28z" fill="#fff" opacity=".85" stroke="#f7a8bd" stroke-width="4"/>
          <path d="M200 190h200l-20 110q-6 24-30 24h-100q-24 0-30-24z" fill="#fff3dc"/>
          <rect x="260" y="326" width="80" height="12" rx="6" fill="#f7a8bd"/><rect x="225" y="338" width="150" height="14" rx="7" fill="#f7a8bd"/>
          <path d="M195 160q20-45 60-30q20-30 45-12q25-18 45 12q40-15 60 30z" fill="#fffdf6"/>
          <g id="f1"><path d="M0-34C-36-34-42 4-14 34Q0 46 14 34C42 4 36-34 0-34z" fill="#e5365f"/><path d="M-14-34l14-14 14 14-14 6z" fill="#4caf6a"/><g fill="#ffd3a3"><circle cx="-10" cy="-8" r="2"/><circle cx="10" cy="-8" r="2"/><circle cx="0" cy="6" r="2"/><circle cx="-12" cy="14" r="2"/><circle cx="12" cy="14" r="2"/></g></g>
          <use href="#f1" transform="translate(255 118) scale(.9)"/><use href="#f1" transform="translate(345 112) scale(1)"/><use href="#f1" transform="translate(300 92) scale(1.1) rotate(-8)"/>
        </svg>
        <figcaption><h2>La copa clásica</h2><p>Fresas maduras sobre una nube de crema.</p></figcaption>
      </figure>

      <figure class="slide">
        <svg viewBox="0 0 600 380" role="img" aria-label="Fresas frescas">
          <rect width="600" height="380" fill="#ffc2d4"/>
          <circle cx="300" cy="200" r="170" fill="#ffd9e3"/>
          <g id="f2"><path d="M0-60C-62-60-74 8-24 60Q0 80 24 60C74 8 62-60 0-60z" fill="#e5365f"/><path d="M-26-60l26-28 26 28-26 10z" fill="#4caf6a"/><g fill="#ffe0b0"><circle cx="-20" cy="-26" r="3"/><circle cx="20" cy="-26" r="3"/><circle cx="0" cy="-8" r="3"/><circle cx="-26" cy="12" r="3"/><circle cx="26" cy="12" r="3"/><circle cx="0" cy="34" r="3"/></g></g>
          <use href="#f2" transform="translate(190 210) rotate(-15)"/><use href="#f2" transform="translate(410 215) rotate(14) scale(.95)"/><use href="#f2" transform="translate(300 170) scale(1.15)"/>
        </svg>
        <figcaption><h2>Fresas frescas</h2><p>Lavadas, cortadas y listas para endulzar el día.</p></figcaption>
      </figure>

      <figure class="slide">
        <svg viewBox="0 0 600 380" role="img" aria-label="Tazón de crema batida">
          <rect width="600" height="380" fill="#ffe3d0"/>
          <circle cx="480" cy="80" r="50" fill="#fff3dc"/>
          <path d="M130 190h340q0 120-170 120T130 190z" fill="#fff" stroke="#f7a8bd" stroke-width="5"/>
          <ellipse cx="300" cy="190" rx="170" ry="26" fill="#fff3dc"/>
          <path d="M190 190q10-50 55-40q10-45 55-30q45-15 55 30q45-10 55 40z" fill="#fffdf6" stroke="#f3e2c4" stroke-width="3"/>
          <path d="M270 120q30-50 60 0q-30 20-60 0z" fill="#fffdf6" stroke="#f3e2c4" stroke-width="3"/>
          <rect x="250" y="306" width="100" height="14" rx="7" fill="#f7a8bd"/>
        </svg>
        <figcaption><h2>Crema batida</h2><p>Suave, ligera y con un toque de vainilla.</p></figcaption>
      </figure>

      <figure class="slide">
        <svg viewBox="0 0 600 380" role="img" aria-label="Fresa bañada en crema">
          <rect width="600" height="380" fill="#f9c4d4"/>
          <circle cx="110" cy="300" r="70" fill="#ffd9e3"/><circle cx="520" cy="90" r="60" fill="#ffd9e3"/>
          <g transform="translate(300 215)"><path d="M0-110C-115-110-135 15-45 112Q0 150 45 112C135 15 115-110 0-110z" fill="#e5365f"/>
            <path d="M-110-50Q-60-30-30-70Q0-30 40-70Q80-30 112-50Q90 20 60 10Q30 60 0 20Q-30 60-60 10Q-95 20-110-50z" fill="#fffdf6"/>
            <path d="M-45-112l45-48 45 48-45 18z" fill="#4caf6a"/>
            <g fill="#ffe0b0"><circle cx="-40" cy="10" r="4"/><circle cx="40" cy="12" r="4"/><circle cx="0" cy="45" r="4"/><circle cx="-30" cy="75" r="4"/><circle cx="32" cy="75" r="4"/></g></g>
          <g fill="#fff" opacity=".8"><circle cx="480" cy="250" r="8"/><circle cx="130" cy="140" r="6"/><circle cx="505" cy="180" r="5"/></g>
        </svg>
        <figcaption><h2>Un bocado perfecto</h2><p>Dulce, fresquita y con cremita por encima.</p></figcaption>
      </figure>

    </div>
  </div>
  <button class="btn prev" id="prev" aria-label="Imagen anterior">‹</button>
  <button class="btn next" id="next" aria-label="Imagen siguiente">›</button>
  <div class="dots" id="dots"></div>
</div>

<main class="receta">
  <section>
    <h3>Ingredientes</h3>
    <ul>
      <li>500 g de fresas</li>
      <li>250 ml de crema para batir</li>
      <li>3 cucharadas de azúcar glas</li>
      <li>1 cucharadita de vainilla</li>
    </ul>
  </section>
  <section>
    <h3>Preparación</h3>
    <ol>
      <li>Lava y corta las fresas.</li>
      <li>Bate la crema con el azúcar y la vainilla hasta que esté suave.</li>
      <li>Sirve las fresas y cúbrelas con la crema.</li>
      <li>Enfría 15 minutos y disfruta.</li>
    </ol>
  </section>
</main>
<section class="sec" id="como">
  <h2>Cómo lo hacemos</h2>
  <div class="grid">
    <div class="box"><span class="ico">🍓</span><h3>1. Elegimos las mejores</h3><p>Fresas frescas, maduras y bien rojas, seleccionadas una por una.</p></div>
    <div class="box"><span class="ico">🥄</span><h3>2. Batimos la crema</h3><p>Crema suave con vainilla y poca azúcar, hecha en el momento.</p></div>
    <div class="box"><span class="ico">🎀</span><h3>3. Servimos con cariño</h3><p>Cada copa se arma al pedido y se entrega bien fría.</p></div>
  </div>
</section>

<section class="sec mv" id="mision">
  <h2>Misión y visión</h2>
  <div class="grid">
    <div class="box"><span class="ico">💗</span><h3>Misión</h3><p>Endulzar el día de nuestros clientes con fresas con crema frescas, deliciosas y preparadas con ingredientes de calidad.</p></div>
    <div class="box"><span class="ico">🌟</span><h3>Visión</h3><p>Ser el lugar favorito para disfrutar un postre de fresas con crema, reconocido por su sabor, su frescura y su atención cercana.</p></div>
  </div>
</section>

<section class="sec contact" id="contacto">
  <h2>Contáctanos</h2>
  <div class="grid">
    <div class="box"><span class="ico">📍</span><h3>Dónde estamos</h3><p>Calle de las Fresas #123<br>Tu ciudad</p></div>
    <div class="box"><span class="ico">📞</span><h3>Escríbenos</h3><p>WhatsApp: <a href="tel:+00000000000">+00 000 000 000</a><br>Correo: <a href="mailto:hola@fresasconcrema.com">hola@fresasconcrema.com</a></p></div>
    <div class="box"><span class="ico">🕒</span><h3>Horarios</h3>
      <ul class="hours"><li><span>Lun a vie</span><span>10:00 – 20:00</span></li><li><span>Sábado</span><span>10:00 – 22:00</span></li><li><span>Domingo</span><span>12:00 – 18:00</span></li></ul></div>
  </div>
  <div class="box" style="margin-top:16px;text-align:center"><h3>Síguenos</h3><p><a href="#contacto">Instagram</a> · <a href="#contacto">Facebook</a> · <a href="#contacto">TikTok</a></p></div>
</section>

<footer>Hecho con cariño y mucha crema 🍓<br>© 2026 Fresas con crema</footer>

<script>
(function(){
  var track=document.getElementById('track'),n=track.children.length,i=0,timer;
  var dots=document.getElementById('dots');
  for(var k=0;k<n;k++){(function(k){var b=document.createElement('button');b.className='dot';b.setAttribute('aria-label','Ir a la imagen '+(k+1));b.onclick=function(){go(k,true)};dots.appendChild(b)})(k)}
  function go(x,user){
    i=(x+n)%n;track.style.transform='translateX('+(-i*100)+'%)';
    Array.prototype.forEach.call(dots.children,function(d,j){d.setAttribute('aria-current',j===i)});
    if(user)restart();
  }
  function restart(){clearInterval(timer);if(!window.matchMedia('(prefers-reduced-motion: reduce)').matches)timer=setInterval(function(){go(i+1)},4500)}
  document.getElementById('prev').onclick=function(){go(i-1,true)};
  document.getElementById('next').onclick=function(){go(i+1,true)};
  document.addEventListener('keydown',function(e){if(e.key==='ArrowLeft')go(i-1,true);if(e.key==='ArrowRight')go(i+1,true)});
  var sx=null;track.addEventListener('touchstart',function(e){sx=e.touches[0].clientX},{passive:true});
  track.addEventListener('touchend',function(e){if(sx===null)return;var d=e.changedTouches[0].clientX-sx;if(Math.abs(d)>40)go(i+(d<0?1:-1),true);sx=null});
  go(0);restart();
})();
</script>
</body>
</html>

