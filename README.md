<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For Amrika ❤️</title>

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Patrick+Hand&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    :root{
      --pink:#ff5a7a;
      --soft:#ffd6df;
      --glass:rgba(255,255,255,.22);
    }

    *{box-sizing:border-box}

    body{
      margin:0;
      font-family:'Poppins',system-ui,-apple-system,Segoe UI,Roboto;
      background: radial-gradient(1200px 600px at 10% -10%, #ffd6df, transparent),
                  radial-gradient(1000px 600px at 90% 10%, #ffc3d1, transparent),
                  linear-gradient(135deg,#ff9a9e,#fad0c4);
      color:#fff;
      overflow-x:hidden;
    }

    /* pages */
    .page{display:none;min-height:100vh;padding:90px 20px 40px;}
    .page.active{display:flex;flex-direction:column;align-items:center;gap:24px;animation:fade .9s ease}
    @keyframes fade{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:none}}

    /* header */
    .hero{
      position:fixed;inset:0 0 auto 0;height:70px;
      display:flex;align-items:center;justify-content:center;
      backdrop-filter: blur(10px);
      background: linear-gradient(to bottom, rgba(255,255,255,.35), rgba(255,255,255,.05));
      border-bottom:1px solid rgba(255,255,255,.25);
      z-index:9;
    }
    .hero strong{font-family:'Playfair Display',serif;font-size:1.2rem}

    h1{font-family:'Playfair Display',serif;font-size:3.1rem;margin:0}
    h2{font-weight:300;margin:0}

    /* glass card */
    .card{
      background:var(--glass);
      backdrop-filter: blur(16px);
      border-radius:28px;
      padding:32px 28px;
      max-width:760px;
      box-shadow:0 30px 60px rgba(0,0,0,.25), inset 0 1px 0 rgba(255,255,255,.35);
    }
    .card p{font-size:1.05rem;line-height:1.75}

    /* buttons */
    .buttons{display:flex;flex-wrap:wrap;gap:14px;justify-content:center}
    button{
      appearance:none;border:0;cursor:pointer;
      padding:12px 26px;border-radius:999px;
      background:linear-gradient(135deg,#fff,#ffeef3);
      color:var(--pink);font-weight:600
    }
    button:hover{transform:translateY(-2px);box-shadow:0 12px 24px rgba(0,0,0,.2)}

    /* floating hearts */
    .heart{position:fixed;bottom:-20px;pointer-events:none;opacity:.9;animation:up 7s linear infinite}
    @keyframes up{to{transform:translateY(-120vh) scale(1.6);opacity:0}}

    /* HOME scrapbook */
    .home-scrapbook{position:absolute;inset:70px 0 0 0;pointer-events:none}
    .mini-photo{
      position:absolute;
      width:140px;
      background:#fff;
      padding:10px 10px 16px;
      border-radius:6px;
      box-shadow:0 14px 28px rgba(0,0,0,.28);
      transform:rotate(var(--r));
      animation:float 6s ease-in-out infinite;
      touch-action:none;
      cursor:grab;
    }
    .mini-photo:active{cursor:grabbing}
    .mini-photo:active{cursor:grabbing}
    .mini-photo img{width:100%;height:120px;object-fit:cover;border-radius:4px}
    .mini-photo span{
      display:block;
      margin-top:8px;
      font-family:'Patrick Hand',cursive;
      color:#222;
      font-size:0.95rem;
      line-height:1.3;
      background:rgba(255,255,255,0.9);
      padding:4px 6px;
      border-radius:4px;
    }
    @keyframes float{50%{transform:translateY(-8px) rotate(var(--r))}}
    .p1{top:18%;left:6%;--r:-6deg}
    .p2{top:24%;right:8%;--r:5deg}
    .p3{bottom:22%;left:10%;--r:4deg}
    .p4{bottom:18%;right:14%;--r:-5deg}

    /* letter */
    .letter p{font-family:'Playfair Display',serif;font-size:1.1rem}

    /* footer */
    footer{opacity:.8;font-size:.85rem}

    /* music toggle */
    .music{
      position:fixed;right:16px;bottom:16px;z-index:9
    }
    .music button{padding:10px 14px}

    /* mobile tweaks */
    @media(max-width:600px){
      h1{font-size:2.4rem}
      .mini-photo{width:130px}
      .mini-photo img{height:110px}
      .mini-photo span{font-size:0.85rem}
    }
      .mini-photo{width:120px}
    }
  .heartbeat{animation:heartbeat 1.5s infinite;cursor:pointer}@keyframes heartbeat{0%{transform:scale(1)}25%{transform:scale(1.08)}40%{transform:scale(1)}60%{transform:scale(1.12)}100%{transform:scale(1)}}
.heartbeat.fast{animation:heartbeat .6s infinite}

.valentine-line{
  font-family:'Patrick Hand',cursive;
  font-size:2.2rem;
  color:#fff;
  text-shadow:0 4px 14px rgba(255,0,100,.8);
  animation:pulse 1.6s infinite;
  margin-top:6px;
}
@keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.08)}}


/* MOBILE LAYOUT FIXES */
.mobile-hero{
  position:relative;
  z-index:5;
  text-align:center;
  padding:12px 8px 20px;
}

@media(max-width:600px){
  .page{padding-top:80px}

  .home-scrapbook{
    position:relative;
    inset:auto;
    width:100%;
    height:360px;
    margin-top:10px;
    pointer-events:auto;
  }

  .mini-photo{
    width:120px;
  }

  .p1{top:10%;left:5%}
  .p2{top:12%;right:5%}
  .p3{top:55%;left:8%}
  .p4{top:55%;right:8%}

  h1{font-size:2.2rem}
  h2{font-size:1.1rem}

  .valentine-line{
    font-size:1.6rem;
    margin-bottom:8px;
  }
}

</style>
</head>
<body>

  <div class="hero"><strong>For Amrika ❤️</strong></div>

  <!-- HOME -->
  <section class="page active" id="home">
    <div class="mobile-hero">
    <h1 id="whisper" class="heartbeat">Amrika ❤️</h1>
    <div id="whisperText" style="opacity:0;font-family:'Patrick Hand',cursive;font-size:1.2rem;margin-top:-10px">Hey Amrika…</div>
    <h2>My wiffeyyy, my favorite person</h2>
    <div class="valentine-line">Love You my cutiiieee bubu💗</div>
    

        </div>

    <div class="home-scrapbook">
      <div class="mini-photo draggable p1"><img src="photo1.jpg"><span>Your eyes have a magic I fall for every time.</span></div>
      <div class="mini-photo draggable p2"><img src="photo2.jpg"><span>With you beside me, everything feels right.</span></div>
      <div class="mini-photo draggable p3"><img src="photo3.jpg"><span>This smile is my favorite sight.</span></div>
      <div class="mini-photo draggable p4"><img src="photo4.jpg"><span>Moments with you are my safest place.</span></div>
    </div>

    <div class="card">
      <p>This little website is made just for you — a soft place filled with love, memories, and tiny pieces of my heart. Take your time, wiffeyyy 💕</p>
      <div class="buttons">
        <button onclick="go('letter')">Read My Letter 💌</button>
        <button onclick="go('why')">Why I Love You 💖</button>
        <button onclick="openSecret()">Secret 💗</button>
        
      </div>
    </div>
    <footer>Made with love by Dipjoy 💖</footer>
  </section>

  <!-- SECRET OVERLAY -->
  <div id="secretOverlay" style="display:none;position:fixed;inset:0;z-index:20;background:rgba(0,0,0,.55);backdrop-filter:blur(6px);">
    <div style="max-width:420px;margin:12vh auto;background:var(--glass);border-radius:24px;padding:26px 22px;box-shadow:0 30px 60px rgba(0,0,0,.35);text-align:center;color:#fff">
      <h2 style="font-family:'Playfair Display',serif;margin-top:0">Unlock my secret 💞</h2>
      <p style="opacity:.9">Only my wiffeyyy knows the word.</p>
      <input id="secretInput" placeholder="Enter the secret emoji" style="width:100%;padding:12px 14px;border-radius:14px;border:0;margin:10px 0" />
      <p class="hint" style="font-size:.85rem;opacity:.85;margin-bottom:14px">Hint: enter the emoji that we used to confess our love in crowd.</p>
      <div class="buttons" style="justify-content:center">
        <button onclick="checkSecret()">Unlock ✨</button>
        <button onclick="closeSecret()">Close</button>
      </div>
      <p id="secretError" style="display:none;color:#ffd6df;margin-top:10px">Hmm… try again 💭</p>
    </div>
  </div>

  <!-- SECRET PAGE -->
  <section class="page" id="secret">
    <h1>Just Between Us 💗</h1>
    <div class="card">
      <p style="font-family:'Playfair Display',serif;font-size:1.15rem">
        If you’re reading this, it means you unlocked a piece of my heart.
        I don’t say this lightly — you are my safe place, my calm, my favorite thought.
        I want a thousand small moments with you, and a lifetime of choosing you.
        <br><br>
        The kisses of this Valentine's Day is remaining the pending ones, you have to give me the kisses with interest💋<br><br>Forever yours,<br>Dipjoy 💖
      </p>
      <div class="buttons"><button onclick="go('home')">Back Home 🏡</button></div>
    </div>
  </section>

  <!-- LETTER -->
  <section class="page" id="letter">
    <h1>A Letter for You 💌</h1>
    <div class="card letter">
      <p>My dearest Amrika,<br><br>
      You have a way of turning ordinary moments into something gentle and bright. Your smile feels like home, and your presence brings a quiet peace. With you, laughter comes easily — and even silence feels warm.<br><br>
      I choose you, again and again, in the little ways and the big ones. Always yours,<br>Dipjoy 💖</p>
      <div class="buttons"><button onclick="go('home')">Back Home 🏡</button></div>
    </div>
  </section>

  <!-- WHY -->
  <section class="page" id="why">
    <h1>Why I Love You 💖</h1>
    <div class="card">
      <p>Because you’re kind and real. Because your laughter makes everything lighter. Because being with you feels natural and safe. And mostly… because you are you. My wiffeyyy ❤️</p>
      <div class="buttons"><button onclick="go('home')">Back Home 🏡</button></div>
    </div>
  </section>

  <!-- Music (optional: add music.mp3 next to index.html) -->
  <div class="music"><button onclick="toggleMusic()">pause music💗</button></div>
  <audio id="bgm" loop autoplay muted playsinline src="music.mp3"></audio>

  <script>
    const pages = document.querySelectorAll('.page');
    function go(id){ pages.forEach(p=>p.classList.remove('active')); document.getElementById(id).classList.add('active'); }

    // whisper effect
    const heart=document.getElementById('whisper');
    heart.addEventListener('click',()=>{
      heart.classList.add('fast');
      setTimeout(()=>heart.classList.remove('fast'),2500);
    });
    window.addEventListener('load', ()=>{
      const w=document.getElementById('whisperText');
      setTimeout(()=>{ w.style.transition='opacity 2s'; w.style.opacity=1; },1200);
    });

    // floating hearts
    setInterval(()=>{const h=document.createElement('div');h.className='heart';h.textContent='❤️';h.style.left=Math.random()*100+'vw';h.style.animationDuration=4+Math.random()*4+'s';document.body.appendChild(h);setTimeout(()=>h.remove(),8000)},380);

    // music autoplay
    const bgm=document.getElementById('bgm');
    document.addEventListener('click',()=>{ if(bgm.muted){ bgm.muted=false; bgm.play(); }},{once:true});
    function toggleMusic(){ bgm.paused?bgm.play():bgm.pause(); }

    

    // secret unlock
    const SECRET_WORD='🤟';
    function openSecret(){ document.getElementById('secretOverlay').style.display='block'; }
    function closeSecret(){ document.getElementById('secretOverlay').style.display='none'; document.getElementById('secretError').style.display='none'; }
    function checkSecret(){ const v=document.getElementById('secretInput').value.trim(); if(v===SECRET_WORD){ closeSecret(); go('secret'); } else document.getElementById('secretError').style.display='block'; }

    // draggable photos
    document.querySelectorAll('.draggable').forEach(photo=>{
      let startX=0,startY=0,dragging=false;
      photo.addEventListener('mousedown',startDrag);
      photo.addEventListener('touchstart',startDrag,{passive:false});
      function startDrag(e){ dragging=true; photo.style.animation='none'; const r=photo.getBoundingClientRect(); const x=e.touches?e.touches[0].clientX:e.clientX; const y=e.touches?e.touches[0].clientY:e.clientY; startX=x-r.left; startY=y-r.top; document.addEventListener('mousemove',drag); document.addEventListener('touchmove',drag,{passive:false}); document.addEventListener('mouseup',endDrag); document.addEventListener('touchend',endDrag); }
      function drag(e){ if(!dragging) return; e.preventDefault(); const x=e.touches?e.touches[0].clientX:e.clientX; const y=e.touches?e.touches[0].clientY:e.clientY; photo.style.left=(x-startX)+'px'; photo.style.top=(y-startY)+'px'; }
      function endDrag(){ dragging=false; document.removeEventListener('mousemove',drag); document.removeEventListener('touchmove',drag); document.removeEventListener('mouseup',endDrag); document.removeEventListener('touchend',endDrag); }
    });
  </script>
</body>
</html>
