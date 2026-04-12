<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | CEO Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; line-height: 1.6; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.1); }
        .overlay-mesh { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-image: radial-gradient(var(--primary) 0.5px, transparent 0.5px); background-size: 30px 30px; opacity: 0.1; z-index: -1; }

        .container { width: 100%; max-width: 480px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Trust Badge */
        .trust-badge { display: inline-flex; align-items: center; gap: 8px; background: rgba(0, 242, 254, 0.1); border: 1px solid var(--primary); padding: 8px 15px; border-radius: 50px; font-size: 0.7rem; font-weight: 600; text-transform: uppercase; color: var(--primary); margin-bottom: 20px; animation: fadeIn 1.5s ease; }

        /* Ultra Premium Card */
        .card { 
            background: var(--glass); backdrop-filter: blur(30px); -webkit-backdrop-filter: blur(30px);
            border: 1px solid var(--border); border-radius: 40px; 
            padding: 30px; margin-bottom: 25px; transition: 0.5s cubic-bezier(0.2, 1, 0.3, 1);
            position: relative;
        }
        .card:hover { transform: translateY(-12px) scale(1.02); border-color: var(--primary); box-shadow: 0 30px 60px rgba(0, 242, 254, 0.15); }

        /* Hero */
        .hero { text-align: center; padding: 50px 10px; }
        .profile-pic-container { position: relative; width: 150px; height: 150px; margin: 0 auto 20px; }
        .profile-pic { width: 100%; height: 100%; border-radius: 50%; border: 2px solid var(--primary); padding: 6px; object-fit: cover; }
        .status-dot { position: absolute; bottom: 10px; right: 10px; width: 20px; height: 20px; background: #25d366; border: 4px solid var(--bg); border-radius: 50%; box-shadow: 0 0 10px #25d366; }

        .gradient-text { background: linear-gradient(to right, #00f2fe, #f093fb); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.5rem; letter-spacing: -1px; }

        /* Service Glow Items */
        .service-item { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; background: rgba(255,255,255,0.02); padding: 18px; border-radius: 25px; border: 1px solid var(--border); transition: 0.3s; }
        .service-item:hover { background: rgba(0, 242, 254, 0.05); transform: translateX(10px); }
        .service-icon { font-size: 1.5rem; color: var(--primary); filter: drop-shadow(0 0 8px var(--primary)); }

        /* Floating WhatsApp */
        .wa-float { position: fixed; bottom: 100px; right: 25px; background: linear-gradient(45deg, #25d366, #128c7e); color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 32px; z-index: 1001; box-shadow: 0 15px 30px rgba(37, 211, 102, 0.3); animation: bounce 3s infinite; text-decoration: none; }
        @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-15px); } }

        /* Footer Nav */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 420px; background: rgba(255, 255, 255, 0.05); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 -10px 40px rgba(0,0,0,0.4); }
        .nav-link { color: rgba(255,255,255,0.6); font-size: 1.5rem; transition: 0.4s; }
        .nav-link:hover { color: var(--primary); transform: scale(1.3) rotate(5deg); opacity: 1; }

        .btn-main { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; width: 100%; border-radius: 25px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 12px; margin-top: 20px; border: none; font-size: 1.1rem; cursor: pointer; transition: 0.3s; }
        .btn-main:hover { box-shadow: 0 10px 30px rgba(0, 242, 254, 0.4); transform: scale(1.02); }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay-mesh"></div>

    <a href="https://wa.me/923332637235" class="wa-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div class="trust-badge"><i class="fas fa-check-circle"></i> Verified Official Partner</div>
            <div class="profile-pic-container">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
                <div class="status-dot"></div>
            </div>
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p id="typewriter" style="font-size: 1.1rem; min-height: 25px; margin-top: 10px; font-weight: 300; opacity: 0.9;"></p>
            
            <div style="display: flex; justify-content: center; gap: 20px; margin-top: 30px; font-size: 0.8rem; opacity: 0.6;">
                <span><i class="fas fa-star" style="color: gold;"></i> 5.0 Rating</span>
                <span><i class="fas fa-globe-americas" style="color: var(--primary);"></i> Global Delivery</span>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 25px; font-weight: 800; letter-spacing: 1px;">Expertise</h3>
            <div class="service-item">
                <div class="service-icon"><i class="fas fa-code"></i></div>
                <div><h4 style="font-size: 1rem;">Full-Stack Development</h4><p style="font-size: 0.75rem; opacity: 0.6;">High-speed web applications & dashboards.</p></div>
            </div>
            <div class="service-item">
                <div class="service-icon"><i class="fas fa-bezier-curve"></i></div>
                <div><h4 style="font-size: 1rem;">UI/UX Design</h4><p style="font-size: 0.75rem; opacity: 0.6;">Extra modern glassmorphism aesthetics.</p></div>
            </div>
            <div class="service-item">
                <div class="service-icon"><i class="fas fa-shield-virus"></i></div>
                <div><h4 style="font-size: 1rem;">Cyber Trust & SEO</h4><p style="font-size: 0.75rem; opacity: 0.6;">Secure branding & Google ranking mastery.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="background: linear-gradient(rgba(255,255,255,0.05), rgba(0, 242, 254, 0.05)); border-bottom: 6px solid var(--primary);">
            <h2 style="text-align: center; margin-bottom: 10px; font-weight: 800;">Let's Build The Future</h2>
            <p style="text-align: center; font-size: 0.8rem; opacity: 0.7; margin-bottom: 25px;">Prime Solutions provides 100% data security and money-back guarantee.</p>
            <a href="https://wa.me/923332637235" class="btn-main">
                <i class="fas fa-bolt"></i> Start Project Now
            </a>
            <p style="text-align: center; font-size: 0.7rem; margin-top: 15px; opacity: 0.4;">Active 24/7 for Client Support</p>
        </div>

        <footer style="text-align: center; font-size: 0.8rem; opacity: 0.2; letter-spacing: 2px;">
            PRIME SOLUTIONS © 2026 | BUILT BY NAZIM
        </footer>
    </div>

    <nav class="nav-bar">
        <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope-open-text"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1200, once: true });

        // High-End Typewriter
        const text = document.getElementById('typewriter');
        const phrases = ["Digital Architect", "Founder Prime Solutions", "UI/UX Visionary", "Firebase Expert"];
        let i = 0; let j = 0; let isDeleting = false;

        function typeEffect() {
            const current = phrases[i];
            if (isDeleting) {
                text.innerHTML = current.substring(0, j - 1);
                j--;
            } else {
                text.innerHTML = current.substring(0, j + 1);
                j++;
            }

            if (!isDeleting && j === current.length) {
                isDeleting = true;
                setTimeout(typeEffect, 2000);
            } else if (isDeleting && j === 0) {
                isDeleting = false;
                i = (i + 1) % phrases.length;
                setTimeout(typeEffect, 500);
            } else {
                setTimeout(typeEffect, isDeleting ? 50 : 100);
            }
        }
        window.onload = typeEffect;
    </script>
</body>
</html>
