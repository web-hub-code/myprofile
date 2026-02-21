<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Official</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --accent: #f093fb;
            --bg: #030508;
            --glass: rgba(255, 255, 255, 0.05);
            --border: rgba(255, 255, 255, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Scroll Progress Bar */
        #progress-container { position: fixed; top: 0; width: 100%; height: 4px; z-index: 1000; }
        #progress-bar { height: 100%; background: linear-gradient(90deg, var(--primary), var(--accent)); width: 0%; }

        /* Video Background */
        #bg-video { position: fixed; top: 0; left: 0; min-width: 100%; min-height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.3); }

        .container { max-width: 900px; margin: 0 auto; padding: 15px 15px 100px; }

        /* Hero Section */
        .hero {
            background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--border);
            border-radius: 30px; padding: 50px 20px; text-align: center; margin-top: 30px;
        }

        .profile-container { position: relative; width: 150px; height: 150px; margin: 0 auto 20px; }
        .profile-pic {
            width: 100%; height: 100%; border-radius: 50%; border: 4px solid var(--primary);
            object-fit: cover; box-shadow: 0 0 30px var(--primary);
        }

        h1 { font-size: clamp(1.8rem, 8vw, 3.5rem); font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Bottom Nav (Mobile App Look) */
        .bottom-nav {
            position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%);
            width: 90%; max-width: 400px; background: rgba(0,0,0,0.7);
            backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border);
            display: flex; justify-content: space-around; padding: 15px; z-index: 1000;
        }
        .nav-item { color: white; font-size: 1.2rem; text-decoration: none; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); transform: translateY(-5px); }

        /* Skills Card */
        .card { background: var(--glass); border: 1px solid var(--border); border-radius: 20px; padding: 25px; margin-top: 20px; backdrop-filter: blur(15px); }
        .skill-tag { display: inline-block; padding: 8px 15px; background: rgba(0, 242, 254, 0.1); border: 1px solid var(--primary); border-radius: 50px; margin: 5px; font-size: 0.8rem; }

        /* Floating WhatsApp */
        .whatsapp-btn { position: fixed; bottom: 100px; right: 20px; background: #25d366; width: 55px; height: 55px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.8rem; color: white; box-shadow: 0 10px 20px rgba(0,0,0,0.3); z-index: 900; }

        /* Image Gallery Look */
        .gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(140px, 1fr)); gap: 15px; margin-top: 20px; }
        .gal-img { width: 100%; height: 150px; border-radius: 15px; object-fit: cover; border: 1px solid var(--border); }

        footer { text-align: center; margin-top: 50px; opacity: 0.5; font-size: 0.8rem; letter-spacing: 2px; }
    </style>
</head>
<body>

    <div id="progress-container"><div id="progress-bar"></div></div>
    
    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
        <a href="https://wa.me/923000000000" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.instagram.com/mr_nazim073" target="_blank" class="nav-item"><i class="fab fa-instagram"></i></a>
    </nav>

    <div class="container">
        <section class="hero" data-aos="zoom-in">
            <div class="profile-container">
                <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            </div>
            <h1>Muhammad Nazim</h1>
            <p style="margin-top: 10px; color: var(--primary); letter-spacing: 3px; font-weight: 300;">PRO WEB DEVELOPER</p>
        </section>

        <div class="card" style="display: flex; justify-content: space-around; text-align: center;" data-aos="fade-up">
            <div><h2 style="color: var(--primary);">40+</h2><p style="font-size: 0.7rem;">Projects</p></div>
            <div><h2 style="color: var(--accent);">100%</h2><p style="font-size: 0.7rem;">Quality</p></div>
            <div><h2 style="color: #25d366;">Active</h2><p style="font-size: 0.7rem;">Status</p></div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-tools"></i> Core Skills</h3>
            <div style="margin-top: 15px;">
                <span class="skill-tag">Mobile First Design</span>
                <span class="skill-tag">UI/UX Animation</span>
                <span class="skill-tag">SEO Expert</span>
                <span class="skill-tag">AI Integration</span>
            </div>
        </div>

        <h3 style="margin: 30px 0 10px 10px;">Portfolio Gallery</h3>
        <div class="gallery" data-aos="fade-up">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=300" class="gal-img">
            <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?w=300" class="gal-img">
            <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=300" class="gal-img">
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | DESIGNED FOR THE FUTURE</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Scroll Progress Logic
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("progress-bar").style.width = scrolled + "%";
        };
    </script>
</body>
</html>
