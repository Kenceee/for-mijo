<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday 🌸</title>
  <style>
    body {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      background: linear-gradient(to bottom, #ff9a9e, #fad0c4);
      font-family: 'Arial', sans-serif;
      overflow: hidden;
    }

    h1 {
      font-size: 36px;
      color: #ff6b81;
      text-align: center;
      margin-bottom: 20px;
      text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.2);
    }

    p {
      font-size: 18px;
      color: #333;
      margin-bottom: 30px;
      text-align: center;
    }

    .flower-container {
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
      gap: 20px;
      width: 100%;
    }

    .flower {
      position: relative;
      width: 120px;
      height: 120px;
      animation: float 3s ease-in-out infinite;
    }

    .flower .petal {
      position: absolute;
      width: 60px;
      height: 100px;
      background: #ff6b81;
      border-radius: 50%;
      top: 20px;
      left: 30px;
      transform-origin: bottom center;
    }

    .flower .petal:nth-child(1) { transform: rotate(0deg); }
    .flower .petal:nth-child(2) { transform: rotate(60deg); }
    .flower .petal:nth-child(3) { transform: rotate(120deg); }
    .flower .petal:nth-child(4) { transform: rotate(180deg); }
    .flower .petal:nth-child(5) { transform: rotate(240deg); }
    .flower .petal:nth-child(6) { transform: rotate(300deg); }

    .flower .center {
      position: absolute;
      width: 50px;
      height: 50px;
      background: yellow;
      border-radius: 50%;
      top: 50px;
      left: 50px;
      box-shadow: 0 0 10px rgba(255, 223, 0, 0.8);
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    button {
      margin-top: 40px;
      padding: 15px 30px;
      border: none;
      background: #ff6b81;
      color: white;
      font-size: 18px;
      border-radius: 25px;
      cursor: pointer;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
      transition: background 0.3s ease, transform 0.2s ease;
    }

    button:hover {
      background: #ff8c94;
      transform: translateY(-2px);
    }

    @keyframes glow {
      0%, 100% { box-shadow: 0 0 15px rgba(255, 107, 129, 0.6); }
      50% { box-shadow: 0 0 30px rgba(255, 107, 129, 1); }
    }
  </style>
</head>
<body>
  <h1>Happy Birthday, Pre! 🎉🌸</h1>
  <p>Here’s a little something to brighten your special day. You are the sunshine of my life. 💛</p>

  <div class="flower-container">
    <!-- Flower 1 -->
    <div class="flower">
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="center"></div>
    </div>

    <!-- Flower 2 -->
    <div class="flower">
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="petal"></div>
      <div class="center"></div>
    </div>
  </div>

  <button onclick="playSong()">Play the Song 🎵</button>

  <audio id="song" src="ikaw-lang.mp3"></audio>

  <script>
    function playSong() {
      const song = document.getElementById('song');
      song.play();
      alert("MISS YOUU!!. 🌸 Happy Birthday!");
    }
  </script>
</body>
</html>
