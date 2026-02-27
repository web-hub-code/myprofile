<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Prime Solutions Architect</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; cursor: default; }

        /* Tech Background Video */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Glassmorphism Card Design */
        .card { 
            background: var(--glass); 
            backdrop-filter: blur(25px); 
            -webkit-backdrop-filter: blur(25px);
            border: 1px solid var(--border); 
            border-radius: 35px; 
            padding: 28px; 
            margin-bottom: 22px; 
            transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); 
        }
        .card:hover { transform: translateY(-5px); border-color: var(--primary); box-shadow: 0 15px 35px rgba(0, 242, 254, 0.15); }
        
        /* Profile & Hero */
        .hero { text-align: center; padding: 45px 10px; }
        .profile-wrapper { position: relative; display: inline-block; }
        .profile-pic { width: 135px; height: 135px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 18px; box-shadow: 0 0 25px rgba(0, 242, 254, 0.3); }
        .status-online { position: absolute; bottom: 25px; right: 12px; width: 18px; height: 18px; background: #2ecc71; border-radius: 50%; border: 3px solid var(--bg); animation: glow 2s infinite; }
        
        @keyframes glow { 0% { box-shadow: 0 0 0 0 rgba(46, 204, 113, 0.7); } 70% { box-shadow: 0 0 0 10px rgba(46, 204, 113, 0); } 100% { box-shadow: 0 0 0 0 rgba(46, 204, 113, 0); } }

        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; letter-spacing: -1px; }

        /* Skill Badges */
        .badge-container { display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; margin-top: 15px; }
        .badge { background: rgba(255,255,255,0.05); border: 1px solid var(--border); padding: 8px 16px; border-radius: 50px; font-size: 0.8rem; font-weight: 500; display: flex; align-items: center; gap: 6px; }
        .badge i { color: var(--primary); }

        /* Portfolio Gallery */
        .work-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 15px; }
        .work-item { border-radius: 20px; overflow: hidden; border: 1px solid var(--border); position: relative; }
        .work-img { width: 100%; height: 120px; object-fit: cover; transition: 0.5s; opacity: 0.8; }
        .work-item:hover .work-img { transform: scale(1.1); opacity: 1; }

        /* FAQ Accordion */
        details { background: rgba(255,255,255,0.03); padding: 12px; border-radius: 15px; margin-bottom: 8px; border: 1px solid var(--border); }
        summary { font-size: 0.9rem; font-weight: 600; cursor: pointer; color: var(--primary); outline: none; }
        details p { font-size: 0.8rem; opacity: 0.7; padding-top: 8px; line-height: 1.5; }

        /* Floating Nav Bar */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 380px; background: rgba(10, 10, 10, 0.8); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; box-shadow: 0 15px 40px rgba(0,0,0,0.6); }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.6; transition: 0.3s; }
        .nav-link:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* Action Buttons */
        .btn-wa { background: linear-gradient(45deg, #25d366, #128c7e); color: white; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 15px; border: none; font-size: 1rem; }
        .btn-call { display: block; text-align: center; margin-top: 15px; color: var(--primary); text-decoration: none; font-size: 0.95rem; font-weight: 600; border: 1px solid var(--primary); padding: 14px; border-radius: 20px; transition: 0.3s; }
        .btn-call:hover { background: rgba(0, 242, 254, 0.1); }

        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; margin-top: 20px; padding-bottom: 20px; }
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
            <div class="profile-wrapper">
                <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
                <div class="status-online"></div>
            </div>
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="opacity: 0.8; font-weight: 300;">Founder of Prime Solutions</p>
            <div class="badge-container">
                <div class="badge"><i class="fas fa-check-circle"></i> Certified Dev</div>
                <div class="badge"><i class="fas fa-star"></i> 5.0 Rating</div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; font-size: 1.1rem;"><i class="fas fa-laptop-code" style="color: var(--primary);"></i> My Expertise</h3>
            <div class="badge-container" style="justify-content: flex-start;">
                <span class="badge"><i class="fas fa-code"></i> Web Architecture</span>
                <span class="badge"><i class="fas fa-mobile-alt"></i> Responsive UI</span>
                <span class="badge"><i class="fas fa-search-plus"></i> SEO Mastery</span>
                <span class="badge"><i class="fas fa-rocket"></i> Speed Optimization</span>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 12px; font-size: 1.1rem;"><i class="fas fa-folder-open"></i> Prime Works</h3>
            <div class="work-grid">
                <div class="work-item"><img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=400" class="work-img"></div>
                <div class="work-item"><img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=400" class="work-img"></div>
            </div>
            <p style="font-size: 0.75rem; text-align: center; margin-top: 12px; opacity: 0.6;">Delivering high-performance digital products worldwide.</p>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; font-size: 1.1rem;"><i class="fas fa-question-circle"></i> Quick Help</h3>
            <details>
                <summary>Delivery kitne time mein hogi?</summary>
                <p>Standard website 2 se 5 din mein complete ho jati hai.</p>
            </details>
            <details>
                <summary>Website ki security kaisi hogi?</summary>
                <p>Hum SSL encryption aur secure coding standards follow karte hain.</p>
            </details>
            <details>
                <summary>Support milegi project ke baad?</summary>
                <p>Ji bilkul! Hum 1 month ki free maintenance support dete hain.</p>
            </details>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 4px solid var(--primary);">
            <h3 style="margin-bottom: 10px;"><i class="fas fa-headset"></i> Start Your Journey</h3>
            <p style="font-size: 0.85rem; opacity: 0.7; margin-bottom: 10px;">Aapka dream project sirf ek message door hai.</p>
            
            <a href="https://wa.me/923332637235" class="btn-wa">
                <i class="fab fa-whatsapp"></i> WhatsApp Consultation
            </a>
            
            <a href="tel:03705519562" class="btn-call">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
        </div>

        <footer class="footer-links">
            <div style="margin-bottom: 15px;">
                <a href="privacy.html" style="color: white; text-decoration: none; margin: 0 10px;">Privacy Policy</a>
                <a href="#" style="color: white; text-decoration: none; margin: 0 10px;">Terms</a>
            </div>
            <p>© 2026 PRIME SOLUTIONS | MUHAMMAD NAZIM</p>
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        console.log("Prime Portfolio v3.0 Live - Developed by Nazim");
    </script>
</body>
</html>
