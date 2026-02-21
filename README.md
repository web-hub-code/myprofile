<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Digital Pro</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.2); }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 120px; }

        /* Modern Glass Card */
        .card { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; }

        .hero { text-align: center; padding: 40px 15px; }
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); box-shadow: 0 0 30px var(--primary); margin-bottom: 15px; }
        
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.2rem; }

        /* Project Slider (Horizontal) */
        .project-slider { display: flex; overflow-x: auto; gap: 15px; padding-bottom: 10px; scrollbar-width: none; }
        .project-slider::-webkit-scrollbar { display: none; }
        .project-card { min-width: 200px; height: 120px; background: rgba(255,255,255,0.05); border-radius: 20px; display: flex; align-items: center; justify-content: center; border: 1px solid var(--border); font-size: 0.8rem; text-align: center; padding: 10px; }

        /* Live Counter Badge */
        .live-badge { display: inline-block; padding: 5px 12px; background: rgba(0, 255, 0, 0.1); border: 1px solid #00ff00; border-radius: 50px; color: #00ff00; font-size: 0.7rem; margin-bottom: 10px; }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 92%; background: rgba(0,0,0,0.85); backdrop-filter: blur(20px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.2rem; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); transform: scale(1.2); }

        .btn-hire { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 20px; font-weight: 800; cursor: pointer; font-size: 1rem; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.3); }

        footer { text-align: center; font-size: 0.75rem; opacity: 0.4; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-paper-plane"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div class="live-badge">🟢 LIVE: 24 PEOPLE VIEWING</div>
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1 id="greeting" style="font-size: 1rem; font-weight: 400; opacity: 0.8;">Hello!</h1>
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="margin-top: 5px; color: var(--primary); letter-spacing: 2px; font-size: 0.7rem;">CEO, PRIME SOLUTIONS</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; font-size: 1rem;"><i class="fas fa-layer-group"></i> My Recent Work</h3>
            <div class="project-slider">
                <div class="project-card">E-Commerce App</div>
                <div class="project-card">Brand Identity</div>
                <div class="project-card">Modern UI Kit</div>
                <div class="project-card">AI Web Tool</div>
            </div>
            <p style="font-size: 0.6rem; opacity: 0.5; margin-top: 10px; text-align: center;">← Swipe to see more →</p>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; font-size: 1rem;"><i class="fas fa-briefcase"></i> Solutions I Provide</h3>
            <div style="font-size: 0.85rem; line-height: 1.8; opacity: 0.9;">
                ✔ Premium Website Development<br>
                ✔ Professional Graphic Designing<br>
                ✔ Digital Marketing Strategy<br>
                ✔ 24/7 Technical Support
            </div>
        </div>

        <button class="btn-hire" onclick="location.href='https://wa.me/923332637235'">GET A FREE QUOTE</button>

        <footer style="margin-top: 30px;">© 2026 | MUHAMMAD NAZIM | PREMIER IDENTITY</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });

        // Dynamic Greeting
        const hour = new Date().getHours();
        const greeting = hour < 12 ? "Good Morning!" : hour < 18 ? "Good Afternoon!" : "Good Evening!";
        document.getElementById('greeting').innerText = greeting;
    </script>
</body>
</html>
