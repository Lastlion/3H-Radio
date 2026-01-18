<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Ma Radio</title>

  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#111111">
  <meta name="apple-mobile-web-app-capable" content="yes">

  <link rel="manifest" href="manifest.json">
  <link rel="apple-touch-icon" href="icon.png">

  <style>
    body {
      background: #111;
      color: white;
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 40px;
    }
    h1 {
      margin-bottom: 20px;
    }
    button {
      background: #e91e63;
      border: none;
      color: white;
      padding: 15px 30px;
      font-size: 18px;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background: #ff4081;
    }
  </style>
</head>

<body>

  <h1>🎧 Ma Radio</h1>
  <p>Appuie sur lecture pour écouter</p>

  <button onclick="playRadio()">▶ Écouter la radio</button>

  <audio id="radio" preload="none">
    <!-- ⚠️ METS ICI TON FLUX RADIO HTTPS -->
    <source src="https://TON-FLUX-RADIO-HTTPS/stream" type="audio/mpeg">
  </audio>

  <script>
    function playRadio() {
      const radio = document.getElementById("radio");
      radio.play();
    }
  </script>

</body>
</html>
