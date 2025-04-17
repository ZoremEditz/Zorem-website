<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Zorem Editz</title>
  
  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    * {
      scroll-behavior: smooth;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-image: url('https://4kwallpapers.com/images/walls/thumbs_3t/15351.jpg'); /* New Anime Wallpaper */
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      color: white;
      overflow-x: hidden;
      margin: 0;
    }

    /* Loading Screen */
    #loading {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: rgba(0, 0, 0, 0.8);
      z-index: 9999;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      color: white;
      font-size: 2rem;
      font-weight: 600;
      opacity: 1;
      animation: fadeOut 2s ease-out 1s forwards;
    }

    @keyframes fadeOut {
      from {
        opacity: 1;
      }
      to {
        opacity: 0;
        display: none;
      }
    }

    /* Navbar */
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
      justify-content: space-between;
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

    .three-dot-menu {
      display: none;
      flex-direction: column;
      position: absolute;
      top: 50px;
      right: 20px;
      background: rgba(0, 0, 0, 0.8);
      border-radius: 5px;
      padding: 10px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.6);
    }

    .three-dot-menu a {
      color: white;
      padding: 10px;
      font-size: 16px;
      text-decoration: none;
      border-radius: 5px;
      margin: 5px 0;
    }

    .three-dot-menu a:hover {
      background-color: #ff4c98;
    }

    .dot {
      width: 20px;
      height: 20px;
      border-radius: 50%;
      background-color: white;
      cursor: pointer;
      margin: 5px;
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

  <!-- Loading Screen -->
  <div id="loading">
    <p>Loading... Please Wait</p>
    <div class="spinner"></div>
  </div>

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
      <div class="dot" onclick="toggleMenu()"></div>
      <div class="three-dot-menu" id="dotMenu">
        <a href="#about">About</a>
        <a href="#featured">Featured</a>
        <a href="#videos">All Shorts</a>
        <a href="#contact">Contact</a>
      </div>
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
    </p>
  </section>

  <!-- Scroll to Top Button -->
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

    // Hide loading screen after page load
    window.onload = function() {
      setTimeout(function() {
        document.getElementById("loading").style.display = "none";
      }, 3000); // Hide after 3 seconds
    };
  </script>

</body>
</html>

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

    .footer img {
      width: 80px;
      margin-top: 10px;
    }

    .quote {
      font-style: italic;
      margin: 20px 0;
      font-size: 1.1rem;
      color: #ccc;
      text-align: center;
    }

    .animated-text {
      font-size: 2rem;
      text-align: center;
      color: #ff4c98;
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
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

    #loader {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: black;
      z-index: 9999;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .loader-text {
      color: #ff4c98;
      font-size: 2rem;
      animation: fadeIn 1.5s infinite alternate;
    }

    @keyframes fadeIn {
      from { opacity: 0.3; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <div id="loader"><div class="loader-text">Loading Zorem Editz...</div></div>

  <audio autoplay loop hidden>
    <source src="https://files.catbox.moe/8mlghm.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <header>
    <h1>Zorem Editz</h1>
    <p class="animated-text">🔥 Anime Edits | JJK | Solo Leveling | More 🔥</p>
  </header>

  <section class="section about">
    <h2>👋 About Me</h2>
    <p>Yo! I'm Zorem Editz – a passionate content creator who loves anime and brings epic moments to life through edits. I post fire YouTube Shorts on anime like Jujutsu Kaisen, Solo Leveling, Naruto, and more! Whether you're here to vibe or get hyped, welcome to my world. 🎬</p>
  </section>

  <section class="section featured">
    <h2>🌟 Featured Edit of the Week</h2>
    <iframe src="https://www.youtube.com/embed/IwmIkEqs0PQ" title="Featured Edit" allowfullscreen></iframe>
  </section>

  <section class="section solo-top">
    <h2>🖤 Solo Leveling Specials</h2>
    <div class="video-grid">
      <iframe src="https://www.youtube.com/embed/6yTLr8svbWY" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/BPWy1hlL_VQ" allowfullscreen></iframe>
    </div>
  </section>

  <section class="section videos">
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

  <section class="section quotes">
    <h2>📜 Character Quotes</h2>
    <div class="quote">"Those who stand at the top determine what's wrong and what's right." – Gojo Satoru</div>
    <div class="quote">"Arise." – Sung Jin-Woo</div>
    <div class="quote">"Power comes in response to a need, not a desire." – Goku</div>
  </section>

  <section class="section contact">
    <h2>📲 Connect With Me</h2>
    <p>
      🔗 <a href="https://www.youtube.com/@Zorem_Editz/shorts" target="_blank">YouTube</a><br>
      📧 Email: <a href="mailto:zorem.editz@gmail.com">zorem.editz@gmail.com</a>
    </p>
  </section>

  <div class="footer">
    <p>© 2025 Zorem Editz. All rights reserved.</p>
    <p><img src="https://upload.wikimedia.org/wikipedia/commons/b/b8/YouTube_Logo_2017.svg" alt="YouTube Logo"><br>Subscribe! To reach 1k Army 💪</p>
  </div>

  <button id="scrollTopBtn" onclick="window.scrollTo({top: 0, behavior: 'smooth'});">⬆️</button>

  <script>
    const scrollBtn = document.getElementById('scrollTopBtn');
    window.onscroll = function () {
      scrollBtn.style.display = (window.scrollY > 400) ? 'block' : 'none';
    };

    window.addEventListener('load', () => {
      document.getElementById('loader').style.display = 'none';
    });
  </script>
</body>
</html>
