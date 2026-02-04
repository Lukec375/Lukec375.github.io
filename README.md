<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Be My Valentine</title>
  <style>
    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: Arial, Helvetica, sans-serif;
      background: #ffe6ec;
      color: #111;
    }

    .card {
      background: #fff;
      padding: 32px;
      border-radius: 16px;
      width: 90%;
      max-width: 420px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.15);
    }

    h1 {
      margin: 0 0 16px 0;
      font-size: 28px;
    }

    p {
      margin: 0 0 24px 0;
      font-size: 16px;
      line-height: 1.4;
    }

    .buttons {
      display: flex;
      gap: 16px;
      justify-content: center;
    }

    button {
      padding: 12px 20px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    .yes {
      background: #ff4d6d;
      color: #fff;
    }

    .no {
      background: #e0e0e0;
      color: #111;
      position: relative;
    }

    .hidden {
      display: none;
    }

    .heart {
      font-size: 64px;
      color: #ff4d6d;
      margin-bottom: 16px;
      animation: beat 1s infinite;
    }

    @keyframes beat {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }
  </style>
</head>
<body>
  <div class="card" id="card">
    <div class="heart">♥</div>
    <h1>Will you be my Valentine?</h1>
    <p>You make my days better. I want to spend this one with you.</p>
    <div class="buttons">
      <button class="yes" onclick="sayYes()">Yes</button>
      <button class="no" id="noBtn">No</button>
    </div>
  </div>

  <script>
    const noBtn = document.getElementById('noBtn');

    noBtn.addEventListener('mouseover', moveButton);
    noBtn.addEventListener('click', moveButton);

    function moveButton() {
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 200 - 100;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    }

    function sayYes() {
      const card = document.getElementById('card');
      card.innerHTML = `
        <div class="heart">♥</div>
        <h1>She said yes.</h1>
        <p>I knew it. Happy Valentine’s Day.</p>
      `;
    }
  </script>
</body>
</html>
