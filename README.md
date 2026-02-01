<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Best Friends 💛</title>

  <!-- Premium font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Poppins', sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #fdf1f6, #e6ecff);
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      overflow: hidden;
    }

    h1 {
      font-size: 2.6rem;
      color: #2f2f2f;
      margin-bottom: 10px;
    }

    .sub {
      color: #555;
      font-size: 1.1rem;
    }

    .buttons {
      margin-top: 40px;
      position: relative;
      width: 320px;
      height: 200px;
    }

    button {
      font-size: 1.1rem;
      padding: 12px 34px;
      border: none;
      border-radius: 40px;
      cursor: pointer;
      position: absolute;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      transition: transform 0.2s ease;
    }

    button:hover {
      transform: scale(1.05);
    }

    #yes {
      background-color: #ff7a9c;
      color: white;
      left: 50%;
      transform: translateX(-50%);
    }

    #no {
      background-color: white;
      color: #ff7a9c;
    }

    #yay {
      display: none;
      margin-top: 30px;
      animation: fadeIn 1s ease forwards;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <h1>Shradha, will you stay my best friend? 🥺💛</h1>
  <div class="sub">No pressure… but also, pressure 😌</div>

  <div class="buttons">
    <button id="yes">Yes 💛</button>
    <button id="no">No 😶</button>
  </div>

  <div id="yay">
    <h2>Oh thank GOD 😮‍💨🥹</h2>
    <p>Best friends. Always. 💛</p>
    <img src="https://media.giphy.com/media/l4FGuhL4U2WyjdkaY/giphy.gif" width="300">
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");
    const yay = document.getElementById("yay");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * 260;
      const y = Math.random() * 140;
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    yesBtn.addEventListener("click", () => {
      document.querySelector(".buttons").style.display = "none";
      yay.style.display = "block";
    });
  </script>

</body>
</html>
