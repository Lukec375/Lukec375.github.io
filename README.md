<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>To My Ari 💌</title>
  <style>
    :root {
      --pink: #ff85c0;
      --dark-pink: #ff4d94;
      --red: #ff3366;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', system-ui, sans-serif;
      background: url('https://thumbs.dreamstime.com/b/shimmering-glass-hearts-floating-pink-clouds-abstract-dreamy-background-three-dimensional-rendering-soft-pastel-colors-367478292.jpg') no-repeat center center fixed;
      background-size: cover;
      color: #333;
      min-height: 100vh;
      overflow-x: hidden;
      position: relative;
    }

    body::before {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(255, 240, 245, 0.45);
      z-index: -2;
    }

    .hearts {
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      pointer-events: none;
      z-index: -1;
    }

    .heart {
      position: absolute;
      font-size: 1.5rem;
      animation: float 12s infinite linear;
      opacity: 0.7;
    }

    @keyframes float {
      0%   { transform: translateY(100vh) rotate(0deg); }
      100% { transform: translateY(-15vh) rotate(360deg); }
    }

    header {
      text-align: center;
      padding: 80px 20px 40px;
    }

    h1 {
      font-size: clamp(2.8rem, 9vw, 5.5rem);
      color: var(--red);
      margin-bottom: 0.3em;
      text-shadow: 0 2px 10px rgba(255, 77, 148, 0.3);
    }

    .letter {
      max-width: 700px;
      margin: 0 auto 3rem;
      background: white;
      padding: 2.5rem;
      border-radius: 20px;
      box-shadow: 0 10px 40px rgba(255, 105, 180, 0.25);
      border: 2px dashed var(--pink);
      font-size: 1.25rem;
      line-height: 1.6;
      color: #444;
    }

    .letter p {
      margin-bottom: 1.5rem;
    }

    .signature {
      text-align: right;
      font-style: italic;
      color: var(--dark-pink);
      font-size: 1.4rem;
      margin-top: 2rem;
    }

    .buttons {
      text-align: center;
      margin: 3rem 0;
    }

    button {
      font-size: 1.6rem;
      padding: 1rem 2.5rem;
      margin: 1rem;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }

    .yes {
      background: linear-gradient(45deg, #ff3366, #ff6699);
      color: white;
    }

    .yes:hover {
      transform: scale(1.15);
      box-shadow: 0 15px 30px rgba(255, 51, 102, 0.4);
    }

    .no {
      background: #ffebee;
      color: #ff3366;
      border: 3px solid #ff3366;
    }

    .no:hover {
      background: #ff3366;
      color: white;
      transform: scale(1.1);
    }

    #yes-page, #sad-page {
      display: none;
      text-align: center;
      padding: 60px 20px;
      min-height: 100vh;
    }

    #yes-page {
      background: linear-gradient(135deg, #4a148c, #7b1fa2);
      color: white;
      position: relative;
      overflow: hidden;
    }

    #yes-page::before {
      content: "";
      position: absolute;
      inset: 0;
      background: url('https://thumbs.dreamstime.com/b/shimmering-glass-hearts-floating-pink-clouds-abstract-dreamy-background-three-dimensional-rendering-soft-pastel-colors-367478292.jpg') no-repeat center center;
      background-size: cover;
      opacity: 0.15;
      z-index: -1;
    }

    #sad-page {
      background: linear-gradient(135deg, #2c003e, #4a0072);
      color: white;
    }

    .response-img {
      max-width: 90%;
      max-height: 60vh;
      border-radius: 20px;
      box-shadow: 0 15px 40px rgba(0,0,0,0.6);
      margin: 2rem auto;
      display: block;
    }

    .response-h2 {
      font-size: 3.5rem;
      margin: 1rem 0;
    }

    #yes-page .response-h2 { color: #ffccff; }
    #sad-page .response-h2 { color: #ff99cc; }

    .response-p {
      font-size: 1.8rem;
      max-width: 700px;
      margin: 2rem auto;
      line-height: 1.6;
      font-weight: 500;
    }

    .back-btn, .yay-btn {
      background: linear-gradient(45deg, #ff99cc, #ff6699);
      color: white;
      font-size: 1.4rem;
      padding: 1rem 2.5rem;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      margin-top: 2rem;
    }

    .yay-btn {
      background: linear-gradient(45deg, #ffeb3b, #ff9800);
    }

    .back-btn:hover, .yay-btn:hover {
      transform: scale(1.1);
    }

    footer {
      text-align: center;
      padding: 3rem 1rem;
      color: #777;
      font-size: 0.95rem;
    }

    @media (max-width: 600px) {
      .letter { padding: 1.8rem; font-size: 1.1rem; }
      button { font-size: 1.4rem; padding: 0.9rem 2rem; }
    }
  </style>
</head>
<body>

  <div class="hearts" id="hearts"></div>

  <div id="main-content">

    <header>
      <h1>Hey Ari 💕</h1>
    </header>

    <div class="letter">
      <p>My beautiful cinnamon,</p>
      
      <p>You are the love of my life, and without you, I feel like only half of myself. Your smile lights up my entire world, your eyes hold a kindness and sparkle that make my heart skip every time I look at you. Your beauty — inside and out — takes my breath away; the way you glow with warmth, grace, and that effortless charm is something I'll never get tired of admiring.</p>
      
      <p>You've shown me what true love really means: it's in the little moments, the way you make me laugh until my sides hurt, how you turn ordinary days into something magical just by being you. You make me happier than I ever thought possible, and you've taught me to love more deeply, more openly, more completely.</p>
      
      <p>You mean everything to me, Ari. I would move mountains, cross oceans, do absolutely anything for you — because a life with you is the only one I want.</p>
      
      <p>So I have one very important question for you...</p>

      <h2 style="text-align:center; color: var(--red); margin: 2rem 0; font-size: 2.2rem;">
        Will you be my Valentine? 🥺❤️
      </h2>

      <div class="signature">
        Forever yours,<br>
        Luka 💌
      </div>
    </div>

    <div class="buttons">
      <button class="yes" onclick="showYes()">Yes! Of course! 💖</button>
      
      <button class="no" onclick="showSad()">No... sorry 😔</button>
    </div>

  </div>

  <div id="yes-page">
    <h2 class="response-h2">YESSS BABYYY, I AM SO HAPPY! 🎉💖</h2>
    <img class="response-img" src="https://assets.teenvogue.com/photos/5994baf49bca9f4c417198b7/16:9/w_2560,c_limit/MCDTANG_EC051_H.JPG" alt="Rapunzel and Flynn in the magical lantern scene from Tangled">
    <p class="response-p">You and I are like Rapunzel and Flynn but I love you even more than he loves her hehe 😘✨</p>
    <button class="yay-btn">I'm so happy!</button>
  </div>

  <div id="sad-page">
    <h2 class="response-h2">Now kitty is sad... 💔</h2>
    <img class="response-img" src="https://thumbs.dreamstime.com/b/apology-eyes-adorable-kitten-holding-i-m-sorry-sign-image-melts-hearts-tiny-peering-torn-edges-305639152.jpg" alt="Adorable sad kitten holding 'I'm sorry' sign">
    <p class="response-p">think about it again pleeeeeassseeee 🥺😿</p>
    <button class="back-btn" onclick="goBack()">Okay fine... ask me again ❤️</button>
  </div>

  <footer>
    Created with all my love by Luka just for Ari 💕 • February 2026
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.9.3/dist/confetti.browser.min.js"></script>

  <script>
    // Floating hearts
    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.innerHTML = ['❤️','💖','💕','💗','💞','🫀'][Math.floor(Math.random()*6)];
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (Math.random() * 8 + 8) + 's';
      heart.style.fontSize = (Math.random() * 1.2 + 0.8) + 'rem';
      document.getElementById('hearts').appendChild(heart);
      setTimeout(() => heart.remove(), 15000);
    }

    setInterval(createHeart, 400);
    for(let i = 0; i < 15; i++) createHeart();

    // Show yes response with confetti
    function showYes() {
      document.getElementById('main-content').style.display = 'none';
      document.getElementById('yes-page').style.display = 'block';
      
      // Pink romantic confetti burst
      confetti({
        particleCount: 120,
        spread: 80,
        origin: { y: 0.6 },
        colors: ['#ff3366', '#ff6699', '#ff99cc', '#ffb3d9', '#ffffff', '#ffeb3b'],
        ticks: 300
      });
    }

    // Show sad cat
    function showSad() {
      document.getElementById('main-content').style.display = 'none';
      document.getElementById('sad-page').style.display = 'block';
    }

    // Go back to main
    function goBack() {
      document.getElementById('sad-page').style.display = 'none';
      document.getElementById('yes-page').style.display = 'none';
      document.getElementById('main-content').style.display = 'block';
    }
  </script>

</body>
</html>
