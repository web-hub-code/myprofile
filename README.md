<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Digital Architect</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #020406; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.2); }
        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 15px 15px 100px; }
        
        /* Professional Cards */
        .card { background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--border); border-radius: 25px; padding: 22px; margin-bottom: 20px; }
        
        .hero { text-align: center; padding: 45px 15px; }
        .profile-pic { width: 125px; height: 125px; border-radius: 50%; border: 3px solid var(--primary); object-fit: cover; box-shadow: 0 0 25px var(--primary); margin-bottom: 15px; }
        h1 { font-size: 2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Form Styling */
        input, textarea { width: 100%; padding: 12px; margin-top: 10px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); border-radius: 12px; color: white; outline: none; }
        .submit-btn { width: 100%; padding: 15px; border-radius: 12px; border: none; background: linear-gradient(45deg, var(--primary), var(--secondary)); color: white; font-weight: bold; margin-top: 15px; cursor: pointer; box-shadow: 0 5px 15px rgba(0, 242, 254, 0.2); }

        /* Services List */
        .service-item { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; }
        .service-icon { width: 45px; height: 45px; background: rgba(0,242,254,0.1); border-radius: 12px; display: flex; align-items: center; justify-content: center; color: var(--primary); }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 15px; left: 50%; transform: translateX(-50%); width: 92%; background: rgba(0,0,0,0.8); backdrop-filter: blur(20px); border-radius: 30px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 12px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.1rem; }

        footer { text-align: center; opacity: 0.4; font-size: 0.75rem; padding-top: 10px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="https://wa.me/923000000000" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Muhammad Nazim</h1>
            <p style="font-size: 0.85rem; opacity: 0.8; margin-top: 5px;">Prime Solutions | Tech Expert</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; color: var(--primary);">What I Offer</h3>
            <div class="service-item">
                <div class="service-icon"><i class="fas fa-laptop-code"></i></div>
                <div><p style="font-weight: 600;">Web Development</p><p style="font-size: 0.7rem; opacity: 0.6;">Modern & Responsive Websites</p></div>
            </div>
            <div class="service-item">
                <div class="service-icon"><i class="fas fa-magic"></i></div>
                <div><p style="font-weight: 600;">UI/UX Design</p><p style="font-size: 0.7rem; opacity: 0.6;">Creative & Clean Interfaces</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px; color: var(--accent);">Get In Touch</h3>
            <form action="mailto:webhub262@gmail.com" method="post" enctype="text/plain">
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea rows="4" placeholder="How can I help you?"></textarea>
                <button type="submit" class="submit-btn">Send Message</button>
            </form>
        </div>

        <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-bottom: 20px;">
            <a href="https://wa.me/923000000000" class="card" style="text-align: center; margin-bottom: 0; text-decoration: none; color: white; padding: 15px;">
                <i class="fab fa-whatsapp" style="font-size: 1.5rem; color: #25d366;"></i>
                <p style="font-size: 0.8rem; margin-top: 5px;">WhatsApp</p>
            </a>
            <a href="tel:+923000000000" class="card" style="text-align: center; margin-bottom: 0; text-decoration: none; color: white; padding: 15px;">
                <i class="fas fa-phone-alt" style="font-size: 1.5rem; color: var(--primary);"></i>
                <p style="font-size: 0.8rem; margin-top: 5px;">Call Now</p>
            </a>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | BUILT FOR SUCCESS</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 800, once: true });</script>
</body>
</html>
