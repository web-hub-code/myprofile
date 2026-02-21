<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Official Portfolio</title>
    
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

        /* Background Video */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.2); }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 120px; }

        /* Modern Cards */
        .card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; transition: 0.3s; }
        
        .hero { text-align: center; padding: 50px 20px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: 0 0 35px var(--primary); margin-bottom: 15px; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }

        /* Rating Stars */
        .rating { color: #ffd700; margin-top: 10px; font-size: 1.2rem; }

        /* Image Gallery */
        .img-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 15px; }
        .grid-img { width: 100%; height: 120px; border-radius: 20px; object-fit: cover; border: 1px solid var(--border); }

        /* Service Badges */
        .service-tag { display: inline-block; padding: 8px 16px; background: rgba(0, 242, 254, 0.1); border: 1px solid var(--primary); border-radius: 50px; font-size: 0.8rem; margin: 5px; }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 92%; background: rgba(0,0,0,0.85); backdrop-filter: blur(25px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.3rem; }

        .btn-call { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 20px; font-weight: 800; cursor: pointer; font-size: 1rem; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.3); margin-top: 10px; text-decoration: none; display: block; text-align: center; }
        
        footer { text-align: center; font-size: 0.75rem; opacity: 0.4; margin-top: 20px; }
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
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p style="opacity: 0.8;">Founder of Prime Solutions</p>
            <div class="rating">
                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i>
                <span style="font-size: 0.7rem; color: white; opacity: 0.6;"> (4.9/5 Client Rating)</span>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> My Expertise</h3>
            <span class="service-tag">Web Development</span>
            <span class="service-tag">UI/UX Design</span>
            <span class="service-tag">Digital Branding</span>
            <span class="service-tag">SEO Mastery</span>
            <span class="service-tag">App Solutions</span>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 10px;"><i class="fas fa-images"></i> Prime Works</h3>
            <div class="img-grid">
                <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=400" class="grid-img">
                <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?w=400" class="grid-img">
            </div>
            <p style="font-size: 0.8rem; margin-top: 15px; line-height: 1.6; opacity: 0.8;">
                Hum "Prime Solutions" mein futuristic digital experiences banate hain jo aapke business ko next level par le jaate hain.
            </p>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-headset"></i> Get In Touch</h3>
            <p style="font-size: 0.85rem; opacity: 0.7; margin-bottom: 20px;">Directly contact me for high-quality digital services.</p>
            <a href="https://wa.me/923332637235" class="btn-call">Chat on WhatsApp</a>
            <a href="tel:+923332637235" style="display: block; text-align: center; margin-top: 15px; color: var(--primary); text-decoration: none; font-size: 0.9rem;">
                <i class="fas fa-phone"></i> +92 333 2637235
            </a>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | BUILT WITH PASSION</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 800, once: true });</script>
</body>
</html>
