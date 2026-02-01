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
      margin-bottom: 12px;
    }

    .sub {
      font-size: 1.1rem;
      color: #555;
    }

    .buttons {
      margin-top: 40px;
      position: relative;
      width: 340px;
      height: 220px;
    }

    button {
      font-size: 1.1rem;
      padding: 14px 38px;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      position: absolute;
      box-shadow: 0 10px 25px rgba(0,0,0,0.12);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    button:hover {
      transform: scale(1.06);
      box-shadow: 0 14px 30px rgba(0,0,0,0.15);
    }

    #yes {
      background: linear-gradient(135deg, #ff7a9c, #ff4f7b);
      color: white;
      left: 50%;
      transform: translateX(-50%);
    }

    #no {
      background-color: white;
      color: #ff4f7b;
    }

    #yay {
      display: none;
      margin-top: 30px;
      animation: fadeIn 1.2s ease forwards;
    }

    #yay img {
      margin-top: 20px;
      border-radius: 18px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.18);
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(12px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
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
    <p>Best friends forever. Always. 💛</p>
    <img src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExdjhwbGhrOWd5a2IwZGMxeGNuazVxOXJ0cWk5a2V2YmlhaGIzOWx1cCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/o75ajIFH0QnQC3nCeD/giphy.gif" width="320">
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");
    const yay = document.getElementById("yay");

    noBtn.addEventListener("mouse
