<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Prime Solutions | Digital Agency</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}
html{scroll-behavior:smooth;}
body{background:#f5f7fb;color:#333;line-height:1.6;}

/* NAVBAR */
header{
position:fixed;top:0;width:100%;z-index:1000;
background:rgba(13,110,253,.95);
padding:15px 60px;
display:flex;justify-content:space-between;align-items:center;
transition:0.3s;}
header h2{color:#fff;letter-spacing:1px;}
header a{color:#fff;text-decoration:none;margin-left:20px;font-weight:500;transition:0.2s;}
header a:hover{color:#ffc107;}

/* HERO */
.hero{
min-height:100vh;
background:linear-gradient(rgba(13,110,253,.6), rgba(102,16,242,.6)), url('https://source.unsplash.com/1600x900/?technology,office');
background-size:cover;background-position:center;
color:#fff;display:flex;align-items:center;justify-content:center;text-align:center;padding:40px;}
.hero h1{font-size:56px;margin-bottom:15px;letter-spacing:1px;}
.hero p{font-size:20px;opacity:.9;margin-bottom:25px;}
.hero button{margin-top:25px;background:#fff;color:#0d6efd;border:none;padding:16px 38px;border-radius:50px;font-size:17px;cursor:pointer;transition:0.3s;}
.hero button:hover{background:#ffc107;color:#fff;transform:scale(1.05);}

/* SECTIONS */
section{padding:100px 60px;}
.section-title{text-align:center;margin-bottom:60px;font-size:36px;font-weight:600;position:relative;}
.section-title::after{content:'';display:block;width:80px;height:4px;background:#0d6efd;margin:15px auto 0;border-radius:2px;}

/* ABOUT */
.about{display:flex;flex-wrap:wrap;align-items:center;gap:40px;}
.about img{flex:1 1 400px;border-radius:20px;max-width:100%;box-shadow:0 20px 40px rgba(0,0,0,.1);}
.about-text{flex:1 1 400px;font-size:18px;color:#555;}

/* STATS */
.stats{background:#fff;display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));text-align:center;gap:20px;padding:60px 40px;border-radius:15px;box-shadow:0 20px 40px rgba(0,0,0,.08);}
.stats div{padding:20px;}
.stats h2{color:#0d6efd;font-size:38px;margin-bottom:10px;}
.stats p{font-size:16px;color:#555;}

/* SERVICES */
.services{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:30px;}
.card{background:#fff;padding:40px;border-radius:20px;box-shadow:0 20px 40px rgba(0,0,0,.08);text-align:center;transition:0.4s;}
.card:hover{transform:translateY(-10px);box-shadow:0 25px 50px rgba(0,0,0,.12);}
.card i{font-size:50px;color:#0d6efd;margin-bottom:20px;transition:0.3s;}
.card:hover i{color:#ffc107;}

/* PORTFOLIO */
.portfolio{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:25px;}
.portfolio img{width:100%;border-radius:15px;transition:0.3s;}
.portfolio img:hover{transform:scale(1.05);}

/* TESTIMONIALS */
.testimonials{background:#f1f3f6;padding:80px 60px;border-radius:20px;display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:25px;}
.testimonials .card{background:#fff;padding:30px;border-radius:20px;box-shadow:0 15px 30px rgba(0,0,0,.08);text-align:center;}
.testimonials .card img{width:80px;height:80px;border-radius:50%;margin-bottom:15px;object-fit:cover;}
.testimonials .card p{font-style:italic;color:#555;margin:15px 0;}

/* PRICING */
.pricing{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:25px;}
.pricing .card{background:#fff;padding:35px;border-radius:20px;box-shadow:0 15px 30px rgba(0,0,0,.08);text-align:center;transition:0.3s;}
.pricing .card:hover{transform:translateY(-10px);box-shadow:0 20px 40px rgba(0,0,0,.12);}
.pricing .card h3{margin-bottom:15px;}

/* CONTACT */
.contact form{max-width:550px;margin:auto;background:#fff;padding:50px;border-radius:20px;box-shadow:0 20px 40px rgba(0,0,0,.08);}
.contact input,.contact textarea{width:100%;padding:15px;margin-bottom:20px;border-radius:12px;border:1px solid #ccc;font-size:16px;}
.contact button{width:100%;padding:16px;background:#0d6efd;color:#fff;border:none;border-radius:50px;font-size:17px;transition:0.3s;cursor:pointer;}
.contact button:hover{background:#ffc107;color:#fff;}

/* FOOTER */
footer{background:#111;color:#fff;text-align:center;padding:25px;font-size:15px;}

/* WHATSAPP */
.whatsapp{position:fixed;bottom:25px;right:25px;background:#25d366;color:#fff;padding:16px;border-radius:50%;font-size:24px;text-decoration:none;transition:0.3s;}
.whatsapp:hover{transform:scale(1.1);}
</style>
</head>

<body>

<header>
<h2>Prime Solutions</h2>
<nav>
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#services">Services</a>
<a href="#portfolio">Portfolio</a>
<a href="#testimonials">Testimonials</a>
<a href="#pricing">Pricing</a>
<a href="#contact">Contact</a>
</nav>
</header>

<!-- HERO -->
<div class="hero" id="home">
<div>
<h1>Prime Solutions</h1>
<p>We help businesses grow online with modern solutions</p>
<button>Get Free Consultation</button>
</div>
</div>

<!-- ABOUT -->
<section id="about" class="about">
<img src="https://source.unsplash.com/600x400/?office,team" alt="About Image">
<div class="about-text">
<h2 class="section-title">About Us</h2>
<p>We provide professional WordPress websites, SEO services, and modern designs to help businesses grow online. Our team ensures premium quality and user-friendly solutions for every client.</p>
</div>
</section>

<!-- STATS -->
<section class="stats">
<div><h2>200+</h2><p>Clients</p></div>
<div><h2>450+</h2><p>Projects</p></div>
<div><h2>7+</h2><p>Years Experience</p></div>
</section>

<!-- SERVICES -->
<section id="services">
<h2 class="section-title">Our Services</h2>
<div class="services">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3></div>
<div class="card"><i class="fa-brands fa-wordpress"></i><h3>WordPress Websites</h3></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Marketing</h3></div>
<div class="card"><i class="fa-solid fa-mobile-screen-button"></i><h3>Responsive Design</h3></div>
</div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
<h2 class="section-title">Our Work</h2>
<div class="portfolio">
<img src="https://source.unsplash.com/400x300/?website,1" alt="Portfolio 1">
<img src="https://source.unsplash.com/400x300/?website,2" alt="Portfolio 2">
<img src="https://source.unsplash.com/400x300/?website,3" alt="Portfolio 3">
<img src="https://source.unsplash.com/400x300/?website,4" alt="Portfolio 4">
</div>
</section>

<!-- TESTIMONIALS -->
<section id="testimonials" class="testimonials">
<h2 class="section-title">Testimonials</h2>
<div class="card">
<img src="https://source.unsplash.com/80x80/?person,1" alt="Client 1">
<p>"Amazing service! Highly recommend Prime Solutions."</p>
<strong>- Client A</strong>
</div>
<div class="card">
<img src="https://source.unsplash.com/80x80/?person,2" alt="Client 2">
<p>"Professional team and fast delivery. Great experience."</p>
<strong>- Client B</strong>
</div>
</section>

<!-- PRICING -->
<section id="pricing" class="pricing">
<h2 class="section-title">Pricing Plans</h2>
<div class="card"><h3>Basic</h3><p>Website setup, 5 pages</p><p>PKR 15,000</p></div>
<div class="card"><h3>Professional</h3><p>Full WordPress website + SEO</p><p>PKR 25,000</p></div>
<div class="card"><h3>Premium</h3><p>Full website + blog + support</p><p>PKR 35,000</p></div>
</section>

<!-- CONTACT -->
<section id="contact" class="contact">
<h2 class="section-title">Contact Us</h2>
<form>
<input type="text" placeholder="Your Name">
<input type="email" placeholder="Email Address">
<textarea rows="4" placeholder="Your Message"></textarea>
<button>Send Message</button>
</form>
</section>

<footer>
© 2026 Prime Solutions — All Rights Reserved
</footer>

<a href="#" class="whatsapp">💬</a>

</body>
</html>
