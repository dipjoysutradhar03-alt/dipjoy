<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For Amrika ❤️</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, sans-serif;
      background: linear-gradient(135deg, #ffb6c1, #ffe4e1);
      color: #fff;
      text-align: center;
      overflow-x: hidden;
    }

    .page {
      display: none;
      min-height: 100vh;
      padding: 40px 20px;
      box-sizing: border-box;
    }

    .page.active {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      animation: fadeIn 0.8s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }

    h2 {
      font-weight: 300;
      margin-bottom: 25px;
    }

    .card {
      background: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(12px);
      border-radius: 25px;
      padding: 30px;
      max-width: 700px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.25);
    }

    .card p {
      font-size: 1.15rem;
      line-height: 1.7;
    }

    .buttons {
      margin-top: 30px;
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      justify-content: center;
    }

    button {
      padding: 12px 28px;
      border: none;
      border-radius: 30px;
      font-size: 1rem;
      cursor: pointer;
      background: #fff;
      color: #ff5a7a;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    button:hover {
      transform: translateY(-3px);
      box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    }

    /* Gallery */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 15px;
      margin-top: 20px;
    }

    .gallery img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 15px;
      box-shadow: 0 8px 15px rgba(0,0,0,0.25);
    }

    /* Floating hearts */
    .heart {
      position: fixed;
      bottom: -20px;
      color: rgba(255,255,255,0.9);
      animation: floatUp 6s linear infinite;
      font-size: 20px;
      pointer-events: none;
    }

    @keyframes floatUp {
      from { transform: translateY(0) scale(1); opacity: 1; }
      to { transform: translateY(-110vh) scale(1.5); opacity: 0; }
    }
    @import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap');

    .home-scrapbook {
      position: absolute;
      inset: 0;
      pointer-events: none;
    }

    .mini-photo {
      position: absolute;
      width: 140px;
      background: #fff;
      padding: 10px 10px 16px;
      border-radius: 6px;
      box-shadow: 0 10px 20px rgba(0,0,0,0.25);
      transform: rotate(var(--r));
      animation: floatSoft 6s ease-in-out infinite;
    }

    .mini-photo img {
      width: 100%;
      height: 120px;
      object-fit: cover;
      border-radius: 4px;
    }

    .mini-photo span {
      display: block;
      margin-top: 6px;
      font-family: 'Patrick Hand', cursive;
      font-size: 0.95rem;
      color: #444;
    }

    .p1 { top: 18%; left: 8%; --r: -6deg; }
    .p2 { top: 25%; right: 10%; --r: 5deg; }
    .p3 { bottom: 20%; left: 12%; --r: 4deg; }
    .p4 { bottom: 18%; right: 14%; --r: -5deg; }

    @keyframes floatSoft {
      0%, 100% { transform: translateY(0) rotate(var(--r)); }
      50% { transform: translateY(-8px) rotate(var(--r)); }
    }

</style>
</head>
<body>

  <!-- PAGE 1: HOME -->
  <div class="page active" id="home">
    <h1>Amrika ❤️</h1>
    <h2>My wiffeyyy, my favorite person</h2>

    <!-- Floating scrapbook photos on home -->
    <div class="home-scrapbook">
      <div class="mini-photo p1">
        <img src="photo1.jpg" alt="Amrika">
        <span>Your eyes have a magic I fall for every time.</span>
      </div>
      <div class="mini-photo p2">
        <img src="photo2.jpg" alt="Us">
        <span>With you beside me, everything feels right.</span>
      </div>
      <div class="mini-photo p3">
        <img src="photo3.jpg" alt="Smile">
        <span>This smile is my favorite sight.</span>
      </div>
      <div class="mini-photo p4">
        <img src="photo4.jpg" alt="Together">
        <span>Moments with you are my safest place.</span>
      </div>
    </div>

    <div class="card">
      <p>
        This little website is made just for you.
        A place filled with love, memories, and tiny pieces of my heart.
        Click around slowly… every page is for you, wiffeyyy 💕
      </p>

      <div class="buttons">
        <button onclick="goTo('letter')">Read My Letter 💌</button>
        <button onclick="goTo('why')">Why I Love You 💖</button>
      </div>
    </div>
  </div>
  </div>

  <!-- PAGE 2: LOVE LETTER -->
  <div class="page" id="letter">
    <h1>A Letter for You 💌</h1>
    <div class="card">
      <p>
        My dearest Amrika,
        <br><br>
        You have a way of making ordinary days feel special.
        Your smile feels like home, and your presence brings me peace.
        With you, laughter comes easily, and even silence feels comforting.
        <br><br>
        I love the way you care, the way you understand,
        and the way you make my world softer just by being in it.
        You are not just someone I love — you are someone I choose,
        again and again.
        <br><br>
        Always yours,<br>
        Dipjoy 💖
      </p>

      <div class="buttons">
        <button onclick="goTo('home')">Back Home 🏡</button>
      </div>
    </div>
  </div>

    <!-- PAGE 4: WHY I LOVE YOU -->
  <div class="page" id="why">
    <h1>Why I Love You 💖</h1>
    <div class="card">
      <p>
        I love you because you are kind, thoughtful, and real.
        <br><br>
        Because you laugh in a way that makes everything lighter.
        Because you care deeply and love genuinely.
        Because being with you feels natural and safe.
        <br><br>
        And mostly… because you are you.
        My wiffeyyy. ❤️
      </p>

      <div class="buttons">
        <button onclick="goTo('home')">Back Home 🏡</button>
      </div>
    </div>
  </div>

  <script>
    function goTo(pageId) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.getElementById(pageId).classList.add('active');
    }

    // Floating hearts
    setInterval(() => {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.innerText = '❤️';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (4 + Math.random() * 4) + 's';
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 8000);
    }, 350);
  </script>
</body>
</html>
