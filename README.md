# 13579jo.github.io
英格莉魔法工作室官方網站
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <title>家家的魔法作品圖牆</title>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+TC&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Noto Serif TC', serif;
      background: #1a001a;
      color: #fff;
      text-align: center;
    }

    h1 {
      margin: 40px 0 10px;
      font-size: 2.5em;
    }

    p.subtitle {
      margin-bottom: 10px;
      color: #ccc;
      font-size: 1.1em;
    }

    .quote-box {
      background: rgba(255, 255, 255, 0.08);
      border-radius: 12px;
      padding: 20px;
      margin: 20px auto;
      max-width: 600px;
      font-size: 1.2em;
      font-weight: bold;
      color: #ffeaff;
      box-shadow: 0 0 10px rgba(255,255,255,0.2);
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 15px;
      padding: 0 20px 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .grid img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 0 12px rgba(255,255,255,0.3);
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 0.8s ease forwards;
      animation-delay: calc(var(--i) * 0.1s);
    }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .audio-btn {
      background: #fff;
      color: #6B3FA0;
      border: none;
      padding: 10px 20px;
      border-radius: 25px;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      margin: 20px auto;
      display: inline-block;
    }

    .audio-btn:hover {
      background: #d1b3ff;
      color: white;
    }

    a.back-home {
      display: inline-block;
      margin: 30px 0;
      padding: 10px 20px;
      background: #fff;
      color: #6B3FA0;
      text-decoration: none;
      border-radius: 25px;
      font-weight: bold;
      transition: 0.3s;
    }

    a.back-home:hover {
      background: #d1b3ff;
      color: white;
    }
  </style>
</head>
<body>
  <h1>🔮 家家的魔法作品圖牆 ✨</h1>
  <p class="subtitle">這裡收藏著我靈感四溢的創作與療癒時刻</p>

  <!-- 隨機語錄 -->
  <div class="quote-box">
    <p id="quote">🌟 「願你的心靈，在每一次創作中找到療癒的力量。」</p>
  </div>

  <!-- 語音播放 -->
  <audio id="bgAudio" src="welcome.mp3"></audio>
  <button onclick="document.getElementById('bgAudio').play()" class="audio-btn">▶️ 播放療癒語音</button>

  <!-- 作品圖牆 -->
  <div class="grid">
    <img src="861047_0.jpg" alt="作品1" style="--i:1;">
    <img src="S__36348138_0.jpg" alt="作品2" style="--i:2;">
    <img src="S__36348139_0.jpg" alt="作品3" style="--i:3;">
    <img src="S__36348140_0.jpg" alt="作品4" style="--i:4;">
    <img src="S__36348141_0.jpg" alt="作品5" style="--i:5;">
    <img src="S__36348142_0.jpg" alt="作品6" style="--i:6;">
    <img src="S__36348143_0.jpg" alt="作品7" style="--i:7;">
    <img src="S__36348144_0.jpg" alt="作品8" style="--i:8;">
    <img src="S__36348145_0.jpg" alt="作品9" style="--i:9;">
    <img src="S__36348146_0.jpg" alt="作品10" style="--i:10;">
    <img src="S__36348147_0.jpg" alt="作品11" style="--i:11;">
    <img src="S__36348149_0.jpg" alt="作品12" style="--i:12;">
    <img src="S__36348150_0.jpg" alt="作品13" style="--i:13;">
    <img src="S__36348151_0.jpg" alt="作品14" style="--i:14;">
    <img src="S__36348152_0.jpg" alt="作品15" style="--i:15;">
    <img src="S__36348153_0.jpg" alt="作品16" style="--i:16;">
  </div>

  <a class="back-home" href="index.html">← 回首頁</a>

  <!-- 隨機語錄腳本 -->
  <script>
    const quotes = [
      "🌟 「願你的心靈，在每一次創作中找到療癒的力量。」",
      "🦄 「宇宙一直都在聽你說話，記得溫柔對自己。」",
      "✨ 「你就是光，哪怕你曾經不相信自己。」",
      "🔮 「真正的魔法，是你選擇了活出真實的自己。」"
    ];
    document.getElementById("quote").innerText = quotes[Math.floor(Math.random() * quotes.length)];
  </script>
</body>
</html>


