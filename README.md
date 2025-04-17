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
      background-image: url('https://4kwallpapers.com/wp-content/uploads/2022/04/sung-jinwoo-dragon-15351.jpg'); /* New Anime Wallpaper */
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      color: white;
      overflow-x: hidden;
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.7);
      padding: 15px 20px;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.7);
    }

    header nav {
      display: flex;
      justify-content: space-around;
      align-items: center;
    }

    header nav a {
      color: white;
      text-decoration: none;
      padding: 10px;
      font-size: 18px;
    }

    header nav a:hover {
      background-color: #ff4c98;
      border-radius: 5px;
    }

    header h1 {
      margin: 0;
      font-size: 3rem;
      z-index: 2;
      position: relative;
      text-align: center;
    }

    .parallax {
      background: url('https://wallpapercave.com/wp/wp1912061.jpg') no-repeat center center fixed;
      background-size: cover;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      font-size: 2.5rem;
      padding: 20px;
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

    /* Scroll to Top */
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

  <audio autoplay loop hidden>
    <source src="https://files.catbox.moe/8mlghm.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <!-- Navbar -->
  <header>
    <nav>
      <a href="#about">About</a>
      <a href="#featured">Featured</a>
      <a href="#videos">All Shorts</a>
      <a href="#contact">Contact</a>
    </nav>
    <h1>Zorem Editz</h1>
  </header>

  <!-- Parallax Section -->
  <div class="parallax">
    <h2>Welcome to Zorem Editz</h2>
    <p>Your go-to place for epic anime edits!</p>
  </div>

  <!-- About Section -->
  <section id="about" class="section about">
    <h2>👋 About Me</h2>
    <p>Yo! I'm Zorem Editz – a passionate content creator who loves anime and brings epic moments to life through edits. I post fire YouTube Shorts on anime like Jujutsu Kaisen, Solo Leveling, Naruto, and more! Whether you're here to vibe or get hyped, welcome to my world. 🎬</p>
  </section>

  <!-- Featured Section -->
  <section id="featured" class="section featured">
    <h2>🌟 Featured Edit of the Week</h2>
    <iframe src="https://www.youtube.com/embed/IwmIkEqs0PQ" title="Featured Edit" allowfullscreen></iframe>
  </section>

  <!-- Solo Leveling Section -->
  <section class="section solo-top">
    <h2>🖤 Solo Leveling Specials</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/6yTLr8svbWY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/BPWy1hlL_VQ" allowfullscreen></iframe>
    </div>
  </section>

  <!-- All Shorts Section -->
  <section id="videos" class="section videos">
    <h2>🎥 All Shorts</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/zrDeEYCEdtE" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/yODg7agTcCM" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/tLoCvvrlLEY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/cH4AljUsn_E" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/6yTLr8svbWY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/BPWy1hlL_VQ" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/F6dkzIj6Aq4" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/QAoZ6YEMCxo" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/7PyY6LsdNdk" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/T2KcxkACh7g" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/6ck9xQPF878" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/0KV9jrKICpQ" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/kp8VxT8rLVc" allowfullscreen></iframe>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section contact">
    <h2>📲 Connect With Me</h2>
    <p>
      🔗 <a href="https://www.youtube.com/@Zorem_Editz/shorts" target="_blank">YouTube</a><br>
      📧 Email: <a href="mailto:bipinchaulagain28@gmail.com">bipinchaulagain28@gmail.com</a><br>
      📸 Instagram: <a href="https://www.instagram.com/Zorem_Editz" target="_blank">@Zorem_Editz</a><br>
      📘 Facebook: <a href="https://www.facebook.com/bipin.chaulagain.98" target="_blank">बिपिन चौलागाईं</a><br>
      🎮 MLBB ID: 1158448185 (13690)<br>
      🎮 Free Fire ID: 644596611
    </p>
  </section>

  <div class="footer">
    <p>© 2025 Zorem Editz. All rights reserved.</p>
    <p>Subscribe to reach 1k Army!</p>
  </div>

  <button id="scrollTopBtn" onclick="window.scrollTo({top: 0, behavior: 'smooth'});">⬆️</button>

  <script>
    const scrollBtn = document.getElementById('scrollTopBtn');
    window.onscroll = function () {
      scrollBtn.style.display = (window.scrollY > 400) ? 'block' : 'none';
    }
  </script>

</body
