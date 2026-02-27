<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Prime Solutions Official</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        .card { 
            background: var(--glass); 
            backdrop-filter: blur(25px); 
            border: 1px solid var(--border); 
            border-radius: 35px; 
            padding: 28px; 
            margin-bottom: 22px; 
            transition: 0.4s; 
        }
        .card:hover { transform: translateY(-5px); border-color: var(--primary); box-shadow: 0 15px 35px rgba(0, 242, 254, 0.15); }
        
        /* Hero Section */
        .hero { text-align: center; padding: 40px 10px; }
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; box-shadow: 0 0 20px rgba(0, 242, 254, 0.3); }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }

        /* Stats Section */
        .stats-grid { display: flex; justify-content: space-around; text-align: center; margin-top: 10px; }
        .stat-item h2 { color: var(--primary); font-size: 1.5rem; }
        .stat-item p { font-size: 0.65rem; opacity: 0.6; text-transform: uppercase; }

        /* Process Steps */
        .step { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; background: rgba(255,255,255,0.03); padding: 12px; border-radius: 20px; border: 1px solid var(--border); }
        .step-num { background: var(--primary); color: #000; width: 30px; height: 30px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 800; }

        /* Navigation */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 380px; background: rgba(10, 10, 10, 0.85); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.6; transition: 0.3s; }
        .nav-link:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* Buttons */
        .btn-primary { background: linear-gradient(45deg, #25d366, #128c7e); color: white; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 15px; border: none; font-size: 1rem; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); }
        .btn-outline { display: block; text-align: center; margin-top: 15px; color: var(--primary); text-decoration: none; font-size: 0.95rem; font-weight: 600; border: 1px solid var(--primary); padding: 14px; border-radius: 20px; transition: 0.3s; }

        .testimonial { font-style: italic; font-size: 0.85rem; opacity: 0.8; border-left: 3px solid var(--accent); padding-left: 15px; margin-top: 10px; }

        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; margin-top: 20px; padding-bottom: 30px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="nav-bar">
        <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="opacity: 0.8; font-weight: 300;">Digital Architect | CEO Prime Solutions</p>
            <div class="stats-grid" style="margin-top: 25px;">
                <div class="stat-item"><h2>50+</h2><p>Projects</p></div>
                <div class="stat-item"><h2>15+</h2><p>Global Clients</p></div>
                <div class="stat-item"><h2>5★</h2><p>Rating</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-rocket" style="color: var(--primary);"></i> Prime Services</h3>
            <div style="font-size: 0.9rem; opacity: 0.8; line-height: 1.8;">
                • Modern Web Development (React/HTML/JS)<br>
                • High-Conversion Landing Pages<br>
                • SEO & Google Ranking Mastery<br>
                • Business Branding & UI/UX Design
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-stream"></i> My Working Process</h3>
            <div class="step"><div class="step-num">1</div><p style="font-size: 0.8rem;"><b>Discovery:</b> Aapke business goals ko samajhna.</p></div>
            <div class="step"><div class="step-num">2</div><p style="font-size: 0.8rem;"><b>Design:</b> Modern aur unique UI/UX prototype.</p></div>
            <div class="step"><div class="step-num">3</div><p style="font-size: 0.8rem;"><b>Develop:</b> Fast aur clean coding with SEO.</p></div>
            <div class="step"><div class="step-num">4</div><p style="font-size: 0.8rem;"><b>Launch:</b> Final testing aur live deployment.</p></div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-quote-left" style="color: var(--accent);"></i> Client Feedback</h3>
            <div class="testimonial">
                "Nazim built our business site in just 3 days. The speed and design are top-notch! Highly recommended for any professional work."
            </div>
            <p style="font-size: 0.7rem; margin-top: 5px; text-align: right; opacity: 0.5;">— CEO, TechStream Agency</p>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 10px;"><i class="fas fa-user-shield"></i> Privacy & Trust</h3>
            <p style="font-size: 0.75rem; opacity: 0.6; line-height: 1.5;">
                Prime Solutions aapke data ki hifazat karta hai. Hum 100% money-back guarantee aur lifetime support provide karte hain. Tamam projects professional NDA ke tehat mukammal kiye jatay hain.
            </p>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 5px solid var(--primary);">
            <h3 style="margin-bottom: 10px;">Let's Build Something Big</h3>
            <a href="https://wa.me/923332637235" class="btn-primary">
                <i class="fab fa-whatsapp"></i> Get Free Consultation
            </a>
            <a href="tel:03705519562" class="btn-outline">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
        </div>

        <footer>
            <div style="margin-bottom: 10px;">
                <a href="#" style="color: white; text-decoration: none; margin: 0 10px;">Privacy Policy</a> | 
                <a href="#" style="color: white; text-decoration: none; margin: 0 10px;">Terms</a>
            </div>
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
