<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Prime Solutions | International Tech Agency</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Multi-Page Navigation Bar */
        .top-nav { position: fixed; top: 0; width: 100%; z-index: 2000; background: rgba(0,0,0,0.8); backdrop-filter: blur(20px); border-bottom: 1px solid var(--border); padding: 15px 0; }
        .nav-container { max-width: 480px; margin: 0 auto; display: flex; justify-content: space-around; font-size: 0.7rem; font-weight: 600; text-transform: uppercase; letter-spacing: 1px; }
        .nav-item { cursor: pointer; color: rgba(255,255,255,0.6); transition: 0.3s; }
        .nav-item.active { color: var(--primary); }

        #progress-bar { position: fixed; top: 50px; left: 0; width: 0%; height: 3px; background: var(--primary); z-index: 2001; }
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }

        .container { width: 100%; max-width: 480px; margin: 70px auto 120px; padding: 20px 15px; }

        /* Pages */
        .page { display: none; }
        .page.active { display: block; }

        /* Stats Section */
        .stats-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; margin-bottom: 30px; }
        .stat-card { background: var(--glass); padding: 20px 10px; border-radius: 20px; text-align: center; border: 1px solid var(--border); }
        .stat-card h2 { color: var(--primary); font-size: 1.5rem; }

        /* Service Cards */
        .service-list { display: grid; gap: 15px; }
        .service-card { background: var(--glass); border: 1px solid var(--border); border-radius: 25px; padding: 25px; transition: 0.4s; }
        .service-card i { font-size: 2rem; color: var(--primary); margin-bottom: 15px; }

        /* Forms */
        .form-input { width: 100%; padding: 18px; border-radius: 20px; border: 1px solid var(--border); background: rgba(255,255,255,0.02); color: white; margin-bottom: 15px; outline: none; }
        .btn-mega { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; width: 100%; border-radius: 20px; font-weight: 800; border: none; font-size: 1rem; cursor: pointer; }

        .footer-info { text-align: center; margin-top: 40px; padding-top: 20px; border-top: 1px solid var(--border); font-size: 0.7rem; opacity: 0.4; }
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
            <section style="text-align: center; margin-bottom: 40px;" data-aos="zoom-in">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" style="width: 140px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px;">
                <h1 style="font-size: 2.2rem; margin-top: 20px;">Muhammad Nazim</h1>
                <p style="color: var(--primary); font-weight: 300; letter-spacing: 2px;">FOUNDER & OWNER</p>
            </section>

            <div class="stats-grid" data-aos="fade-up">
                <div class="stat-card"><h2>500+</h2><p style="font-size: 0.5rem;">GLOBAL CLIENTS</p></div>
                <div class="stat-card"><h2>98%</h2><p style="font-size: 0.5rem;">SUCCESS RATE</p></div>
                <div class="stat-card"><h2>24/7</h2><p style="font-size: 0.5rem;">TECH SUPPORT</p></div>
            </div>

            <div class="service-card" data-aos="fade-up">
                <h3>Our Mission</h3>
                <p style="font-size: 0.8rem; opacity: 0.7; margin-top: 10px; line-height: 1.6;">Prime Solutions ka maqsad har business ko digital dunya ka titan banana hai. Hum sirf code nahi karte, hum brand banate hain.</p>
                <button onclick="showPage('contact')" style="margin-top: 15px; background: none; border: 1px solid var(--primary); color: var(--primary); padding: 10px 20px; border-radius: 50px; font-size: 0.7rem;">WORK WITH US</button>
            </div>
        </div>

        <div id="services" class="page">
            <h2 style="margin-bottom: 25px; text-align: center; color: var(--primary);">Exclusive Services</h2>
            <div class="service-list">
                <div class="service-card">
                    <i class="fas fa-code"></i>
                    <h4>Elite Web Architecture</h4>
                    <p style="font-size: 0.7rem; opacity: 0.6; margin-top: 5px;">React, Node, aur Firebase par mabni super-fast websites.</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-paint-brush"></i>
                    <h4>Next-Gen UI/UX</h4>
                    <p style="font-size: 0.7rem; opacity: 0.6; margin-top: 5px;">Aisa design jo users ko dekhte hi pasand aa jaye.</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-chart-line"></i>
                    <h4>SEO Dominance</h4>
                    <p style="font-size: 0.7rem; opacity: 0.6; margin-top: 5px;">Google search ke pehle page par aapka raaj.</p>
                </div>
            </div>
        </div>

        <div id="contact" class="page">
            <div class="service-card">
                <h2 style="text-align: center; margin-bottom: 20px;">Book a Consultation</h2>
                <form id="megaForm">
                    <input type="text" placeholder="Full Name" class="form-input" required>
                    <input type="email" placeholder="Business Email" class="form-input" required>
                    <select class="form-input" style="background: #0a0a0a;">
                        <option>Choose Project Type</option>
                        <option>E-Commerce Store</option>
                        <option>Portfolio / Blog</option>
                        <option>Custom Web App</option>
                    </select>
                    <textarea placeholder="Tell us about your project..." rows="4" class="form-input"></textarea>
                    <button type="submit" class="btn-mega">START JOURNEY</button>
                </form>
            </div>
        </div>

        <div class="footer-info">
            <div style="margin-bottom: 10px;">
                <i class="fab fa-whatsapp"></i> +92 333 2637235 | <i class="fas fa-envelope"></i> webhub262@gmail.com
            </div>
            PRIME SOLUTIONS © 2026 | ALL RIGHTS RESERVED
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init();

        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            document.querySelectorAll('.nav-item').forEach(n => n.classList.remove('active'));
            
            document.getElementById(pageId).classList.add('active');
            event.target.classList.add('active');
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
