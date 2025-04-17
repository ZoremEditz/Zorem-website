<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Zorem Editz</title>
  <style>
    * {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-image: url('https://4kwallpapers.com/images/walls/thumbs_3t/15351.jpg');
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      color: white;
      overflow-x: hidden;
    }

    header {
      background: rgba(0, 0, 0, 0.7);
      padding: 20px;
      text-align: center;
      position: relative;
    }

    header::after {
      content: '';
      background: url('https://i.ibb.co/gPgPrf9/jinwoo-silhouette.png') no-repeat center;
      background-size: contain;
      opacity: 0.2;
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 400px;
      height: 100%;
      pointer-events: none;
    }

    header h1 {
      margin: 0;
      font-size: 2.5rem;
      z-index: 2;
      position: relative;
    }

    #loading {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.8);
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      font-size: 2rem;
      z-index: 999;
    }

    #menuBtn {
      display: none;
      background-color: #ff4c98;
      color: white;
      font-size: 30px;
      border: none;
      cursor: pointer;
      padding: 10px;
      position: fixed;
      top: 10px;
      right: 10px;
      z-index: 999;
    }

    #dotMenu {
      display: none;
      position: fixed;
      top: 50px;
      right: 10px;
      background-color: rgba(0, 0, 0, 0.7);
      border-radius: 5px;
      padding: 10px;
    }

    #dotMenu a {
      color: white;
      display: block;
      padding: 5px 0;
      text-decoration: none;
    }

    #dotMenu a:hover {
      color: #ff4c98;
    }

    .section {
      padding: 30px 20px;
      max-width: 1200px;
      margin: auto;
      background: rgba(0, 0, 0, 0.7);
      margin-bottom: 20px;
      border-radius: 10px;
    }

    .section h2 {
      color: #ff4c98;
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .about p {
      font-size: 1.2rem;
      line-height: 1.8;
    }

    .video-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 20px;
    }

    iframe {
      width: 100%;
      height: 500px;
      border-radius: 10px;
    }

    .footer {
      background-color: rgba(0, 0, 0, 0.8);
      color: #aaa;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }

    a {
      color: #ff4c98;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    #scrollTopBtn {
      position: fixed;
      bottom: 30px;
      right: 30px;
      background: #ff4c98;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 50%;
      cursor: pointer;
      font-size: 18px;
      box-shadow: 0 0 10px #000;
      display: none;
    }

    #scrollTopBtn:hover {
      background: #ff79b0;
    }
  </style>
</head>
<body>
  <div id="loading">
    <div class="loader">Loading...</div>
  </div>

  <button id="menuBtn" onclick="toggleMenu()">&#8942;</button>

  <div id="dotMenu">
    <a href="#about">About</a>
    <a href="#videos">All Shorts</a>
    <a href="#contact">Connect</a>
  </div>

  <header>
    <h1>Zorem Editz</h1>
    <p>🔥 Anime Edits | JJK | Solo Leveling | More 🔥</p>
  </header>

  <section class="section about" id="about">
    <h2>👋 About Me</h2>
    <p>Yo! I'm Zorem Editz – a passionate content creator who loves anime and brings epic moments to life through edits. I post fire YouTube Shorts on anime like Jujutsu Kaisen, Solo Leveling, Naruto, and more! Whether you're here to vibe or get hyped, welcome to my world. 🎬</p>
  </section>

  <section class="section solo-top">
    <h2>🖤 Solo Leveling Specials</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/6yTLr8svbWY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/BPWy1hlL_VQ" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/IwmIkEqs0PQ" allowfullscreen></iframe>
    </div>
    <!-- Added image to Solo Leveling Specials -->
    <img src="https://static.wikia.nocookie.net/jujutsu-kaisen/images/f/f5/Satoru_quotes_I_alone_am_the_honored_one_%28Anime%29.png/revision/latest?cb=20230727233257" alt="Solo Leveling Image" style="width:100%; max-height: 400px; object-fit: cover;">
  </section>

  <section class="section jjk-top">
    <h2>🔥 Jujutsu Kaisen Edits</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/zrDeEYCEdtE" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/yODg7agTcCM" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/tLoCvvrlLEY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/cH4AljUsn_E" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/F6dkzIj6Aq4" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/QAoZ6YEMCxo" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/7PyY6LsdNdk" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/T2KcxkACh7g" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/6ck9xQPF878" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/0KV9jrKICpQ" allowfullscreen></iframe>
    </div>
  </section>

  <section class="section demonslayer-top">
    <h2>🔥 Demon Slayer Specials</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/XzE22l_nBOI" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/11DXYkh_i5A" allowfullscreen></iframe>
      <!-- Added new video for Demon Slayer -->
      <iframe src="https://www.youtube.com/embed/kp8VxT8rLVc" allowfullscreen></iframe>
    </div>
  </section>

  <section class="section trollface-top">
    <h2>🤡 Trollface / Skull Editz</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/zrDeEYCEdtE" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/IwmIkEqs0PQ" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/F6dkzIj6Aq4" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/QAoZ6YEMCxo" allowfullscreen></iframe>
    </div>
  </section>

  <section id="videos" class="section videos">
    <h2>🎥 All Shorts</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/zrDeEYCEdtE" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/yODg7agTcCM" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/tLoCvvrlLEY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/cH4AljUsn_E" allowfullscreen></iframe>
    </div>
  </section>

  <section id="contact" class="section contact">
    <h2>📲 Connect With Me</h2>
    <p>
      🔗 <a href="https://www.youtube.com/@Zorem_Editz/shorts" target="_blank">YouTube</a><br>
      📧 Email: <a href="mailto:zorem.editz@gmail.com">zorem.editz@gmail.com</a><br>
      📸 Instagram: <a href="https://www.instagram.com/Zorem_Editz">Zorem_Editz</a><br>
      📘 Facebook: <a href="https://www.facebook.com/bipinchaulagain28">बिपिन चौलागाईं</a>
    </p>
  </section>

  <div class="footer">
    <p>© 2025 Zorem Editz. All rights reserved.</p>
  </div>

  <button id="scrollTopBtn" onclick="scrollToTop()">↑</button>

  <script>
    function toggleMenu() {
      var menu = document.getElementById('dotMenu');
      menu.style.display = menu.style.display === 'flex' ? 'none' : 'flex';
    }

    window.onscroll = function() {
      var scrollBtn = document.getElementById("scrollTopBtn");
      if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
        scrollBtn.style.display = "block";
      } else {
        scrollBtn.style.display = "none";
      }
    };

    function scrollToTop() {
      window.scrollTo({top: 0, behavior: 'smooth'});
    }

    window.onload = function() {
      setTimeout(function() {
        document.getElementById("loading").style.display = "none";
      }, 3000);
    };
  </script>

</body>
</html>
