<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SkyLink Networks</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }
    header {
      background: #003366;
      color: white;
      padding: 1em;
    }
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }
    nav ul li a {
      color: white;
      text-decoration: none;
    }
    .logo {
      height: 50px;
    }
    .hero {
      padding: 2em;
      background: #f4f4f4;
      text-align: center;
    }
    .towns {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1em;
      padding: 1em;
    }
    .package {
      background: #eaf3ff;
      padding: 1em;
      border-radius: 10px;
    }
    .book-btn {
      background: #0078d4;
      color: white;
      padding: 10px 15px;
      text-decoration: none;
      display: inline-block;
      margin: 1em;
      border-radius: 8px;
    }
    footer {
      background: #111;
      color: white;
      padding: 1em;
      text-align: center;
    }
    .social a {
      color: #99ccff;
      text-decoration: none;
    }
    #chatbot-float {
      position: fixed;
      bottom: 30px;
      left: 50%;
      transform: translateX(-50%);
      background: #0078d4;
      color: white;
      padding: 10px 15px;
      border-radius: 25px;
      z-index: 999;
      text-decoration: none;
    }
    section {
      padding: 1.5em;
    }
    button {
      padding: 10px 15px;
      margin: 5px;
      background: #0078d4;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
  </style>
</head>
<body>

<!-- Floating Chatbot -->
<a href="https://bit.ly/SkylinkNetworks" id="chatbot-float" target="_blank">💬 Chat with Us</a>

<!-- Header Navigation -->
<header>
  <nav>
    <img src="assets/images/skylink-logo.png" alt="SkyLink Logo" class="logo">
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#pricing">Pricing</a></li>
      <li><a href="#shop">Our Shop</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<!-- Hero Section -->
<section id="home" class="hero">
  <h1>Speed That Doesn't Flinch. Support That Doesn't Ghost You.</h1>
  <p>Welcome to SkyLink Networks, where blazing-fast internet meets real human support. No gimmicks. No lag. Just power, precision, and peace of mind.</p>
  <button onclick="scrollToSection('pricing')">Explore Plans</button>
  <button onclick="scrollToSection('coverage')">See Coverage</button>
</section>

<!-- Location Access Section -->
<section id="coverage">
  <h2>Check Coverage in Your Area</h2>
  <button onclick="checkLocation()">Enable Location</button>
  <div id="location-result"></div>
</section>

<!-- Pricing Section -->
<section id="pricing">
  <h2>Explore Our Unlimited Internet Packages</h2>
  <div class="towns">
    <div class="package">
      <h3>Muguga</h3>
      <ul>
        <li>8Mbps - KES 1,750</li>
        <li>10Mbps - KES 1,900</li>
        <li>15Mbps - KES 2,000</li>
        <li>20Mbps - KES 2,500</li>
        <li>30Mbps - KES 3,000</li>
        <li>40Mbps - KES 4,000</li>
      </ul>
    </div>
    <div class="package">
      <h3>Nakuru / Eldoret / Kitale</h3>
      <ul>
        <li>12Mbps - KES 2,000</li>
        <li>20Mbps - KES 2,500</li>
        <li>30Mbps - KES 3,000</li>
        <li>40Mbps - KES 4,000</li>
        <li><em>Egerton: Installation fee KES 2,000</em></li>
      </ul>
    </div>
    <div class="package">
      <h3>Kapsabet</h3>
      <ul>
        <li>10Mbps - KES 2,000</li>
        <li>15Mbps - KES 2,500</li>
        <li>20Mbps - KES 3,000</li>
        <li>30Mbps - KES 4,000</li>
        <li><em>Installation fee KES 2,000</em></li>
      </ul>
    </div>
    <div class="package">
      <h3>Business Lite</h3>
      <ul>
        <li>15Mbps - KES 2,500</li>
        <li>30Mbps - KES 3,500</li>
        <li>60Mbps - KES 6,000</li>
        <li>80Mbps - KES 7,000</li>
        <li>100Mbps - KES 8,000</li>
      </ul>
    </div>
  </div>
  <a class="book-btn" href="https://bit.ly/customerreq" target="_blank">Get Started</a>
</section>

<!-- About Section -->
<section id="about">
  <h2>Built for Speed. Driven by Service.</h2>
  <p>At SkyLink Networks, we're not just in the business of internet—we're in the business of connection... real speed, and real accountability.</p>
  <blockquote>“We don’t follow the industry standard. We raise it.”</blockquote>
</section>

<!-- Testimonials Section -->
<section id="testimonials">
  <h2>Don’t Take Our Word for It—Take Theirs.</h2>
  <blockquote>“I used to dread video calls. Now I run my business from my living room. And it just works.”<br>– Jessica Reuben, Small Biz Owner</blockquote>
  <blockquote>“Moved out of the city, thought I’d be stuck with dial-up speeds. SkyLink proved me wrong.”<br>– Tarus Kipkalya, Rural Customer</blockquote>
  <blockquote>“Skylink Networks didn’t just give us speed—they gave us stability. Our team relies on them every day to stay connected, serve clients, and grow our brand.”<br>– Asaph Njenga, Ventures Tech House</blockquote>
</section>

<!-- Contact Section -->
<section id="contact">
  <h2>Real Support. Real Fast.</h2>
  <p>📞 +254 725 013 972 | +254 111 053 184</p>
  <p>📧 info@skylinknetworks.co.ke</p>
  <p>🌐 www.skylinknetworks.co.ke</p>
  <p>Working Hours: Mon–Sat, 9:00am–5:00pm</p>
  <button onclick="callNow()">Book Us Now</button>
</section>

<!-- Footer -->
<footer>
  <div class="stats">
    <div>👨‍💼 2678+ Happy Clients</div>
    <div>💼 281+ Experts</div>
    <div>🔥 100% Satisfaction</div>
    <div>⏳ 8+ Years Experience</div>
    <div>🏆 20+ ISP Awards</div>
  </div>
  <p>We are NFP & ASP licensed.</p>
  <p>&copy; 2025 SkyLink Networks LTD. All Rights Reserved.</p>
  <div class="social">
    <a href="https://facebook.com/SkylinkKenya" target="_blank">📘 Facebook @SkylinkKenya</a><br>
    <a href="https://instagram.com/SkylinkKenya" target="_blank">📸 Instagram @SkylinkKenya</a><br>
    <a href="https://twitter.com/SkyLinkKenya_" target="_blank">🐦 X (Twitter) @SkyLinkKenya_</a><br>
    <a href="https://www.tiktok.com/@SkylinkKenya" target="_blank">🎵 TikTok @SkylinkKenya</a><br>
    <a href="https://www.linkedin.com/company/skylink-kenya" target="_blank">💼 LinkedIn Skylink Kenya</a>
  </div>
</footer>

<script>
  function scrollToSection(id) {
    document.getElementById(id).scrollIntoView({ behavior: "smooth" });
  }

  function callNow() {
    window.location.href = "tel:+254725013972";
  }

  function checkLocation() {
    if (!navigator.geolocation) {
      alert("Geolocation is not supported by your browser");
      return;
    }
    navigator.geolocation.getCurrentPosition((position) => {
      const lat = position.coords.latitude;
      const lng = position.coords.longitude;
      document.getElementById("location-result").innerText =
        "📍 Location detected. Our team will confirm availability shortly!";
    }, () => {
      alert("Unable to retrieve your location");
    });
  }
</script>
</body>
</html>
