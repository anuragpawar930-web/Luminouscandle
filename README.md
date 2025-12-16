<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Luminious Candle</title>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: #faf7f2;
  color: #333;
}

header {
  background: linear-gradient(to right, #e6d3b3, #f3eadc);
  text-align: center;
  padding: 80px 20px;
}

header h1 {
  font-size: 42px;
  margin-bottom: 10px;
}

header p {
  font-size: 18px;
}

.buttons a {
  display: inline-block;
  margin: 10px;
  padding: 12px 22px;
  text-decoration: none;
  color: white;
  border-radius: 6px;
  font-weight: bold;
}

.shop {
  background: #5a3e2b;
}

.whatsapp {
  background: #25D366;
}

.instagram {
  background: #C13584;
}

section {
  padding: 60px 20px;
  max-width: 1100px;
  margin: auto;
}

section h2 {
  text-align: center;
  margin-bottom: 30px;
}

.products {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 25px;
}

.product {
  background: white;
  border-radius: 12px;
  padding: 20px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  text-align: center;
}

.product img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: 10px;
}

.product h3 {
  margin: 15px 0 5px;
}

.price {
  font-size: 18px;
  font-weight: bold;
}

.product a, .product button {
  display: block;
  margin-top: 10px;
  padding: 10px;
  border-radius: 5px;
  border: none;
  cursor: pointer;
  text-decoration: none;
  color: white;
  font-weight: bold;
}

.buy {
  background: #5a3e2b;
}

footer {
  background: #5a3e2b;
  color: white;
  text-align: center;
  padding: 20px;
}

/* Floating WhatsApp */
.whatsapp-float {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: #25D366;
  color: white;
  padding: 15px;
  border-radius: 50%;
  font-size: 22px;
  text-decoration: none;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
}
</style>
</head>

<body>

<header>
  <h1>Luminious Candle</h1>
  <p>Hand-poured candles made to light your moments</p>

  <div class="buttons">
    <a href="#shop" class="shop">Shop Now</a>
    <a href="https://wa.me/919307708258" class="whatsapp">Order on WhatsApp</a>
    <a href="https://instagram.com/luminiouscancle09" class="instagram">DM on Instagram</a>
  </div>
</header>

<section id="about">
  <h2>About Us</h2>
  <p style="text-align:center;">
    Luminious Candle is a handcrafted candle brand created with love and care.
    Each candle is made using quality wax, soothing fragrances, and attention to detail.
    Our mission is to bring warmth, calm, and beauty into your everyday moments.
  </p>
</section>

<section id="shop">
  <h2>Our Candles</h2>

  <div class="products">

    <div class="product">
      <img src="https://images.unsplash.com/photo-1603006905003-be475563bc59" alt="Vanilla Bliss">
      <h3>Vanilla Bliss</h3>
      <p>Sweet vanilla fragrance</p>
      <p class="price">₹499</p>
      <a href="PASTE_RAZORPAY_LINK_HERE" class="buy">Buy Now</a>
      <button class="whatsapp" onclick="orderWhatsApp('Vanilla Bliss')">Order on WhatsApp</button>
    </div>

    <div class="product">
      <img src="https://images.unsplash.com/photo-1589987607627-616cac8d7d45" alt="Lavender Calm">
      <h3>Lavender Calm</h3>
      <p>Relaxing lavender scent</p>
      <p class="price">₹549</p>
      <a href="PASTE_RAZORPAY_LINK_HERE" class="buy">Buy Now</a>
      <button class="whatsapp" onclick="orderWhatsApp('Lavender Calm')">Order on WhatsApp</button>
    </div>

    <div class="product">
      <img src="https://images.unsplash.com/photo-1616627983796-4a3dc0c39fce" alt="Rose Elegance">
      <h3>Rose Elegance</h3>
      <p>Soft floral rose aroma</p>
      <p class="price">₹599</p>
      <a href="PASTE_RAZORPAY_LINK_HERE" class="buy">Buy Now</a>
      <button class="whatsapp" onclick="orderWhatsApp('Rose Elegance')">Order on WhatsApp</button>
    </div>

  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <p style="text-align:center;">
    📧 luminiouscandle@gmail.com <br>
    📱 WhatsApp: 9307708258 <br>
    📸 Instagram: @luminiouscancle09
  </p>
</section>

<footer>
  © 2025 Luminious Candle. All rights reserved.
</footer>

<a class="whatsapp-float" href="https://wa.me/919307708258">💬</a>

<script>
function orderWhatsApp(productName) {
  const message = `Hi, I want to order the ${productName} candle from Luminious Candle.`;
  const url = `https://wa.me/919307708258?text=${encodeURIComponent(message)}`;
  window.open(url, "_blank");
}
</script>

</body>
</html>

