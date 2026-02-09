# valentine-
A little something for my pooks 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Toosh 💕</title>
  <style>
    body {
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Comic Sans MS', cursive;
      text-align: center;
      overflow: hidden;
    }

    .card {
      background: #fff0f6;
      padding: 40px;
      border-radius: 25px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.15);
      max-width: 320px;
    }

    h1 {
      color: #ff4d88;
      font-size: 2em;
    }

    p {
      color: #ff6fa5;
      font-size: 1.1em;
    }

    .bear {
      font-size: 80px;
      margin: 15px 0;
    }

    button {
      padding: 12px 25px;
      font-size: 16px;
      border-radius: 20px;
      border: none;
      cursor: pointer;
      margin: 10px;
    }

    .yes {
      background: #ff4d88;
      color: white;
    }

    .no {
      background: white;
      border: 2px solid #ff4d88;
      color: #ff4d88;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Toosh 💕</h1>
    <div class="bear">🧸</div>
    <p>Will you be my Valentine?</p>

    <button class="yes" onclick="yesClick()">Yes 💖</button>
    <button class="no" id="noBtn">No 🙃</button>
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 120);
      const y = Math.random() * (window.innerHeight - 60);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    function yesClick() {
      document.body.innerHTML = `
        <div style="text-align:center;">
          <h1 style="color:#ff4d88;">YAY TOOSH 💖🧸</h1>
          <p style="font-size:1.2em;">You just made me the happiest 💕</p>
        </div>
      `;
    }
  </script>

</body>
</html>
