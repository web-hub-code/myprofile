<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Prime Solutions | Digital Agency</title>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins,Arial}
html{scroll-behavior:smooth}
body{background:#f5f7fb;color:#333}

/* NAVBAR */
header{
position:fixed;top:0;width:100%;z-index:1000;
background:rgba(13,110,253,.95);
padding:15px 60px;
display:flex;justify-content:space-between;align-items:center}
header h2{color:#fff}
header a{color:#fff;text-decoration:none;margin-left:18px;font-weight:500}

/* HERO */
.hero{
min-height:100vh;
background:linear-gradient(135deg,#0d6efd,#6610f2);
color:#fff;
display:flex;align-items:center;justify-content:center;
text-align:center;padding:40px}
.hero h1{font-size:52px;margin-bottom:15px}
.hero p{font-size:18px;opacity:.9}
.hero button{
margin-top:25px;
background:#fff;color:#0d6efd;
border:none;padding:14px 34px;
border-radius:30px;font-size:16px;cursor:pointer}

/* SECTIONS */
section{padding:90px 60px}
.section-title{text-align:center;margin-bottom:50px;font-size:32px}

/* ABOUT */
.about p{max-width:900px;margin:auto;text-align:center;font-size:17px}

/* STATS */
.stats{
background:#fff;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
text-align:center}
.stats div{padding:40px}
.stats h2{color:#0d6efd;font-size:36px}

/* SERVICES */
.services{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
gap:25px}
.card{
background:#fff;
padding:35px;
border-radius:18px;
box-shadow:0 20px 40px rgba(0,0,0,.08);
text-align:center}
.card i{font-size:42px;color:#0d6efd;margin-bottom:15px}

/* PORTFOLIO */
.portfolio{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
gap:20px}
.portfolio div{
background:linear-gradient(135deg,#e9ecef,#dee2e6);
padding:60px;border-radius:15px;
text-align:center;font-weight:600}

/* CONTACT */
.contact form{
max-width:520px;margin:auto;
background:#fff;padding:40px;
border-radius:18px;
box-shadow:0 20px 40px rgba(0,0,0,.08)}
.contact input,.contact textarea{
width:100%;padding:14px;margin-bottom:15px;
border-radius:10px;border:1px solid #ccc}
.contact button{
width:100%;padding:14px;
background:#0d6efd;color:#fff;
border:none;border-radius:30px;font-size:16px}

/* FOOTER */
footer{
background:#111;color:#fff;
text-align:center;padding:25px}

/* WHATSAPP */
.whatsapp{
position:fixed;bottom:25px;right:25px;
background:#25d366;color:#fff;
padding:16px;border-radius:50%;
font-size:22px;text-decoration:none}
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
<a href="#contact">Contact</a>
</nav>
</header>

<div class="hero" id="home">
<div>
<h1>Prime Solutions</h1>
<p>Digital Growth Starts Here</p>
<button>Get Free Consultation</button>
</div>
</div>

<section id="about" class="about">
<h2 class="section-title">About Us</h2>
<p>
We help businesses grow online with modern WordPress websites,
SEO optimization and professional digital solutions.
</p>
</section>

<section class="stats">
<div><h2>200+</h2><p>Clients</p></div>
<div><h2>450+</h2><p>Projects</p></div>
<div><h2>7+</h2><p>Years Experience</p></div>
</section>

<section id="services">
<h2 class="section-title">Our Services</h2>
<div class="services">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3></div>
<div class="card"><i class="fa-brands fa-wordpress"></i><h3>WordPress Websites</h3></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Marketing</h3></div>
<div class="card"><i class="fa-solid fa-mobile-screen"></i><h3>Responsive Design</h3></div>
</div>
</section>

<section id="portfolio">
<h2 class="section-title">Our Work</h2>
<div class="portfolio">
<div>Business Website</div>
<div>E-Commerce Store</div>
<div>Landing Page</div>
<div>Corporate Website</div>
</div>
</section>

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
