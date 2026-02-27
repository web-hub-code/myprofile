<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Professional Web Architect</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        /* Animated Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Glassmorphism Card Style */
        .card { 
            background: var(--glass); 
            backdrop-filter: blur(20px); 
            border: 1px solid var(--border); 
            border-radius: 30px; 
            padding: 25px; 
            margin-bottom: 20px; 
            transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); 
        }
        .card:hover { transform: translateY(-8px); border-color: var(--primary); box-shadow: 0 15px 30px rgba(0, 242, 254, 0.1); }
        
        /* Hero Section */
        .hero { text-align: center; padding: 40px 10px; }
        .profile-container { position: relative; display: inline-block; }
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; }
        .status-dot { position: absolute; bottom: 25px; right: 10px; width: 15px; height: 15px; background: #2ecc71; border-radius: 50%; border: 3px solid var(--bg); animation: pulse 2s infinite; }
        
        @keyframes pulse { 0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(46, 204, 113, 0.7); } 70% { transform: scale(1); box-shadow: 0 0 0 10px rgba(46, 204, 113, 0); } 100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(46, 204, 113, 0); } }

        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.2rem; line-height: 1.2; }
        .rating { color: #ffd700; margin-top: 8px; font-size: 0.9rem; letter-spacing: 2px; }

        /* Expertise Badges */
        .service-tag { display: inline-flex; align-items: center; gap: 6px; padding: 10px 18px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); border-radius: 50px; font-size: 0.85rem; margin: 5px; font-weight: 500; }
        .service-tag i { color: var(--primary); }

        /* Project Grid */
        .img-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 15px; }
        .project-card { border-radius: 20px; overflow: hidden; position: relative; border: 1px solid var(--border); }
        .grid-img { width: 100%; height: 130px; object-fit: cover; transition: 0.5s; }
        .project-card:hover .grid-img { transform: scale(1.1); }
        .project-info { padding: 10px; font-size: 0.75rem; text-align: center; background: rgba(0,0,0,0.5); }

        /* Trust Badges */
        .trust-flex { display: flex; justify-content: space-around; text-align: center; margin-top: 10px; opacity: 0.7; font-size: 0.7rem; }
        .trust-flex i { font-size: 1.2rem; display: block; margin-bottom: 5px; color: var(--secondary); }

        /* Bottom Navigation */
        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: rgba(10, 10, 10, 0.8); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 12px; z-index: 1000; box-shadow: 0 10px 30px rgba(0,0,0,0.5); }
        .nav-item { color: white; font-size: 1.4rem; transition: 0.3s; opacity: 0.6; }
        .nav-item:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* Action Buttons */
        .btn-call { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 25px; font-weight: 800; cursor: pointer; font-size: 1rem; box-shadow: 0 8px 20px rgba(0, 242, 254, 0.2); text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 10px; }
        
        .footer-links { text-align: center; font-size: 0.8rem; margin-top: 20px; opacity: 0.5; }
        .footer-links a { color: white; text-decoration: none; margin: 0 10px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div class="profile-container">
                <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
                <div class="status-dot"></div>
            </div>
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="opacity: 0.8; font-weight: 300; letter-spacing: 1px;">Creative Web Developer & UI Architect</p>
            <div class="rating">
                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                <div style="font-size: 0.7rem; color: white; opacity: 0.5; margin-top: 5px;">Trusted by 50+ Global Clients</div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; font-size: 1.1rem;"><i class="fas fa-shield-halved" style="color: var(--primary);"></i> Core Expertise</h3>
            <div class="service-tag"><i class="fas fa-code"></i> Custom Coding</div>
            <div class="service-tag"><i class="fas fa-bolt"></i> Speed Optimization</div>
            <div class="service-tag"><i class="fas fa-layer-group"></i> UI/UX Design</div>
            <div class="service-tag"><i class="fas fa-search-dollar"></i> SEO Mastery</div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 10px; font-size: 1.1rem;"><i class="fas fa-fire"></i> Premium Works</h3>
            <div class="img-grid">
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=400" class="grid-img">
                    <div class="project-info">E-commerce App</div>
                </div>
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=400" class="grid-img">
                    <div class="project-info">Business Analytics</div>
                </div>
            </div>
            <p style="font-size: 0.8rem; margin-top: 15px; line-height: 1.6; opacity: 0.7; text-align: center;">
                "Transforming complex ideas into simple, beautiful digital realities."
            </p>
        </div>

        <div class="card" data-aos="fade-up">
            <div class="trust-flex">
                <div><i class="fas fa-lock"></i> Secure Code</div>
                <div><i class="fas fa-clock"></i> 24/7 Support</div>
                <div><i class="fas fa-check-double"></i> 100% Quality</div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="background: linear-gradient(to bottom right, rgba(0, 242, 254, 0.05), rgba(240, 147, 251, 0.05));">
            <h3 style="margin-bottom: 10px;"><i class="fas fa-comment-dots"></i> Start a Project</h3>
            <p style="font-size: 0.85rem; opacity: 0.7; margin-bottom: 20px;">Ready to grow your business? Let's discuss your vision.</p>
            <a href="https://wa.me/923332637235" class="btn-call">
                <i class="fab fa-whatsapp"></i> Chat on WhatsApp
            </a>
            <a href="tel:+923332637235" style="display: block; text-align: center; margin-top: 15px; color: var(--primary); text-decoration: none; font-size: 0.9rem;">
                Quick Call: +92 333 2637235
            </a>
        </div>

        <div class="footer-links">
            <a href="privacy.html">Privacy Policy</a> | <a href="#">Terms of Use</a>
            <p style="margin-top: 15px; opacity: 0.6;">© 2026 PRIME SOLUTIONS | MUHAMMAD NAZIM</p>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        // Smooth Title Animation
        console.log("Portfolio Loaded Successfully | Developed by Nazim");
    </script>
</body>
</html>
