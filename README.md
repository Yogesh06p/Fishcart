# Fishcart
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>FISH - Fresh Fish Delivery</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f7f7f7; }
    header { background: #000; color: #fff; padding: 20px; text-align: center; }
    .logo { font-size: 2em; font-weight: bold; letter-spacing: 2px; }
    nav { background: #333; color: #fff; padding: 10px; text-align: center; }
    nav a { color: white; margin: 0 15px; text-decoration: none; font-weight: bold; }
    .section { padding: 20px; }
    .fish-item { background: #fff; margin: 10px 0; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
    .fish-item img { width: 100px; float: left; margin-right: 20px; }
    .btn { display: inline-block; padding: 10px 15px; background: #28a745; color: white; border-radius: 5px; text-decoration: none; margin-top: 10px; }
    footer { background: #222; color: #fff; text-align: center; padding: 15px; margin-top: 20px; }
    .clearfix::after { content: ""; clear: both; display: table; }
  </style>
</head>
<body>

<header>
  <div class="logo">FISH</div>
  <p>Fresh Local Fish Delivered Daily</p>
</header>

<nav>
  <a href="#menu">Fish Menu</a>
  <a href="#about">About</a>
  <a href="#contact">Contact</a>
</nav>

<div class="section" id="menu">
  <h2>Fish Menu</h2>

  <div class="fish-item clearfix">
    <img src="https://via.placeholder.com/100" alt="Surmai" />
    <h3>Surmai</h3>
    <p>₹800 / kg</p>
    <a class="btn" href="https://wa.me/919999999999">Order on WhatsApp</a>
  </div>

  <div class="fish-item clearfix">
    <img src="https://via.placeholder.com/100" alt="Bangda" />
    <h3>Bangda</h3>
    <p>₹300 / kg</p>
    <a class="btn" href="https://wa.me/919999999999">Order on WhatsApp</a>
  </div>

  <div class="fish-item clearfix">
    <img src="https://via.placeholder.com/100" alt="Kolambi" />
    <h3>Kolambi</h3>
    <p>₹600 / kg</p>
    <a class="btn" href="https://wa.me/919999999999">Order on WhatsApp</a>
  </div>

  <div class="fish-item clearfix">
    <img src="https://via.placeholder.com/100" alt="Bombil" />
    <h3>Bombil</h3>
    <p>₹250 / kg</p>
    <a class="btn" href="https://wa.me/919999999999">Order on WhatsApp</a>
  </div>
</div>

<div class="section" id="about">
  <h2>About Us</h2>
  <p>We deliver the freshest fish daily across Mumbai & Navi Mumbai. Cleaned, packed, and handled with hygiene – straight from the dock to your home!</p>
</div>

<div class="section" id="contact">
  <h2>Contact</h2>
  <p>Call / WhatsApp: +91 99999 99999</p>
  <p>Delivery in: Mumbai, Navi Mumbai</p>
</div>

<footer>
  &copy; 2025 FISH - Fresh Local Fish Delivery
</footer>

</body>
</html>
