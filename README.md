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
            background: var(--glass); backdrop-filter: blur(25px); 
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 28px; margin-bottom: 22px; transition: 0.4s; position: relative; overflow: hidden;
        }
        .card:hover { transform: translateY(-8px); border-color: var(--primary); box-shadow: 0 15px 40px rgba(0, 242, 254, 0.2); }
        
        /* Rotating Glow Effect */
        .card::before { content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%; background: conic-gradient(transparent, transparent, transparent, var(--primary)); animation: rotate 6s linear infinite; z-index: -1; opacity: 0.1; }
        @keyframes rotate { 100% { transform: rotate(360deg); } }

        /* Hero Section */
        .hero { text-align: center; padding: 40px 10px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.4); object-fit: cover; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }

        /* Counter Stats */
        .stats-grid { display: flex; justify-content: space-around; text-align: center; margin-top: 25px; }
        .counter { color: var(--primary); font-size: 1.8rem; font-weight: 800; display: block; }
        .stat-item p { font-size: 0.7rem; opacity: 0.6; text-transform: uppercase; letter-spacing: 1px; }

        /* Logo Slider */
        .slider-container { overflow: hidden; padding: 10px 0; }
        .slider { display: flex; gap: 40px; animation: scroll 20s linear infinite; width: max-content; }
        @keyframes scroll { 0% { transform: translateX(0); } 100% { transform: translateX(-50%); } }
        .slider i { font-size: 1.8rem; opacity: 0.5; transition: 0.3s; }
        .slider i:hover { opacity: 1; color: var(--primary); }

        /* Navigation */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: rgba(10, 10, 10, 0.85); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; box-shadow: 0 10px 30px rgba(0,0,0,0.5); }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.6; transition: 0.3s; }
        .nav-link:hover { color: var(--primary); opacity: 1; transform: translateY(-5px) scale(1.1); }

        /* Buttons */
        .btn-primary { background: linear-gradient(45deg, #25d366, #128c7e); color: white; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 15px; border: none; font-size: 1rem; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); }
        .btn-outline { display: block; text-align: center; margin-top: 15px; color: var(--primary); text-decoration: none; font-size: 0.95rem; font-weight: 600; border: 1px solid var(--primary); padding: 14px; border-radius: 20px; transition: 0.3s; }
        .btn-outline:hover { background: var(--primary); color: #000; }

        .step { display: flex; align-items: center; gap: 15px; margin-bottom: 12px; background: rgba(255,255,255,0.03); padding: 15px; border-radius: 20px; border-left: 4px solid var(--primary); }
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
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="opacity: 0.8; font-weight: 300; letter-spacing: 1px;">Digital Architect | CEO Prime Solutions</p>
            
            <div class="stats-grid">
                <div class="stat-item"><span class="counter" data-target="50">0</span><p>Projects</p></div>
                <div class="stat-item"><span class="counter" data-target="15">0</span><p>Clients</p></div>
                <div class="stat-item"><span class="counter" data-target="100">0</span><p>Trust %</p></div>
            </div>
        </section>

        <div class="card" style="padding: 15px;">
            <div class="slider-container">
                <div class="slider">
                    <i class="fab fa-html5"></i> <i class="fab fa-css3-alt"></i> <i class="fab fa-js"></i> 
                    <i class="fab fa-react"></i> <i class="fab fa-node-js"></i> <i class="fab fa-github"></i>
                    <i class="fab fa-html5"></i> <i class="fab fa-css3-alt"></i> <i class="fab fa-js"></i> 
                    <i class="fab fa-react"></i> <i class="fab fa-node-js"></i> <i class="fab fa-github"></i>
                </div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-rocket" style="color: var(--primary);"></i> Prime Services</h3>
            <div class="step"><i class="fas fa-code"></i> Modern Web Development</div>
            <div class="step"><i class="fas fa-paint-brush"></i> UI/UX Glassmorphism Design</div>
            <div class="step"><i class="fas fa-search-dollar"></i> SEO & Ranking Mastery</div>
            <div class="step"><i class="fas fa-shield-alt"></i> Secure Business Branding</div>
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
                Prime Solutions aapke data ki hifazat karta hai. Hum 100% money-back guarantee aur lifetime support provide karte hain.
            </p>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 5px solid var(--primary);">
            <h3 style="margin-bottom: 10px;">Let's Build Something Big</h3>
            <a href="https://wa.me/923332637235" target="_blank" class="btn-primary">
                <i class="fab fa-whatsapp"></i> Get Free Consultation
            </a>
            <a href="tel:03705519562" class="btn-outline">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
        </div>

        <footer>
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Counter Animation Logic
        const counters = document.querySelectorAll('.counter');
        counters.forEach(counter => {
            const updateCount = () => {
                const target = +counter.getAttribute('data-target');
                const count = +counter.innerText;
                const speed = 250; 
                const inc = target / speed;
                if (count < target) {
                    counter.innerText = Math.ceil(count + inc);
                    setTimeout(updateCount, 15);
                } else {
                    counter.innerText = target + (target === 100 ? '%' : '+');
                }
            };
            updateCount();
        });
    </script>
</body>
</html>
