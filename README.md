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
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; cursor: none; }

        /* Animated Background Video */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.18); }

        /* Custom Cursor for Desktop */
        #cursor { width: 10px; height: 10px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 9999; box-shadow: 0 0 15px var(--primary); transition: transform 0.1s; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Premium Glass Card */
        .card { 
            background: var(--glass); 
            backdrop-filter: blur(25px); 
            border: 1px solid var(--border); 
            border-radius: 35px; 
            padding: 28px; 
            margin-bottom: 22px; 
            transition: 0.4s; 
            position: relative;
            overflow: hidden;
        }
        .card:hover { transform: scale(1.02); border-color: var(--primary); }
        
        /* Hero Details */
        .hero { text-align: center; padding: 45px 10px; }
        .profile-pic { width: 135px; height: 135px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; box-shadow: 0 0 25px rgba(0, 242, 254, 0.3); margin-bottom: 18px; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; letter-spacing: -1px; }
        
        .status-badge { display: inline-block; background: rgba(46, 204, 113, 0.15); color: #2ecc71; padding: 5px 15px; border-radius: 20px; font-size: 0.75rem; font-weight: 600; margin-top: 10px; }

        /* Service Tags */
        .service-tag { display: inline-flex; align-items: center; gap: 8px; padding: 12px 20px; background: rgba(255,255,255,0.04); border: 1px solid var(--border); border-radius: 50px; font-size: 0.8rem; margin: 6px; }
        .service-tag i { color: var(--primary); font-size: 1rem; }

        /* Project Display */
        .project-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 15px; }
        .project-box { border-radius: 22px; overflow: hidden; border: 1px solid var(--border); background: #000; }
        .project-img { width: 100%; height: 120px; object-fit: cover; opacity: 0.7; transition: 0.5s; }
        .project-box:hover .project-img { opacity: 1; transform: scale(1.1); }

        /* Bottom Floating Bar */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 380px; background: rgba(10, 10, 10, 0.85); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.4rem; opacity: 0.7; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); opacity: 1; }

        /* Contact Buttons */
        .btn-main { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; cursor: pointer; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 12px; margin-top: 10px; }
        .btn-outline { display: block; text-align: center; margin-top: 15px; color: var(--primary); text-decoration: none; font-size: 0.95rem; font-weight: 600; border: 1px solid var(--primary); padding: 12px; border-radius: 20px; }

        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; margin-top: 30px; }
    </style>
</head>
<body>

    <div id="cursor"></div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-house"></i></a>
        <a href="https://wa.me/923332637235" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="opacity: 0.7; font-weight: 300;">Next-Gen Web Solutions</p>
            <div class="status-badge"><i class="fas fa-circle" style="font-size: 8px;"></i> Available for Projects</div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-wand-magic-sparkles"></i> Premium Services</h3>
            <div class="service-tag"><i class="fas fa-bolt"></i> High Speed Hosting</div>
            <div class="service-tag"><i class="fas fa-mobile"></i> Mobile First Design</div>
            <div class="service-tag"><i class="fas fa-code"></i> Clean React/HTML</div>
            <div class="service-tag"><i class="fas fa-magnifying-glass"></i> SEO Boost</div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 12px;"><i class="fas fa-rocket"></i> My Portfolio</h3>
            <div class="project-grid">
                <div class="project-box"><img src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97?w=400" class="project-img"></div>
                <div class="project-box"><img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=400" class="project-img"></div>
            </div>
            <p style="font-size: 0.8rem; opacity: 0.6; margin-top: 15px; text-align: center;">Verified 5-Star Experience in Web Dev</p>
        </div>

        <div class="card" data-aos="fade-up" style="border-left: 4px solid var(--primary);">
            <h3 style="margin-bottom: 10px;"><i class="fas fa-phone-volume"></i> Direct Contact</h3>
            <p style="font-size: 0.85rem; opacity: 0.7; margin-bottom: 20px;">Main hamesha premium support aur fast delivery provide karta hoon.</p>
            
            <a href="https://wa.me/923332637235" class="btn-main">
                <i class="fab fa-whatsapp"></i> Chat on WhatsApp
            </a>
            
            <a href="tel:03705519562" class="btn-outline">
                <i class="fas fa-phone"></i> Call: 0370 5519562
            </a>
        </div>

        <footer class="footer-links">
            <p>© 2026 PRIME SOLUTIONS | MUHAMMAD NAZIM</p>
            <div style="margin-top: 10px;">
                <a href="privacy.html" style="color: white; opacity: 0.5; text-decoration: none;">Privacy Policy</a>
            </div>
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Custom Cursor Script
        const cursor = document.getElementById('cursor');
        document.addEventListener('mousemove', e => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
        });

        // Hide cursor on touch devices
        if ('ontouchstart' in window) { cursor.style.display = 'none'; }
    </script>
</body>
</html>
