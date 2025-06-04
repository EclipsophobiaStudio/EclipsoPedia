<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Eclipsophobia Studio</title>
  <style>
    body {
      font-family: "Courier New", monospace;
      background-color: #000000;
      color: #e0e0e0;
      margin: 0;
      padding: 0;
      background-image: radial-gradient(circle at center, #1a1a1a 0%, #000000 80%);
    }
    header {
      background-color: #080808;
      padding: 2em 1em;
      text-align: center;
      border-bottom: 1px solid #222;
    }
    h1 {
      font-size: 2.7em;
      text-shadow: 0 0 20px #000000, 0 0 5px #222;
    }
    .eclipsophobia {
      color: #ffd700; /* yellowish like a dying sun */
    }
    .studio {
      color: #3caeff; /* moonlight blue */
    }
    h2 {
      color: #c70000;
      text-shadow: 0 0 5px black;
    }
    section {
      padding: 2em;
    }
    .game-card {
      background: #111111;
      border: 1px solid #2a2a2a;
      padding: 1em;
      margin-bottom: 1em;
      border-radius: 8px;
      box-shadow: 0 0 20px #1a1a1a;
      transition: transform 0.2s ease;
    }
    .game-card:hover {
      transform: scale(1.03);
      background: #191919;
    }
    /* Stil pentru butoanele de personaje */
    .character-button {
      background: #111111;
      border: 1px solid #2a2a2a;
      padding: 0.8em 1.2em;
      margin: 0.5em 0;
      border-radius: 8px;
      width: 100%;
      font-size: 1.1em;
      color: #e0e0e0;
      cursor: pointer;
      box-shadow: 0 0 20px #1a1a1a;
      transition: transform 0.2s ease, background 0.2s ease;
    }
    .character-button:hover {
      transform: scale(1.03);
      background: #191919;
    }
    .character-info {
      background: #0f0f0f;
      padding: 1em;
      margin-top: 0.3em;
      border-radius: 8px;
      display: none;
      border: 1px solid #222;
    }
    footer {
      text-align: center;
      padding: 1em;
      background-color: #080808;
      font-size: 0.8em;
      color: #666;
      border-top: 1px solid #222;
    }
    a {
      color: #ff4c4c;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <header>
    <h1>
      <span class="eclipsophobia">Eclipsophobia</span> <span class="studio">Studio</span>
    </h1>
    <p>Horror Games Under The Eclipse Light.</p>
  </header>

  <section>
    <h2>About The Studio</h2>
    <p>An Indie Horror Game Studio on Roblox prepared to scare you. Our stories are not just games — they are nightmares born under a dying light.</p>
  </section>

  <section>
    <h2>Our Games</h2>
    <div class="game-card">
      <h3>Walking Nightmares</h3>
      <p>Thought phobias don't exist? Think again. You cannot wake up from what was never a dream.</p>
    </div>
  </section>

  <section>
    <h2>Characters</h2>
    
    <button class="character-button" onclick="toggleInfo('chester-info')">Chester</button>
    <div id="chester-info" class="character-info">
      <p>🎪 Join the show! The clown is here! But don’t trust his laugh... it's hiding something rotten.</p>
    </div>
    
    <button class="character-button" onclick="toggleInfo('lucas-info')">Lucas</button>
    <div id="lucas-info" class="character-info">
      <p>👔 The great mayor that everybody loves. Everybody... except Chester. What secrets does he hide?</p>
    </div>
    
    <button class="character-button" onclick="toggleInfo('esther-info')">Esther</button>
    <div id="esther-info" class="character-info">
      <p>🐰 Our favorite bunny from the show! She has a lot of nerve. Maybe too much.</p>
    </div>

    <button class="character-button" onclick="toggleInfo('lila-info')">Lila</button>
    <div id="lila-info" class="character-info">
      <p>🎪 Chesters lover, the jester of the show, Lila! She is warmly and calm. Too Calm...</p>
    </div>
    
  </section>

  <footer>
    &copy; 2025 <span class="eclipsophobia">Eclipsophobia</span> <span class="studio">Studio</span> — All Rights Reserved.
  </footer>

  <script>
    function toggleInfo(id) {
      var infoDiv = document.getElementById(id);
      if(infoDiv.style.display === "none" || infoDiv.style.display === "") {
        infoDiv.style.display = "block";
      } else {
        infoDiv.style.display = "none";
      }
    }
  </script>
  <style>
  body {
    font-family: "Courier New", monospace;
    background-color: #000000;
    color: #e0e0e0;
    margin: 0;
    padding: 0;
    background-image: radial-gradient(circle at center, #1a1a1a 0%, #000000 80%);
  }

  header {
    background-color: #080808;
    padding: 2em 1em;
    text-align: center;
    border-bottom: 1px solid #222;
  }

  h1 {
    font-size: 2.7em;
    text-shadow: 0 0 20px #000000, 0 0 5px #222;
  }

  .eclipsophobia {
    color: #f5d742;
  }

  .studio {
    color: #4287f5;
  }

  section {
    padding: 2em;
    max-width: 1000px;
    margin: auto;
  }

  .card {
    background-color: #111;
    padding: 1em;
    margin: 1em 0;
    border: 1px solid #333;
    border-radius: 10px;
    box-shadow: 0 0 10px #00000088;
    transition: transform 0.2s ease;
  }

  .card:hover {
    transform: scale(1.02);
  }

  /* 📱📱📱 Mobile-friendly magic */
  @media only screen and (max-width: 768px) {
    body {
      font-size: 1em;
    }

    header {
      padding: 1.5em 0.5em;
    }

    h1 {
      font-size: 2em;
    }

    section {
      padding: 1em;
    }

    .card {
      padding: 1em;
      margin: 1em 0;
    }
  }
</style>

</body>
</html>
