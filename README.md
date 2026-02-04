<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>To My Favorite Person 💌</title>
  <style>
    :root {
      --pink: #ff85c0;
      --dark-pink: #ff4d94;
      --red: #ff3366;
      --bg: #fff0f5;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', system-ui, sans-serif;
      background: linear-gradient(135deg, #fff0f5, #ffe4f1);
      color: #333;
      min-height: 100vh;
      overflow-x: hidden;
      position: relative;
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

    .maybe {
      background: #ffebee;
      color: #ff3366;
      border: 3px solid #ff3366;
    }

    .maybe:hover {
      background: #ff3366;
      color: white;
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

  <header>
    <h1>Hey [Her Name / Nickname] 💕</h1>
  </header>

  <div class="letter">
    <p>My love,</p>
    
    <p>Every day with you feels like Valentine's Day already... but I still want to make it official 😊</p>
    
    <p>You make my heart do stupid little flips, you laugh at my terrible jokes, and somehow you make even boring days feel magical.</p>
    
    <p>So I have one very important question for you...</p>

    <h2 style="text-align:center; color: var(--red); margin: 2rem 0; font-size: 2.2rem;">
      Will you be my Valentine? 🥺❤️
    </h2>

    <div class="signature">
      Forever yours,<br>
      [Your Name / Nickname] 💌
    </div>
  </div>

  <div class="buttons">
    <button class="yes" onclick="alert('YAYYYYY! 🎉💖 I love you so much! Let’s make this the best Valentine’s ever 😘')">Yes! Of course! 💖</button>
    
    <button class="maybe" onclick="alert('Take your time baby... but you know I’m not letting you go either way 😏❤️')">Umm... ask again in 5 mins? 😳</button>
  </div>

  <footer>
    Made with all my love just for you • February 2026
  </footer>

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
    // Initial burst
    for(let i=0; i<15; i++) createHeart();
  </script>

</body>
</html>
