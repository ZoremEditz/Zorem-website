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

    /* Three Dot Menu */
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
      📧 Email: <a href="mailto:zorem.editz@gmail.com">zorem.editz@gmail.com</a>
    </p>
  </section>

  <!-- Footer -->
  <div class="footer">
    <p>© 2025 Zorem Editz. All rights reserved.</p>
  </div>

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
