
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rohit Sharma | The Hitman</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background: #080d19;
      color: white;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 22px 8%;
      background: #0d1425;
      border-bottom: 1px solid #25314b;
    }

    .logo {
      font-size: 24px;
      font-weight: bold;
      color: #ff6333;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 22px;
      font-size: 14px;
    }

    nav a:hover {
      color: #ff6333;
    }

    .hero {
      min-height: 85vh;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 35px;
      padding: 60px 8%;
      background:
        radial-gradient(circle at 80% 40%, #183d68 0, transparent 45%),
        #080d19;
    }

    .hero-content {
      max-width: 580px;
    }

    .tag {
      color: #ff6333;
      font-weight: bold;
      letter-spacing: 4px;
      margin-bottom: 20px;
    }

    h1 {
      font-size: clamp(45px, 7vw, 85px);
      line-height: 1;
      margin-bottom: 22px;
    }

    h1 span {
      color: #ff6333;
    }

    .hero p {
      color: #bac4d8;
      line-height: 1.8;
      margin-bottom: 28px;
    }

    .btn {
      display: inline-block;
      padding: 14px 25px;
      border-radius: 6px;
      background: #ff6333;
      color: white;
      text-decoration: none;
      font-weight: bold;
      border: none;
      cursor: pointer;
    }

    .btn:hover {
      background: #e84b1c;
      transform: translateY(-2px);
    }

    .player-image {
      width: min(40%, 380px);
      min-width: 220px;
      aspect-ratio: 3 / 4;
      object-fit: cover;
      object-position: center;
      border-radius: 20px;
      border: 2px solid #ff6333;
      box-shadow: 0 0 50px #ff633344;
    }

    section {
      padding: 75px 8%;
    }

    .section-title {
      text-align: center;
      font-size: 36px;
      margin-bottom: 40px;
    }

    .section-title span {
      color: #ff6333;
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .card {
      background: #111b2e;
      border: 1px solid #273650;
      padding: 28px 15px;
      text-align: center;
      border-radius: 12px;
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-7px);
      border-color: #ff6333;
    }

    .card h3 {
      font-size: 32px;
      color: #ff6333;
      margin-bottom: 12px;
    }

    .card p {
      color: #bac4d8;
    }

    .about {
      text-align: center;
      background: #0d1425;
    }

    .about p {
      max-width: 750px;
      margin: auto;
      color: #bac4d8;
      line-height: 1.9;
    }

    footer {
      text-align: center;
      padding: 25px;
      background: #060a12;
      color: #9aa7bd;
    }

    footer span {
      color: #ff6333;
    }

    @media (max-width: 768px) {
      header {
        flex-direction: column;
        gap: 18px;
      }

      nav a {
        margin: 0 7px;
      }

      .hero {
        flex-direction: column;
        text-align: center;
      }

      .player-image {
        width: 80%;
        max-width: 320px;
      }

      .stats {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 380px) {
      nav a {
        font-size: 12px;
        margin: 0 4px;
      }

      .stats {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">HITMAN.</div>

    <nav>
      <a href="#home">Home</a>
      <a href="#records">Records</a>
      <a href="#about">About</a>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="hero-content">
        <div class="tag">INDIAN CRICKET STAR</div>

        <h1>ROHIT<br><span>SHARMA</span></h1>

        <p>
          The Hitman of Indian Cricket.
          A leader, a match winner, and one of the most
          entertaining batters in the game.
        </p>

        <a href="#records" class="btn">EXPLORE RECORDS ↗</a>
      </div>

      <img
        class="player-image"
        src="https://placehold.co/600x800/111b2e/ff6333?text=ROHIT+SHARMA"
        alt="Rohit Sharma placeholder image"
      >
    </section>

    <section id="records">
      <h2 class="section-title">CAREER <span>HIGHLIGHTS</span></h2>

      <div class="stats">
        <div class="card">
          <h3>3</h3>
          <p>ODI Double Centuries</p>
        </div>

        <div class="card">
          <h3>264</h3>
          <p>Highest ODI Score</p>
        </div>

        <div class="card">
          <h3>5</h3>
          <p>IPL Titles as Captain</p>
        </div>

        <div class="card">
          <h3>2024</h3>
          <p>T20 World Cup Champion</p>
        </div>
      </div>
    </section>

    <section class="about" id="about">
      <h2 class="section-title">ABOUT <span>HITMAN</span></h2>

      <p>
        Rohit Sharma is an Indian international cricketer known
        for his elegant batting, powerful sixes and leadership.
        He has created many memorable moments in international
        cricket and is admired by fans around the world.
      </p>

      <br><br>

      <button class="btn" onclick="showMessage()">
        HITMAN FAN CLUB ❤️
      </button>

      <p id="message" style="margin-top:20px;"></p>
    </section>
  </main>

  <footer>
    <p>Made with ❤️ by <span>Aditya Singh</span></p>
    <p>Fan-made website • Not an official Rohit Sharma website</p>
  </footer>

  <script>
    function showMessage() {
      document.getElementById("message").textContent =
        "Thank you for supporting Rohit Sharma! 🏏";
    }
  </script>

</body>
</html>
