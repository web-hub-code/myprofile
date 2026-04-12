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
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        /* Multi-Page Navigation */
        .top-nav { position: fixed; top: 0; width: 100%; z-index: 2000; background: rgba(0,0,0,0.85); backdrop-filter: blur(20px); border-bottom: 1px solid var(--border); padding: 15px 0; }
        .nav-container { max-width: 500px; margin: 0 auto; display: flex; justify-content: space-around; font-size: 0.75rem; font-weight: 600; text-transform: uppercase; }
        .nav-item { cursor: pointer; color: rgba(255,255,255,0.6); transition: 0.3s; }
        .nav-item.active { color: var(--primary); }

        #progress-bar { position: fixed; top: 52px; left: 0; width: 0%; height: 3px; background: var(--primary); z-index: 2001; }
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }

        .container { width: 100%; max-width: 500px; margin: 80px auto 120px; padding: 20px 15px; }

        .page { display: none; animation: fadeIn 0.5s ease; }
        .page.active { display: block; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        .card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 25px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }

        /* Hero Styling */
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }

        /* Stats & Lists */
        .stats-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; margin: 20px 0; }
        .stat-item { background: rgba(255,255,255,0.03); padding: 15px 5px; border-radius: 20px; text-align: center; border: 1px solid var(--border); }
        .stat-item h2 { color: var(--primary); font-size: 1.3rem; }

        /* Buttons */
        .btn-main { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; border: none; font-size: 1rem; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; text-decoration: none; }
        .btn-whatsapp { background: #25d366; color: white; margin-top: 10px; }

        /* Footer Navigation */
        .bottom-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 380px; background: rgba(10, 10, 10, 0.9); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .bottom-link { color: white; opacity: 0.6; font-size: 1.3rem; transition: 0.3s; }
        .bottom-link:hover { color: var(--primary); opacity: 1; }
    </style>
</head>
<body>

    <div id="progress-bar"></div>
    <nav class="top-nav">
        <div class="nav-container">
            <span class="nav-item active" onclick="showPage('home')">Home</span>
            <span class="nav-item" onclick="showPage('services')">Services</span>
            <span class="nav-item" onclick="showPage('portfolio')">Projects</span>
            <span class="nav-item" onclick="showPage('contact')">Contact</span>
        </div>
    </nav>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <div class="container">
        
        <div id="home" class="page active">
            <section class="card" style="text-align: center;" data-aos="zoom-in">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
                <h1 class="gradient-text">Muhammad Nazim</h1>
                <p style="opacity: 0.8; font-weight: 300;">Founder & Owner | Prime Solutions</p>
                
                <div class="stats-grid">
                    <div class="stat-item"><h2>50+</h2><p style="font-size: 0.5rem;">PROJECTS</p></div>
                    <div class="stat-item"><h2>15+</h2><p style="font-size: 0.5rem;">CLIENTS</p></div>
                    <div class="stat-item"><h2>5★</h2><p style="font-size: 0.5rem;">RATING</p></div>
                </div>
            </section>

            <div class="card" data-aos="fade-up">
                <h3><i class="fas fa-quote-left" style="color: var(--accent);"></i> Client Feedback</h3>
                <p style="font-style: italic; font-size: 0.85rem; opacity: 0.8; margin-top: 10px; border-left: 3px solid var(--primary); padding-left: 15px;">
                    "Nazim built our business site in just 3 days. The speed and design are top-notch! Highly recommended."
                </p>
                <p style="font-size: 0.6rem; text-align: right; margin-top: 5px; opacity: 0.5;">— CEO, TechStream Agency</p>
            </div>
        </div>

        <div id="services" class="page">
            <h2 style="text-align: center; margin-bottom: 25px;">Prime Services</h2>
            <div class="card" data-aos="fade-up">
                <i class="fas fa-rocket" style="font-size: 2rem; color: var(--primary);"></i>
                <h4 style="margin-top: 15px;">Elite Development</h4>
                <p style="font-size: 0.8rem; opacity: 0.7; margin-top: 5px;">React, HTML, aur JavaScript ke sath fast aur secure websites.</p>
            </div>
            <div class="card" data-aos="fade-up">
                <i class="fas fa-search-dollar" style="font-size: 2rem; color: var(--primary);"></i>
                <h4 style="margin-top: 15px;">SEO Mastery</h4>
                <p style="font-size: 0.8rem; opacity: 0.7; margin-top: 5px;">Google ranking aur organic traffic barhane ke expert solutions.</p>
            </div>
        </div>

        <div id="portfolio" class="page">
            <h2 style="text-align: center; margin-bottom: 25px;">Live Masterpieces</h2>
            <div class="card" style="display: flex; justify-content: space-between; align-items: center;">
                <div><h4>Pakgold</h4><p style="font-size: 0.6rem; opacity: 0.5;">Investment Portal</p></div>
                <i class="fas fa-external-link-alt" style="color: var(--primary);"></i>
            </div>
            <div class="card" style="display: flex; justify-content: space-between; align-items: center;">
                <div><h4>Web-Hub</h4><p style="font-size: 0.6rem; opacity: 0.5;">Official Agency Site</p></div>
                <i class="fas fa-external-link-alt" style="color: var(--primary);"></i>
            </div>
        </div>

        <div id="contact" class="page">
            <div class="card">
                <h3 style="text-align: center; margin-bottom: 20px;">Get In Touch</h3>
                <a href="https://wa.me/923332637235" class="btn-main btn-whatsapp" target="_blank">
                    <i class="fab fa-whatsapp"></i> WhatsApp Consultation
                </a>
                <a href="tel:03705519562" class="btn-main" style="margin-top: 15px; background: rgba(255,255,255,0.05); color: white; border: 1px solid var(--primary);">
                    <i class="fas fa-phone-alt"></i> Call: 0370 5519562
                </a>
                <a href="mailto:webhub262@gmail.com" class="btn-main" style="margin-top: 15px; background: none; color: var(--primary); border: 1px solid var(--border);">
                    <i class="fas fa-envelope"></i> Email Us Directly
                </a>
            </div>
            
            <div class="card" style="text-align: center;">
                <h4 style="margin-bottom: 15px;">Follow Our Journey</h4>
                <div style="display: flex; justify-content: center; gap: 25px; font-size: 1.5rem;">
                    <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" style="color: #1877F2;"><i class="fab fa-facebook"></i></a>
                    <a href="#" style="color: #E4405F;"><i class="fab fa-instagram"></i></a>
                    <a href="#" style="color: white;"><i class="fab fa-github"></i></a>
                </div>
            </div>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.4;">
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED
        </footer>
    </div>

    <nav class="bottom-bar">
        <a href="#" class="bottom-link" onclick="showPage('home')"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="bottom-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="bottom-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="bottom-link"><i class="fas fa-envelope"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            document.querySelectorAll('.nav-item').forEach(n => n.classList.remove('active'));
            
            document.getElementById(pageId).classList.add('active');
            // Update top nav active state
            const items = document.querySelectorAll('.nav-item');
            if(pageId === 'home') items[0].classList.add('active');
            if(pageId === 'services') items[1].classList.add('active');
            if(pageId === 'portfolio') items[2].classList.add('active');
            if(pageId === 'contact') items[3].classList.add('active');
            
            window.scrollTo(0,0);
        }

        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
        };
    </script>
</body>
</html>
