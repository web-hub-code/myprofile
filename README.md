<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global CEO - Prime Solutions Infinity</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        /* Animated Vision Background */
        .vision-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 500px; height: 500px; background: var(--primary); filter: blur(200px); opacity: 0.1; border-radius: 50%; animation: pulse 10s infinite alternate; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 140px; }

        /* Fake Live Notifications */
        #notify-box { position: fixed; top: 15px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 85%; max-width: 400px; display: none; }
        .notify { background: rgba(0, 0, 0, 0.95); border: 1px solid var(--primary); padding: 12px 18px; border-radius: 50px; backdrop-filter: blur(20px); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 40px rgba(0,242,254,0.3); animation: slideDown 0.6s cubic-bezier(0.17, 0.67, 0.83, 0.67); }
        @keyframes slideDown { from { transform: translateY(-100px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

        /* CEO Hero Hub */
        .ceo-hero { background: var(--glass); backdrop-filter: blur(35px); border: 1px solid var(--border); border-radius: 45px; padding: 40px 20px; text-align: center; position: relative; overflow: hidden; }
        .pfp-wrap { position: relative; width: 145px; height: 145px; margin: 0 auto 20px; }
        .pfp-main { width: 100%; height: 100%; border-radius: 50%; border: 3px solid var(--primary); padding: 6px; object-fit: cover; box-shadow: 0 0 50px rgba(0, 242, 254, 0.3); }
        .status-dot { position: absolute; bottom: 12px; right: 12px; width: 18px; height: 18px; background: #25d366; border-radius: 50%; border: 3px solid #000; animation: glow 1.5s infinite; }
        @keyframes glow { 0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7); } 70% { box-shadow: 0 0 0 10px rgba(37, 211, 102, 0); } 100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); } }

        /* Social Dock */
        .social-row { display: flex; justify-content: center; gap: 12px; margin-top: 25px; }
        .social-link { width: 42px; height: 42px; background: rgba(255,255,255,0.05); border-radius: 12px; display: flex; align-items: center; justify-content: center; color: white; text-decoration: none; border: 1px solid var(--border); transition: 0.3s; }
        .social-link:hover { background: var(--primary); color: #000; transform: translateY(-5px); border-color: var(--primary); }

        /* Infinity Cards */
        .card { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-top: 25px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }

        /* Service Matrix */
        .service-item { display: flex; align-items: center; gap: 15px; padding: 20px; background: rgba(255,255,255,0.02); border-radius: 25px; margin-bottom: 15px; border: 1px solid transparent; transition: 0.3s; text-decoration: none; color: white; }
        .service-item:hover { border-color: var(--primary); background: rgba(0,242,254,0.08); }
        .service-item i { font-size: 1.8rem; color: var(--primary); }

        /* Trust Engine (Reviews) */
        .review { background: rgba(0,0,0,0.2); padding: 15px; border-radius: 20px; margin-bottom: 12px; border-left: 3px solid var(--primary); }
        .stars { color: #f1c40f; font-size: 0.8rem; margin-bottom: 5px; }

        /* Floating Nav Dock */
        .nav-dock { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.9); backdrop-filter: blur(30px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 20px; z-index: 9999; box-shadow: 0 40px 80px rgba(0,0,0,0.7); }
        .dock-item { color: white; opacity: 0.35; font-size: 1.4rem; cursor: pointer; transition: 0.3s; }
        .dock-item.active { opacity: 1; color: var(--primary); transform: scale(1.2) translateY(-5px); }

        /* Mega CTA */
        .btn-mega { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; width: 100%; border-radius: 25px; font-weight: 800; border: none; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 20px; text-decoration: none; font-size: 1.1rem; }
        
        .section-view { display: none; }
        .section-view.active { display: block; animation: zoomReveal 0.6s ease; }
        @keyframes zoomReveal { from { opacity: 0; transform: scale(0.9); } to { opacity: 1; transform: scale(1); } }
    </style>
</head>
<body>

    <div class="vision-bg"><div class="glow"></div></div>

    <div id="notify-box">
        <div class="notify">
            <i class="fas fa-crown" style="color: var(--primary);"></i>
            <span id="alert-text" style="font-size: 0.75rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="container">
        
        <section id="view-home" class="section-view active">
            <div class="ceo-hero" data-aos="zoom-in">
                <div class="pfp-wrap">
                    <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-main" alt="Muhammad Nazim">
                    <div class="status-dot"></div>
                </div>
                <h1 style="font-size: 2.6rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
                <p style="opacity: 0.7; font-size: 0.9rem;">Global CEO | Prime Solutions Hub</p>
                
                <div class="social-row">
                    <a href="#" class="social-link"><i class="fab fa-facebook-f"></i></a>
                    <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" class="social-link"><i class="fab fa-github"></i></a>
                    <a href="#" class="social-link"><i class="fab fa-twitter"></i></a>
                </div>
            </div>

            <div class="card" data-aos="fade-up">
                <h3><i class="fas fa-chart-line" style="color: var(--primary);"></i> Global Influence</h3>
                <div style="display: flex; justify-content: space-around; margin-top: 25px; text-align: center;">
                    <div><h2 style="color: var(--primary);">150+</h2><p style="font-size: 0.55rem; opacity: 0.5; letter-spacing: 1px;">PROJECTS</p></div>
                    <div><h2 style="color: var(--primary);">50+</h2><p style="font-size: 0.55rem; opacity: 0.5; letter-spacing: 1px;">COUNTRIES</p></div>
                    <div><h2 style="color: var(--primary);">100%</h2><p style="font-size: 0.55rem; opacity: 0.5; letter-spacing: 1px;">TRUST</p></div>
                </div>
            </div>
        </section>

        <section id="view-services" class="section-view">
            <div class="card">
                <h3 style="margin-bottom: 25px;"><i class="fas fa-rocket"></i> Premium Services</h3>
                <a href="javascript:void(0)" onclick="navTo('contact')" class="service-item">
                    <i class="fas fa-vault"></i>
                    <div><h4>Investment Portals</h4><p style="font-size: 0.7rem; opacity: 0.5;">Secure financial branding & profit tracking.</p></div>
                </a>
                <a href="javascript:void(0)" onclick="navTo('contact')" class="service-item">
                    <i class="fas fa-shopping-cart"></i>
                    <div><h4>Elite E-Commerce</h4><p style="font-size: 0.7rem; opacity: 0.5;">Global shops with seamless payment gateways.</p></div>
                </a>
                <a href="javascript:void(0)" onclick="navTo('contact')" class="service-item">
                    <i class="fas fa-code-branch"></i>
                    <div><h4>Software Ecosystems</h4><p style="font-size: 0.7rem; opacity: 0.5;">Custom business logic & management tools.</p></div>
                </a>
            </div>
        </section>

        <section id="view-trust" class="section-view">
            <div class="card">
                <h3>Global Feedback</h3>
                <div style="margin-top: 20px;">
                    <div class="review">
                        <div class="stars">★★★★★</div>
                        <p style="font-size: 0.8rem;"><b>David G. (USA):</b> "Nazim is a magician! My investment site is making profits daily. Highly professional."</p>
                    </div>
                    <div class="review">
                        <div class="stars">★★★★★</div>
                        <p style="font-size: 0.8rem;"><b>Sarah J. (UAE):</b> "Prime Solutions is the best for a reason. Quality and speed are unmatched."</p>
                    </div>
                </div>
            </div>

            <div class="card">
                <h3><i class="fas fa-shield-alt"></i> Company Policies</h3>
                <p style="font-size: 0.75rem; opacity: 0.6; line-height: 1.6; margin-top: 10px;">
                    <b>Privacy Policy:</b> We secure your digital assets with military-grade encryption.<br>
                    <b>Terms:</b> All project blueprints are protected under Prime Solutions NDA. We offer 24/7 dedicated support for lifetime.
                </p>
            </div>
        </section>

        <section id="view-contact" class="section-view">
            <div class="card">
                <h3>Connect with CEO</h3>
                <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 25px;">Direct access to Muhammad Nazim.</p>
                
                <input type="text" id="clientName" placeholder="Full Name" style="width: 100%; padding: 20px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none;">
                <textarea id="projectDetails" rows="3" placeholder="Vision for your project..." style="width: 100%; padding: 20px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 25px; outline: none;"></textarea>
                
                <a href="javascript:void(0)" class="btn-mega" onclick="contactCEO()">
                    <i class="fab fa-whatsapp"></i> MESSAGE VIA WHATSAPP
                </a>
                <a href="tel:03705519562" class="btn-mega" style="background: transparent; border: 1px solid var(--primary); color: var(--primary);">
                    <i class="fas fa-phone-alt"></i> CALL: 0370 5519562
                </a>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 40px; opacity: 0.3; font-size: 0.7rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL HUB © 2026<br>
            WORLD'S #1 RATED DIGITAL AGENCY
        </footer>

    </div>

    <nav class="nav-dock">
        <div class="dock-item active" onclick="navTo('home')"><i class="fas fa-home-alt"></i></div>
        <div class="dock-item" onclick="navTo('services')"><i class="fas fa-grid-2"></i></div>
        <div class="dock-item" onclick="navTo('trust')"><i class="fas fa-shield-halved"></i></div>
        <div class="dock-item" onclick="navTo('contact')"><i class="fas fa-envelope-open"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Sales Alert Engine
        const names = ["Ali", "Sofia", "Liam", "Chen", "Isabella", "Omar", "Noah"];
        const places = ["London", "Dubai", "New York", "Karachi", "Singapore", "Sydney"];
        const types = ["Investment Site", "E-Com Store", "App Design", "SEO Package"];

        function pushAlert() {
            const n = names[Math.floor(Math.random() * names.length)];
            const p = places[Math.floor(Math.random() * places.length)];
            const t = types[Math.floor(Math.random() * types.length)];
            
            document.getElementById('alert-text').innerText = `${n} from ${p} just hired Nazim for a ${t}!`;
            const box = document.getElementById('notify-box');
            box.style.display = 'block';
            
            setTimeout(() => { box.style.display = 'none'; }, 5000);
        }
        setInterval(pushAlert, 10000); // Har 10 second baad ek notification

        // Smooth Page Switcher
        function navTo(pageId) {
            document.querySelectorAll('.section-view').forEach(s => s.classList.remove('active'));
            document.getElementById('view-' + pageId).classList.add('active');
            
            document.querySelectorAll('.dock-item').forEach(i => i.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        // WhatsApp Command
        function contactCEO() {
            const name = document.getElementById('clientName').value;
            const details = document.getElementById('projectDetails').value;
            const text = `Hello CEO Nazim! My name is ${name}. I have a vision for a project: ${details}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
