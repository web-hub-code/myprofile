<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Founder & Owner Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #4facfe; --secondary: #00f2fe; --accent: #f093fb;
            --bg: #f8f9fa; --text: #1a1a1a; --glass: rgba(255, 255, 255, 0.7); --border: rgba(0, 0, 0, 0.05);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        /* Animated Soft Background */
        .bg-gradient { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: linear-gradient(120deg, #e0f7fa 0%, #ffffff 100%); }
        .mesh-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-image: radial-gradient(var(--primary) 0.5px, transparent 0.5px); background-size: 40px 40px; opacity: 0.1; z-index: -1; }

        .container { width: 100%; max-width: 500px; margin: 20px auto 120px; padding: 20px 15px; }

        /* Premium Glass Card */
        .card { 
            background: var(--glass); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px);
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 30px; margin-bottom: 25px; transition: 0.5s cubic-bezier(0.2, 1, 0.3, 1);
            box-shadow: 0 10px 30px rgba(0,0,0,0.03);
        }
        .card:hover { transform: translateY(-8px); border-color: var(--primary); box-shadow: 0 20px 40px rgba(79, 172, 254, 0.1); }

        /* Hero Section */
        .hero { text-align: center; padding: 40px 10px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid #fff; box-shadow: 0 10px 25px rgba(0,0,0,0.1); margin-bottom: 20px; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.5rem; letter-spacing: -1px; }

        /* Dynamic Stats */
        .stats-grid { display: flex; justify-content: space-around; margin: 25px 0; }
        .stat-box h2 { color: var(--primary); font-size: 1.8rem; font-weight: 800; }
        .stat-box p { font-size: 0.6rem; text-transform: uppercase; letter-spacing: 1px; opacity: 0.6; }

        /* Service Badges */
        .service-tag { background: rgba(79, 172, 254, 0.1); color: var(--primary); padding: 8px 15px; border-radius: 50px; font-size: 0.75rem; font-weight: 600; display: inline-block; margin: 5px; }

        /* Main CTA Buttons */
        .btn-call { background: var(--primary); color: white; padding: 20px; width: 100%; border-radius: 25px; font-weight: 800; display: flex; align-items: center; justify-content: center; gap: 12px; text-decoration: none; margin-top: 15px; transition: 0.3s; box-shadow: 0 10px 20px rgba(79, 172, 254, 0.2); }
        .btn-call:hover { transform: scale(1.02); filter: brightness(1.1); }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 400px; background: rgba(255,255,255,0.8); backdrop-filter: blur(15px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 15px 35px rgba(0,0,0,0.05); }
        .nav-link { color: #555; font-size: 1.4rem; transition: 0.3s; }
        .nav-link:hover { color: var(--primary); transform: scale(1.2); }
    </style>
</head>
<body>

    <div class="bg-gradient"></div>
    <div class="mesh-overlay"></div>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div style="background: rgba(79, 172, 254, 0.1); color: var(--primary); display: inline-block; padding: 5px 15px; border-radius: 50px; font-size: 0.6rem; font-weight: 800; margin-bottom: 20px;">OFFICIAL PRIME AGENCY PORTAL</div>
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="font-size: 1rem; opacity: 0.7; font-weight: 400; margin-top: 5px;">Founder & Owner | Prime Solutions</p>
            
            <div class="stats-grid">
                <div class="stat-box"><h2>50+</h2><p>Projects</p></div>
                <div class="stat-box"><h2>15+</h2><p>Countries</p></div>
                <div class="stat-box"><h2>100%</h2><p>Success</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-layer-group" style="color: var(--primary);"></i> Premium Solutions</h3>
            <div class="service-tag">Full Stack Web</div>
            <div class="service-tag">UI/UX Design</div>
            <div class="service-tag">Google SEO</div>
            <div class="service-tag">Firebase Auth</div>
            <div class="service-tag">Mobile Apps</div>
            <div class="service-tag">API Security</div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-bolt"></i> Elite Workflow</h3>
            <div style="display: flex; gap: 15px; margin-bottom: 15px;">
                <div style="background: var(--primary); color: white; width: 30px; height: 30px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 800;">1</div>
                <p style="font-size: 0.85rem; padding-top: 5px;"><b>Consultation:</b> Idea ko business mein badalna.</p>
            </div>
            <div style="display: flex; gap: 15px; margin-bottom: 15px;">
                <div style="background: var(--primary); color: white; width: 30px; height: 30px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 800;">2</div>
                <p style="font-size: 0.85rem; padding-top: 5px;"><b>Dev:</b> Modern coding with high-end security.</p>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-left: 5px solid var(--primary);">
            <h3><i class="fas fa-shield-alt" style="color: var(--primary);"></i> Why Trust Us?</h3>
            <p style="font-size: 0.8rem; opacity: 0.7; margin-top: 10px; line-height: 1.6;">
                Prime Solutions sirf code nahi karta, hum aapka bharosa jeet-te hain. 100% Privacy aur 24/7 Dedicated Support ke sath hum har project ko master-piece banate hain.
            </p>
        </div>

        <div class="card" data-aos="fade-up" style="background: linear-gradient(135deg, #ffffff, #f0f7ff);">
            <h3 style="text-align: center; margin-bottom: 15px;">Start Your Project</h3>
            <a href="https://wa.me/923332637235" class="btn-call" style="background: #25d366;">
                <i class="fab fa-whatsapp"></i> WhatsApp Chat
            </a>
            <a href="tel:03705519562" class="btn-call">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
        </div>

        <footer style="text-align: center; font-size: 0.75rem; opacity: 0.5; margin-top: 30px;">
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED<br>
            Designed with <i class="fas fa-heart" style="color: var(--accent);"></i> by Nazim
        </footer>
    </div>

    <nav class="bottom-nav">
        <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope-open"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1200, once: true });
    </script>
</body>
</html>
