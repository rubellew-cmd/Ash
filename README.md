# Ash
Ask Ash on a date
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Ash, Will You Go Out With Me?</title>
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <canvas id="laserCanvas"></canvas>
  <div class="pigeon-container">
    <img src="https://upload.wikimedia.org/wikipedia/commons/0/0b/Feral_Pigeon_1.jpg" alt="Carrier Pigeon" class="pigeon" />
    <div class="message">
      <h1>Hey Ash!</h1>
      <p>Would you like to go out on a date?</p>
      <button onclick="respond('yes')">Yes! 🕺</button>
      <button onclick="respond('no')">Maybe next time... 🕊️</button>
    </div>
  </div>
  <script src="laser.js"></script>
  <script>
    function respond(ans) {
      const msg = ans === 'yes'
        ? "The pigeon carries your 'YES!' into the glittering laser sky 🎉"
        : "The pigeon coos softly, maybe another time 🌙";
      document.querySelector('.message').innerHTML = `<h2>${msg}</h2>`;
    }
  </script>
</body>
</html>
