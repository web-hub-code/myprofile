<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Digital Powerhouse</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.06); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        /* Background & Glows */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.2); }
        .glow { position: fixed; width: 300px; height: 300px; background: var(--primary); filter: blur(150px); opacity: 0.15; z-index: -1; border-radius: 50%; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 120px; }

        /* Premium Cards */
        .card { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; position: relative; overflow: hidden; }
        .card::before { content: ''; position: absolute; top: 0; left: -100%; width: 100%; height: 100%; background: linear-gradient(90deg, transparent, rgba(255,255,255,0.05), transparent); transition: 0.5s; }
        .card:hover::before { left: 100%; }

        .hero { text-align: center; padding: 60px 20px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); object-fit: cover; box-shadow: 0 0 40px rgba(0, 242, 254, 0.6); margin-bottom: 20px; }
        h1 { font-size: 2.3rem; font-weight: 800; line-height: 1.1; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Services Grid */
        .service-box { margin-top: 15px; }
        .s-card { display: flex; align-items: flex-start; gap: 15px; margin-bottom: 20px; padding: 15px; border-radius: 20px; background: rgba(255,255,255,0.03); }
        .s-card i { font-size: 1.5rem; color: var(--primary); margin-top: 5px; }
        .s-card h4 { font-size: 1.1rem; color: var(--secondary); margin-bottom: 4px; }
        .s-card p { font-size: 0.8rem; opacity: 0.7; line-height: 1.4; }

        /* Visitor Map Placeholder */
        .map-section { text-align: center; }
        .map-img { width: 100%; border-radius: 15px; opacity: 0.8; margin-top: 10px; }

        /* Navigation */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; background: rgba(0,0,0,0.8); backdrop-filter: blur(25px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.2rem; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); transform: scale(1.2); }

        .btn-main { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 20px; font-weight: 800; cursor: pointer; margin-top: 10px; font-size: 1rem; box-shadow: 0 10px 25px rgba(0, 242, 254, 0.3); }

        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; letter-spacing: 2px; }
    </style>
</head>
<body>

    <div class="glow" style="top: 10%; left: -10%;"></div>
    <div class="glow" style="bottom: 10%; right: -10%; background: var(--accent);"></div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="https://wa.me/923000000000" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-paper-plane"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Hi, I'm <span class="gradient-text">Nazim</span></h1>
            <p style="margin-top: 10px; font-weight: 300; letter-spacing: 4px; font-size: 0.7rem; color: var(--primary);">FOUNDER OF PRIME SOLUTIONS</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-crown" style="color: gold;"></i> My Premium Services</h3>
            
            <div class="s-card">
                <i class="fas fa-code"></i>
                <div>
                    <h4>Next-Gen Web Development</h4>
                    <p>Main aisi websites banata hoon jo super fast hain aur 2026 ke modern standards par poori utarti hain.</p>
                </div>
            </div>

            <div class="s-card">
                <i class="fas fa-palette"></i>
                <div>
                    <h4>Creative Branding</h4>
                    <p>Aapke business ko aik brand banana meri zimmedari hai. Unique logos aur eye-catching designs.</p>
                </div>
            </div>

            <div class="s-card">
                <i class="fas fa-brain"></i>
                <div>
                    <h4>AI Digital Solutions</h4>
                    <p>Automated systems aur AI tools ke zariye aapke mushkil kaamo ko asaan aur smart banana.</p>
                </div>
            </div>
        </div>

        <div class="card map-section" data-aos="fade-up">
            <h3><i class="fas fa-globe-americas" style="color: var(--primary);"></i> Global Presence</h3>
            <p style="font-size: 0.75rem; opacity: 0.6; margin-top: 5px;">Tracking real-time profile visitors worldwide.</p>
            <img src="https://upload.wikimedia.org/wikipedia/commons/e/ec/World_map_blank_without_borders.svg" class="map-img" style="filter: invert(1) sepia(1) saturate(5) hue-rotate(175deg);">
            <div style="margin-top: 15px; font-weight: 800; font-size: 1.2rem; color: var(--primary);">LIVE 🟢</div>
        </div>

        <div class="card" data-aos="fade-up" style="text-align: center;">
            <h3 style="margin-bottom: 10px;">Ready to Start?</h3>
            <p style="font-size: 0.8rem; opacity: 0.7; margin-bottom: 20px;">Let's turn your idea into a digital masterpiece.</p>
            <button class="btn-main" onclick="location.href='https://wa.me/923000000000'">Hired Me on WhatsApp</button>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | DESIGNED WITH LOVE</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
