<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HeyHitsGames - Gaming Hub</title>
  <style>
    /* Reset and basics */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: #0d0d0d;
      color: #f5f5f5;
      line-height: 1.6;
    }

    header {
      background-color: #1a1a1a;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      font-size: 2rem;
      color: #00ffcc;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 1rem;
    }

    nav a {
      color: #f5f5f5;
      text-decoration: none;
      font-size: 1rem;
      transition: color 0.3s, transform 0.3s;
    }

    nav a::after {
      content: '';
      display: block;
      width: 0;
      height: 2px;
      background: #00ffcc;
      transition: width 0.3s;
      margin-top: 5px;
    }

    nav a:hover {
      color: #00ffcc;
      transform: translateY(-2px);
    }

    nav a:hover::after {
      width: 100%;
    }

    /* Hero section */
    .hero {
      text-align: center;
      padding: 6rem 2rem;
      background: linear-gradient(135deg, #1f1c2c, #928dab);
    }

    .hero h2 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 2rem;
    }

    .btn {
      background: #00ffcc;
      color: #0d0d0d;
      padding: 0.8rem 1.5rem;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #00cc99;
    }

    /* Emoji Animation */
    .emoji-animation {
      font-size: 4rem;
      animation: bounce 2s infinite;
    }

    @keyframes bounce {
      0%, 100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(-20px);
      }
    }

    /* Sections styles */
    section {
      padding: 4rem 2rem;
    }

    .latest-news, .about-me, .community-section, .games-section, footer {
      background: #161616;
    }

    .community-section, .games-section {
      background: #1a1a1a;
    }

    .community-card, .game-card {
      background: #222;
      padding: 2rem;
      border-radius: 10px;
      text-align: center;
      transition: transform 0.3s;
    }

    .community-card i, .game-card img {
      margin-bottom: 1rem;
      width: 100%;
      border-radius: 10px;
    }

    .community-card:hover, .game-card:hover {
      transform: scale(1.05);
    }

    .community-cards, .game-list {
      display: grid;
      gap: 2rem;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      margin-top: 2rem;
    }

    /* Footer Section */
    footer {
      padding: 2rem;
      text-align: center;
      font-size: 0.9rem;
      background: #111;
    }

    .social-links a {
      color: #f5f5f5;
      margin: 0 0.5rem;
      font-size: 1.5rem;
      transition: color 0.3s;
    }

    .social-links a:hover {
      color: #00ffcc;
    }

    /* About Me Section */
    .about-me img {
      border-radius: 50%;
      width: 150px;
      height: 150px;
      margin-bottom: 1rem;
    }

    .about-me p {
      max-width: 600px;
      margin: 0 auto;
      font-size: 1.2rem;
    }

    /* Description Section */
    .Description div {
      background: #222;
      padding: 1.5rem;
      border-radius: 10px;
      margin-bottom: 1.5rem;
    }

    .Description h3 {
      margin-bottom: 0.8rem;
      font-size: 1.6rem;
    }

    .Description p {
      font-size: 1rem;
    }
  </style>

  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

  <header>
    <h1>HeyHitsGames</h1>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#games">Games</a></li>
        <li><a href="#Description">Description</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <div class="emoji-animation">🎮</div>
    <h2>Welcome to HeyHitsGames</h2>
    <p>Your ultimate destination for gaming description, recommendations, reviews, and community!</p>
    <button class="btn">Explore Now</button>
  </section>

  <section id="Description">
    <h2>Games Description</h2>
    <div class="emoji-animation">🎮</div>
    <div class="Description">
      <div>
        <h3>Resident Evil 8 Village</h3>
        <p>Resident Evil Village is a 2021 survival horror game developed and published by Capcom. Players control Ethan Winters, who searches for his kidnapped daughter in a mysterious village filled with mutant creatures.</p>
      </div>
      <div>
        <h3>The Last of Us Part II</h3>
        <p>The Last of Us Part II is a 2020 action-adventure game developed by Naughty Dog. The game focuses on two playable characters: Ellie, who seeks revenge for a murder, and Abby, involved in a conflict between her militia and a cult.</p>
      </div>
      <div>
        <h3>God of War</h3>
        <p>God of War is an action-adventure game following Kratos, a Spartan warrior who becomes the God of War, battling mythological creatures from different pantheons.</p>
      </div>
      <div>
        <h3>Devil May Cry 5</h3>
        <p>Devil May Cry 5 follows Nero and Dante as they battle the Demon King Urizen. Players control each character with distinct playstyles and abilities.</p>
      </div>
    </div>
  </section>

  <section id="about" class="about-me">
    <img src="https://scontent.fmnl30-1.fna.fbcdn.net/v/t39.30808-6/475887591_1161059292347188_5525287589594889373_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=a5f93a&_nc_eui2=AeEFmp2DZsIvf4MBzOD1SFuc-CVbYQTBlFX4JVthBMGUVa9ZkeNaoaklpCgDaY1T7-F9VEOUpGFj25gemd4nujSY&_nc_ohc=xSkYzVjJT64Q7kNvwGk1Trs&_nc_oc=AdlDCzVQ6ZFx6jmQIbh3hmMQMRrQIFkS4Mu4XTlDscd_WNyn-nHv8azAN_KziqYTlTQ&_nc_zt=23&_nc_ht=scontent.fmnl30-1.fna&_nc_gid=khq2hYNrRVF8SWaPHj9MgQ&oh=00_AfGuRHjacXIGI-NDhpY1fgeF8SIxiTWf1O0P4QjzzT8BwQ&oe=67FCD37C" alt="Profile Picture">
    <h2>About Me</h2>
    <div class="emoji-animation">🌷</div>
    <p>Hey there! I'm <strong>Lee</strong>, and this is my website about Games and there description and that's why I create this Portfolio is give insights for those who would like to play my recommendations games in this portfolio and that's all of my introduction Thank You so Much for Visiting my Portfolio!!</p>
  </section>

  <section id="games" class="games-section">
    <h2>Featured Games</h2>
    <div class="game-list">
      <div class="game-card">
        <img src="https://c4.wallpaperflare.com/wallpaper/780/420/942/resident-evil-8-village-resident-evil-video-games-chris-redfield-artwork-hd-wallpaper-preview.jpg" alt="Resident Evil 8 Village">
        <h3>Resident Evil 8 Village</h3>
      </div>
      <div class="game-card">
        <img src="https://images6.alphacoders.com/130/thumb-440-1305433.webp" alt="The Last of Us Part II">
        <h3>The Last of Us Part II</h3>
      </div>
      <div class="game-card">
        <img src="https://images7.alphacoders.com/413/thumb-440-413551.webp" alt="God of War">
        <h3>God of War</h3>
      </div>
      <div class="game-card">
        <img src="https://images6.alphacoders.com/926/926723.jpg" alt="Devil May Cry 5">
        <h3>Devil May Cry 5</h3>
      </div>
    </div>
  </section>

  <section id="contact" class="contact-section">
    <footer>
      &copy; 2025 HeyHitsGames. All rights reserved.
      <div class="social-links">
        <a href="https://facebook.com" target="_blank"><i class="fab fa-facebook"></i></a>
        <a href="https://twitter.com" target="_blank"><i class="fab fa-twitter"></i></a>
        <a href="https://instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://youtube.com" target="_blank"><i class="fab fa-youtube"></i></a>
      </div>
    </footer>
  </section>

</body>
</html>
