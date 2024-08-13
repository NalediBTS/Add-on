<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Add-onProject</title>
    <style>
      body {
        background: #fbd0f5;
      }
      h1,
      h2 {
        text-align: center;
      }
      img {
        max-width: 100%;
      }
      p {
        font-size: 18px;
        line-height: 1.5;
      }
      button {
        font-size: 18px;
        border-radius: 30px;
        padding: 16px 21px;
        border: 1px solid #8c5ba3;
        box-shadow: rgba(37, 39, 89, 0.08) 0px 8px 8px 0;
        transition: all 200ms ease-in-out;
        display: block;
        margin: 20px auto;
        background: #8c5ba3;
        color: #fff;
      }
      button:hover {
        background: white;
        color: #8c5ba3;
        cursor: pointer;
        border: 1px solid #8c5ba3;
      }
      footer {
        text-align: center;
        margin: 10px 0;
        font-size: 18px;
      }
      .devide {
        max-width: 600px;
        margin: 20px auto;
        background: white;
        padding: 20px;
        border-radius: 10px;
      }
      .theme-button {
        border-radius: 25px;
        margin: 0 auto;
        display: block;
        background: #c20ac8;
        border: 1px solid #c20ac8;
        color: white;
        font-size: 16px;
        line-height: 22px;
        padding: 16px 24px;
        text-decoration: none;
        transition: all 200ms ease;
      }
      .theme-button:hover {
        color: #c20ac8;
        background: #fff;
        cursor: pointer;
      }
      .intro {
        border-radius: 10px;
        transition: all 150ms ease-in-out;
        max-width: 100%;
      }
      .intro:hover {
        filter: contrast(100%);
        transform: scale(1.5, 1.5);
      }
      .grid {
        margin: 15px 0;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-gap: 15px;
      }
      .grid img {
        width: 100%;
        border-radius: 8px;
        aspect-ratio: 3/2;
        transition: all 200ms ease-in-out;
      }
      .grid img:hover {
        transform: scale(1.5, 1.5);
      }
      .dark {
        background: black;
        color: white;
      }
      .dark .devide {
        background: rgba(255, 255, 255, 0.1);
      }
      .dark a {
        color: #fbd0f5;
      }
      .dark button {
        background: white;
        color: black;
        border: 1px solid white;
      }
      .dark button:hover {
        background: black;
        color: white;
        border: 1px solid white;
      }
      .dark h1,
      .dark h2,
      .dark p {
        color: white;
      }
      .info {
        font-size: 18px;
        text-decoration: none;
        color: #8c5ba3;
      }

      .info:hover {
        text-decoration: underline;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <button id="theme-button" class="theme-button">Change Theme🖤</button>
    <div class="devide">
      <h1>🎶 K-pop</h1>
      <h2>My favourite music genre</h2>
      <a
        id="link"
        href="https://kpopping.com/profiles/the-groups"
        target="_blank"
      >
        <img
          src="https://www.allkpop.com/upload/2022/08/content/181531/web_data/allkpop_1660851640_allkpop-1648756491-untitled-1.jpg"
          alt="KPOP"
          class="intro"
        />
      </a>
      <div class="grid">
        <img
          src="https://i.ytimg.com/vi/hLfItPNreoI/maxresdefault.jpg"
          alt="playlist"
        />
        <img
          src="https://i0.wp.com/ononestudios.com/wp-content/uploads/2022/06/maxresdefault.jpg?fit=1024%2C576&ssl=1"
          alt="dance"
        />
        <img
          src="https://storage.googleapis.com/koreaboo-cdn/255163146_267840595307017_7831446373936276564_n.jpg"
          alt="singing"
        />
        <img
          src="https://i.ytimg.com/vi/mr0Oq_OiR8Y/sddefault.jpg?v=66710011"
          alt="challenge"
        />
      </div>
      <p>
        K-pop, the sparkling gem of South Korea, is a colorful whirlwind of
        catchy melodies, stunning choreography, and endless charm. It’s a global
        sensation that brings people together with its infectious tunes and
        vibrant performances. From cute concepts to powerful anthems, K-pop is a
        musical rainbow that brightens up the world. 🎵🌈😊
      </p>
      <a
        class="info"
        href="https://en.wikipedia.org/wiki/K-pop"
        target="_blank"
      >
        Find out more on Wikipedia🤓</a
      >
      <br />
      <br />
      <button id="kpop-button">Listen to K-POP💗</button>
    </div>
    <footer>
      Coded by
      <a
        href="https://linkedin.com/in/nakedi-makgakga-33a64a273"
        target="_blank"
      >
        Nakedi Makgakga👩‍💻</a
      >
    </footer>
    <script>
      function changeTheme() {
        let body = document.querySelector("body");
        body.classList.toggle("dark");
      }

      let themeButton = document.querySelector("#theme-button");
      themeButton.addEventListener("click", changeTheme);

      let kpopButton = document.querySelector("#kpop-button");
      kpopButton.addEventListener("click", function () {
        let name = prompt("What is your name?");
        let isFan = confirm("Are you a K-pop fan?");
        if (isFan) {
          alert("Welcome to a colourful world, " + name + "☺❤");
        } else {
          alert(
            "That's okay, " + name + ". Enjoy exploring the world of K-pop!"
          );
        }
      });
    </script>
  </body>
</html>

