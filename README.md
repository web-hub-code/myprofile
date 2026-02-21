<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>Muhammad Nazim | Web Developer & Creative Designer</title>
    <meta name="description" content="Official portfolio of Muhammad Nazim. Specialized in modern web development, UI/UX design, and digital solutions.">
    <meta name="keywords" content="Muhammad Nazim, Web Developer, Prime Solutions, Portfolio, UI/UX Designer, Muhammad Nazim GitHub">
    <meta name="author" content="Muhammad Nazim">

    <meta property="og:title" content="Muhammad Nazim | Professional Portfolio">
    <meta property="og:description" content="Check out my latest web projects and digital solutions.">
    <meta property="og:image" content="Snapchat-2096615446.jpg">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    
    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: rgba(3, 5, 8, 0.9); --card-bg: rgba(255, 255, 255, 0.05);
            --text: #ffffff; --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: #000; color: var(--text); overflow-x: hidden; scroll-behavior: smooth; }
        #bg-video { position: fixed; top: 0; left: 0; min-width: 100%; min-height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.3); }
        .container { max-width: 900px; margin: 0 auto; padding: 20px; position: relative; }
        .card { background: var(--card-bg); padding: 30px; border-radius: 25px; border: 1px solid var(--border); backdrop-filter: blur(15px); margin-bottom: 25px; }
        .hero { text-align: center; padding: 60px 20px; margin-top: 30px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); object-fit: cover; box-shadow: 0 0 30px var(--primary); margin-bottom: 20px; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: clamp(2rem, 8vw, 3.5rem); }
        .whatsapp-float { position: fixed; bottom: 25px; left: 25px; background: #25d366; color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 30px; z-index: 100; text-decoration: none; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.3); }
        .skill-bar { height: 8px; background: rgba(255,255,255,0.1); border-radius: 10px; margin: 10px 0 20px; overflow: hidden; }
        .skill-fill { height: 100%; background: linear-gradient(90deg, var(--primary), var(--secondary)); }
        footer { text-align: center; padding: 40px 0; opacity: 0.5; font-size: 0.8rem; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <a href="https://wa.me/923000000000" class="whatsapp-float" target="_blank"><i class="fab fa-whatsapp"></i></a>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="letter-spacing: 2px; opacity: 0.8;">EXPERTISE IN MODERN WEB SOLUTIONS</p>
        </section>

        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
            <div class="card" data-aos="fade-right">
                <h3 style="margin-bottom: 20px; color: var(--primary);">Skills & Tech</h3>
                <p>Web Development</p><div class="skill-bar"><div class="skill-fill" style="width: 90%;"></div></div>
                <p>Digital Branding</p><div class="skill-bar"><div class="skill-fill" style="width: 85%;"></div></div>
            </div>

            <div class="card" data-aos="fade-left">
                <h3 style="margin-bottom: 20px; color: var(--accent);">Direct Connect</h3>
                <p style="margin-bottom: 15px;">Available for professional collaborations.</p>
                <a href="mailto:webhub262@gmail.com" style="color: var(--primary); text-decoration: none; font-weight: bold;"><i class="fas fa-envelope"></i> webhub262@gmail.com</a>
            </div>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | GOOGLE OPTIMIZED PORTFOLIO</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
