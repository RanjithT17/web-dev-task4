<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>Ranjith OTT - The New OTT</title>
    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/clappr@latest/dist/clappr.min.js"></script>

    <style>
      .flex-container {
        padding: 0;
        margin: 0;
        list-style: none;
        display: -webkit-box;
        display: -moz-box;
        display: -ms-flexbox;
        display: -webkit-flex;
        display: flex;
        -webkit-flex-flow: row wrap;
        justify-content: space-around;
      }
      .flex-item {
        background: tomato;
        padding: 5px;
        width: 640px;
        height: 360px;
        margin-top: 10px;
        line-height: 150px;
        color: white;
        font-weight: bold;
        font-size: 3em;
        text-align: center;
      }
      .title {
        font-color: white;
        color: darkorange;
        font-size: xxx-large;
        text-align: center;
        text-transform: full-width;
        font-weight: lighter;
      }

      .subtitle {
        font-color: white;
        color: dimgray;
        font-size: larger;
        text-align: center;
        text-transform: full-width;
        font-weight: lighter;
      }
      .notstealenfromnetflix {
        background-color: #141414
      }
footer {
    background-color: #333;
    color: white; /* Set text color to white */
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}

footer p {
    color: white; /* Set text color to white */
}
header {
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }

        header input[type="text"] {
            padding: 5px;
            width: 200px;
        }

        header button {
            padding: 5px 10px;
            background-color: darkorange;
            color: white;
            border: none;
            cursor: pointer;
        }
    </style>
  </head>
  <body class="notstealenfromnetflix">
  <header>
    <h1 class="title">OTT Platform - The New Cinema World</h1>
    <h2 class="subtitle">Using IA, blockchain, ML, VR, IoT to show you colorbar and bunnies</h2>
    <input type="text" placeholder="Search movies..." />
    <button>Search</button>
</header>
    <ul class="flex-container">
      <li class="flex-item">
        <div id="player"></div>
      </li>
      <li class="flex-item">
        <div id="player1"></div>
      </li>
    </ul>

    <script>
      var player = new Clappr.Player(
        {
          source: "http://localhost:8080/hls/colorbar.m3u8?token=token",
          parentId: "#player",
          poster: 'https://cdn11.bigcommerce.com/s-yzgoj/images/stencil/1280x1280/products/2910923/5971657/MOVAB75711__13699.1679612834.jpg?c=2',
          mute: true,
          height: 360,
          width: 640,
        });
      var player1 = new Clappr.Player(
        {
          source: "https://test-streams.mux.dev/x36xhzz/x36xhzz.m3u8",
          parentId: "#player1",
          poster: 'https://c4.wallpaperflare.com/wallpaper/743/1018/523/interstellar-2014-wallpaper-preview.jpg',
          mute: true,
          height: 360,
          width: 640,
        });
    </script>
<footer>
      <p>&copy; 2024 Ranjith OTT Platform.All rights reserved.</p>
</footer>
  </body>
</html>
