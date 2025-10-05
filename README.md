<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Your Shop Name</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body, html { height: 100%; font-family: 'Segoe UI', sans-serif; color: #fff; }

    /* Navigation / header bar */
    .navbar {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      z-index: 10;
    }
    .navbar .logo {
      font-size: 1.5rem;
      font-weight: bold;
      color: #f5f5f5;
    }
    .navbar .menu {
      display: flex;
      gap: 1.5rem;
    }
    .navbar .menu a {
      color: #f5f5f5;
      text-decoration: none;
      font-weight: 500;
    }
    .navbar .menu a:hover {
      text-decoration: underline;
    }

    /* Hero / banner section */
    .hero {
      position: relative;
      height: 70vh;
      min-height: 400px;
      background: url('hero-image.jpg') center center / cover no-repeat;
    }
    .hero::after {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(106,13,173, 0.6); /* purple overlay with transparency */
    }
    .hero-content {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      padding: 0 1rem;
    }
    .hero-content h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    .hero-content p {
      font-size: 1.2rem;
      margin-bottom: 1.5rem;
    }
    .hero-content .btn {
      padding: 0.75rem 1.5rem;
      background-color: #8a2be2; /* button light purple */
      color: white;
      border: none;
      border-radius: 30px;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
    }
    .hero-content .btn:hover {
      background-color: #6a0dad;
    }

    /* Below hero, normal content */
    .container {
      width: 90%;
      max-width: 960px;
      margin: 0 auto;
      padding: 2rem 0;
      background: #f4f1fa;
      color: #333;
    }
    .container h2 {
      color: #6a0dad;
      margin-bottom: 1rem;
    }
    .menu-items {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1.5rem;
    }
    .menu-item {
      background: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      color: #333;
    }
    .menu-item img {
      width: 100%;
      height: auto;
      display: block;
    }
    .menu-item .info {
      padding: 1rem;
    }
    .menu-item .info h3 {
      margin: 0;
      font-size: 1.2rem;
    }
    .menu-item .info p {
      margin-top: 0.5rem;
      color: #666;
    }
  </style>
</head>
<body>

  <nav class="navbar">
    <div class="logo">pooja poli bhaji kendra </div>
    <div class="menu">
      <a href="#menu">Menu</a>
      <a href="#contact">Contact</a>
      <a href="#order">Order</a>
    </div>
  </nav>

  <div class="hero">
    <div class="hero-content">
      <h1>Welcome to Our Kendra</h1>
      <p>Delicious meals served daily — taste, quality & comfort</p>
      <a href="#menu" class="btn">Explore Menu</a>
    </div>
  </div>

  <div class="container" id="menu">
    <h2>Our Menu</h2>
    <div class="menu-items">
      <div class="menu-item">
        <img src=" C:\Users\paldi\Downloads\thali.png "alt="Veg Thali">
        <div class="info">
          <h3>Veg Thali</h3>
          <p>₹120</p>
        </div>
      </div>
      <div class="menu-item">
        <img src="C:\Users\paldi\Downloads\paneer.png" alt="Paneer Thali">
        <div class="info">
          <h3>Paneer Thali</h3>
          <p>₹150</p>
        </div>
      </div>
     <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\non.png" alt="Non‑Veg Thali">
          <div class="details">
            <h3>Non‑Veg Thali</h3>
            <p class="price">₹180</p>
          </div>
        </div>
      </div>
    </section>

    <section class="menu-section">
      <h2>Main Dishes</h2>
      <div class="menu-items">
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\fishfry.png" alt="Fish Fry">
          <div class="details">
            <h3>Fish Fry</h3>
            <p class="price">₹100</p>
          </div>
        </div>
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\Egg-Curry.jpg" alt="Egg Curry">
          <div class="details">
            <h3>Egg Curry</h3>
            <p class="price">₹80</p>
          </div>
        </div>
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\biryani.jpg" alt="Veg Biryani">
          <div class="details">
            <h3>Veg Biryani</h3>
            <p class="price">₹100</p>
          </div>
        </div>
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\non veg briyani.jpg" alt="Nonveg Biryani">
          <div class="details">
            <h3>Non‑Veg Biryani</h3>
            <p class="price">₹130</p>
          </div>
        </div>
      </div>
    </section>

    <section class="menu-section">
      <h2>Breakfast</h2>
      <div class="menu-items">
        <div class="menu-item">
          <img src=":\Users\paldi\Downloads\aloo.png" alt="Aloo Paratha">
          <div class="details">
            <h3>Aloo Paratha</h3>
            <p class="price">₹60</p>
          </div>
        </div>
      </div>
    </section>

    <section class="menu-section">
      <h2>Roti / Chapati</h2>
      <div class="menu-items">
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\plain roti.jpg" alt="Plain Chapati">
          <div class="details">
            <h3>Plain Chapati</h3>
            <p class="price">₹10</p>
          </div>
        </div>
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\jowar.png" alt="Jowar Roti">
          <div class="details">
            <h3>Jowar Roti</h3>
            <p class="price">₹15</p>
          </div>
        </div>
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\bajra.png" alt="Bajra Roti">
          <div class="details">
            <h3>Bajra Roti</h3>
            <p class="price">₹15</p>
          </div>
        </div>
      </div>
    </section>

    <section class="menu-section">
      <h2>Sweets & Special Orders</h2>
      <div class="menu-items">
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\purnpoli.png" alt="Puranpoli">
          <div class="details">
            <h3>Puranpoli</h3>
            <p class="price">₹25 per piece</p>
          </div>
        </div>
        <div class="menu-item">
          <img src="C:\Users\paldi\Downloads\modak.png" alt="Modak">
          <div class="details">
            <h3>Modak (On Order)</h3>
            <p class="price">Price varies – Order in advance</p>
          </div>
        </div>
      </div>
    </section>

  <div class="container" id="contact">
    <h2>Contact Us</h2>
    <p>Address: Your address here</p>
    <p>Phone: <a href="tel:+1234567890">+12 3456 7890</a></p>
    <p>WhatsApp: <a href="https://wa.me/1234567890" target="_blank">Chat on WhatsApp</a></p>
  </div>

</body>
</html>
