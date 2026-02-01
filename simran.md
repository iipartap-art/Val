<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Simran, Will You Be My Valentine? 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff69b4, #ffb6c1);
      font-family: 'Comic Sans MS', cursive, sans-serif;
      overflow: hidden;
    }

    .flowers {
      position: absolute;
      top: 0;
      left: 0;
      font-size: 30px;
      width: 100%;
      height: 100%;
      pointer-events: none;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      align-content: space-around;
      opacity: 0.4;
    }

    .card {
      background: #ffe4f1;
      padding: 40px;
      border-radius: 25px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.25);
      z-index: 1;
    }

    h1 {
      color: #d63384;
      margin-bottom: 30px;
    }

    button {
      font-size: 18px;
      padding: 12px 30px;
      border-radius: 30px;
      border: none;
      cursor: pointer;
      margin: 10px;
      transition: 0.2s ease;
    }

    #yesBtn {
      background-color: #ff4d9d;
      color: white;
    }

    #yesBtn:hover {
      transform: scale(1.15);
    }

    #noBtn {
      background-color: #d8bfd8;
      color: #333;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="flowers">
    🌸 💜 🌸 💐 🌸 💜 🌸 💐 🌸 💜 🌸 💐
    🌸 💜 🌸 💐 🌸 💜 🌸 💐 🌸 💜 🌸 💐
    🌸 💜 🌸 💐 🌸 💜 🌸 💐 🌸 💜 🌸 💐
  </div>

  <div class="card">
    <h1>Simran 💖<br>Will you be my Valentine? 🌸💜</h1>
    <button id="yesBtn">Yes 💖</button>
    <button id="noBtn">No 😢</button>
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");
    const yesBtn = document.getElementById("yesBtn");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - noBtn.clientWidth);
      const y = Math.random() * (window.innerHeight - noBtn.clientHeight);

      noBtn.style.left = `${x}px`;
      noBtn.style.top = `${y}px`;
    });

    yesBtn.addEventListener("click", () => {
      document.body.innerHTML = `
        <div style="
          height: 100vh;
          display: flex;
          justify-content: center;
          align-items: center;
          background: linear-gradient(135deg, #ff69b4, #ffb6c1);
          font-family: 'Comic Sans MS', cursive;
          text-align: center;
        ">
          <h1 style="color:#d63384;">
            Yayyy Simran!! 💘🥰🌸💜<br>
            You just made me the happiest person 💐
          </h1>
        </div>
      `;
    });
  </script>

</body>
</html>
