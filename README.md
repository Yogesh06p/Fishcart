<!DOCTYPE html>
<html>
<head>
  <title>Fishcart - Fresh Fish</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4fcff;
      padding: 20px;
      text-align: center;
    }

    h1 {
      color: #0077cc;
    }

    .fish-item {
      margin: 15px 0;
    }

    select, input {
      padding: 8px;
      margin: 10px;
    }

    .btn {
      background-color: #28a745;
      color: white;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 5px;
      display: inline-block;
      margin-top: 15px;
    }
  </style>
</head>
<body>

  <h1>Welcome to Fishcart!</h1>
  <p>Fresh fish delivered to your doorstep.</p>

  <h2>Place Your Order</h2>
  <label for="fish">Fish Type:</label>
  <select id="fish">
    <option value="Surmai">Surmai – ₹800/kg</option>
    <option value="Kolambi">Kolambi – ₹650/kg</option>
    <option value="Bombil">Bombil – ₹200/kg</option>
    <option value="Bangda">Bangda – ₹300/kg</option>
  </select><br>

  <label for="qty">Quantity (kg):</label>
  <input type="number" id="qty" min="1" value="1"><br>

  <a id="orderBtn" class="btn" target="_blank">Order on WhatsApp</a>

  <h2 style="margin-top:40px;">Available Fish</h2>

  <div class="fish-item"><strong>Surmai</strong> – ₹800/kg</div>
  <div class="fish-item"><strong>Kolambi</strong> – ₹650/kg</div>
  <div class="fish-item"><strong>Bombil</strong> – ₹200/kg</div>
  <div class="fish-item"><strong>Bangda</strong> – ₹300/kg</div>

  <script>
    const prices = {
      "Surmai": 800,
      "Kolambi": 650,
      "Bombil": 200,
      "Bangda": 300
    };

    document.getElementById("orderBtn").addEventListener("click", function () {
      const fish = document.getElementById("fish").value;
      const qty = parseFloat(document.getElementById("qty").value);
      const price = prices[fish];
      const total = price * qty;
      const message = `Hello, I would like to order ${qty} kg of ${fish}. Total price will be ₹${total}.`;
      const whatsappURL = `https://wa.me/919664239863?text=${encodeURIComponent(message)}`;
      this.href = whatsappURL;
    });
  </script>

</body>
</html>
