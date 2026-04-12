<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global CEO - Prime Solutions Hub</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* Infinity Background */
        .vision-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; 
            background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow-effect { position: absolute; width: 500px; height: 500px; background: var(--primary); filter: blur(200px); opacity: 0.1; border-radius: 50%; animation: float 15s infinite alternate; }
        @keyframes float { from { transform: translate(-50px, -50px); } to { transform: translate(100px, 100px); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 150px; }

        /* Sales Notification System */
        #sales-notify { position: fixed; top: 15px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 90%; max-width: 400px; display: none; }
        .notify-pill { background: rgba(0, 0, 0, 0.95); border: 1px solid var(--primary); padding: 12px 20px; border-radius: 50px; backdrop-filter: blur(20px); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 40px rgba(0,242,254,0.3); animation: slideIn 0.6s cubic-bezier(0.18, 0.89, 0.32, 1.28); }
        @keyframes slideIn { from { transform: translateY(-100px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

        /* Profile Hub */
        .profile-card { background: var(--glass); backdrop-filter: blur(35px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 30px; text-align: center; position: relative; overflow: hidden; }
        .pfp-main { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); padding: 6px; box-shadow: 0 0 50px rgba(0, 242, 254, 0.3); margin-bottom: 25px; transition: 0.5s; object-fit: cover; }
        .pfp-main:hover { transform: scale(1.05) rotate(5deg); }
        .online-status { position: absolute; top: 45px; right: 35%; width: 20px; height: 20px; background: #25d366; border-radius: 50%; border: 4px solid #010204; animation: pulse 1.5s infinite; }

        /* Social Hub Grid */
        .social-grid { display: grid; grid-template-columns: repeat(5, 1fr); gap: 10px; margin-top: 25px; }
        .social-icon { background: rgba(255,255,255,0.05); height: 50px; border-radius: 18px; display: flex; align-items: center; justify-content: center; font-size: 1.3rem; color: white; text-decoration: none; border: 1px solid var(--border); transition: 0.3s; }
        .social-icon:hover { background: var(--primary); color: #000; transform: translateY(-5px); border-color: var(--primary); box-shadow: 0 10px 20px rgba(0,242,254,0.2); }

        /* Multi-Page Views */
        .view-section { display: none; }
        .view-section.active { display: block; animation: zoomIn 0.5s ease; }
        @keyframes zoomIn { from { opacity: 0; transform: scale(0.95); } to { opacity: 1; transform: scale(1); } }

        /* Service Cards */
        .service-box { display: flex; align-items: center; gap: 20px; padding: 22px; background: rgba(255,255,255,0.02); border-radius: 30px; margin-bottom: 15px; text-decoration: none; color: white; border: 1px solid transparent; transition: 0.4s; }
        .service-box:hover { border-color: var(--primary); background: rgba(0,242,254,0.08); transform: scale(1.02); }
        .service-box i { font-size: 2rem; color: var(--primary); text-shadow: 0 0 15px var(--primary); }

        /* Navigation Dock */
        .bottom-dock { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.9); backdrop-filter: blur(35px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 22px; z-index: 9999; box-shadow: 0 40px 80px rgba(0,0,0,0.8); }
        .dock-btn { color: white; opacity: 0.35; font-size: 1.5rem; cursor: pointer; transition: 0.4s; position: relative; }
        .dock-btn.active { opacity: 1; color: var(--primary); transform: translateY(-8px); }
        .dock-btn.active::after { content: ''; position: absolute; bottom: -12px; left: 50%; transform: translateX(-50%); width: 20px; height: 4px; background: var(--primary); border-radius: 10px; box-shadow: 0 0 15px var(--primary); }

        /* Luxury Contact Buttons */
        .btn-luxury { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 22px; border-radius: 30px; width: 100%; border: none; font-weight: 800; font-size: 1.1rem; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 12px; margin-top: 25px; text-decoration: none; }
    </style>
</head>
<body>

    <div class="vision-bg"><div class="glow-effect"></div></div>

    <div id="sales-notify">
        <div class="notify-pill">
            <i class="fas fa-certificate" style="color: var(--primary);"></i>
            <span id="alert-text" style="font-size: 0.75rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="container">
        
        <section id="p-home" class="view-section active">
            <div class="profile-card" data-aos="zoom-in">
                <div class="online-status"></div>
                <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-main" alt="Nazim">
                <h1 style="font-size: 2.7rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
                <p style="opacity: 0.7; letter-spacing: 1px; font-weight: 300;">Architect of Digital Empires | Global CEO</p>
                
                <div class="social-grid">
                    <a href="https://facebook.com/prime.solutions" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                    <a href="https://instagram.com/nazim.prime" class="social-icon"><i class="fab fa-instagram"></i></a>
                    <a href="https://linkedin.com/in/nazim-ceo" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
                    <a href="https://github.com/web-hub-code" class="social-icon"><i class="fab fa-github"></i></a>
                    <a href="https://wa.me/923332637235" class="social-icon"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>

            <div class="profile-card" style="margin-top: 25px; padding: 30px;" data-aos="fade-up">
                <h3 style="margin-bottom: 20px;"><i class="fas fa-gem" style="color: var(--primary);"></i> Why Prime Solutions?</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.8;">
                    Prime Solutions dunya ki #1 agency hai jo aapke khwabon ko haqeeqat mein badalti hai. Humne 150+ projects worldwide mukammal kiye hain 100% client satisfaction ke saath.
                </p>
                <div style="display: flex; justify-content: space-between; margin-top: 25px; text-align: center;">
                    <div><h2 style="color: var(--primary);">150+</h2><p style="font-size: 0.5rem; opacity: 0.5;">DONE</p></div>
                    <div><h2 style="color: var(--primary);">50+</h2><p style="font-size: 0.5rem; opacity: 0.5;">CLIENTS</p></div>
                    <div><h2 style="color: var(--primary);">100%</h2><p style="font-size: 0.5rem; opacity: 0.5;">TRUST</p></div>
                </div>
            </div>
        </section>

        <section id="p-services" class="view-section">
            <h3 style="margin-bottom: 25px; padding-left: 10px;"><i class="fas fa-layer-group"></i> Elite Units</h3>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-box">
                <i class="fas fa-chart-line"></i>
                <div><h4>Investment Ecosystems</h4><p style="font-size: 0.7rem; opacity: 0.5;">Real-time ROI tracking & secure portals.</p></div>
            </a>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-box">
                <i class="fas fa-shopping-cart"></i>
                <div><h4>Global E-Commerce</h4><p style="font-size: 0.7rem; opacity: 0.5;">Scalable online stores with automated logic.</p></div>
            </a>
            <a href="javascript:void(0)" onclick="navTo('contact')" class="service-box">
                <i class="fas fa-shield-halved"></i>
                <div><h4>Software Security</h4><p style="font-size: 0.7rem; opacity: 0.5;">Advanced encryption for corporate data.</p></div>
            </a>
        </section>

        <section id="p-trust" class="view-section">
            <div class="profile-card" style="text-align: left; padding: 25px;">
                <h3 style="margin-bottom: 20px;">Client Testimonials</h3>
                <div style="background: rgba(0,0,0,0.2); padding: 15px; border-radius: 20px; border-left: 3px solid var(--primary); margin-bottom: 15px;">
                    <div style="color: #f1c40f; font-size: 0.8rem; margin-bottom: 5px;">★★★★★</div>
                    <p style="font-size: 0.8rem;">"Nazim is the best! My investment site works perfectly. High quality work." - <b>Adam (USA)</b></p>
                </div>
                <div style="background: rgba(0,0,0,0.2); padding: 15px; border-radius: 20px; border-left: 3px solid var(--primary);">
                    <div style="color: #f1c40f; font-size: 0.8rem; margin-bottom: 5px;">★★★★★</div>
                    <p style="font-size: 0.8rem;">"Highly professional agency. Their mobile UI is world-class." - <b>Sofia (Dubai)</b></p>
                </div>
            </div>

            <div class="profile-card" style="margin-top: 25px; text-align: left; padding: 25px;">
                <h3><i class="fas fa-user-shield"></i> Privacy & Company</h3>
                <p style="font-size: 0.75rem; opacity: 0.6; line-height: 1.7; margin-top: 15px;">
                    <b>Prime Solutions</b> is a registered digital agency. Hum 100% confidentiality ensure karte hain. Aapka data aur aapki investment details humari priority hain. Hum har client ke saath professional NDA sign karte hain.
                </p>
            </div>
        </section>

        <section id="p-contact" class="view-section">
            <div class="profile-card">
                <h3>Connect with CEO</h3>
                <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 25px;">Direct inquiries for premium projects.</p>
                <input type="text" id="c-name" placeholder="Full Name" style="width: 100%; padding: 20px; border-radius: 25px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none;">
                <textarea id="c-msg" rows="3" placeholder="Project details..." style="width: 100%; padding: 20px; border-radius: 25px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 20px; outline: none;"></textarea>
                
                <a href="javascript:void(0)" class="btn-luxury" onclick="sendInquiry()">
                    <i class="fab fa-whatsapp"></i> MESSAGE CEO NAZIM
                </a>
                <a href="tel:03705519562" class="btn-luxury" style="background: transparent; border: 1px solid var(--primary); color: var(--primary);">
                    <i class="fas fa-phone"></i> CALL: 0370 5519562
                </a>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 50px; opacity: 0.3; font-size: 0.65rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL CONGLOMERATE © 2026<br>
            Coded with Excellence by Muhammad Nazim
        </footer>
    </div>

    <nav class="bottom-dock">
        <div class="dock-btn active" onclick="navTo('home')"><i class="fas fa-home-alt"></i></div>
        <div class="dock-btn" onclick="navTo('services')"><i class="fas fa-th-large"></i></div>
        <div class="dock-btn" onclick="navTo('trust')"><i class="fas fa-shield-check"></i></div>
        <div class="dock-btn" onclick="navTo('contact')"><i class="fas fa-envelope-open-text"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Fake Order Notification System
        const persons = ["Ali", "James", "Fatima", "Chen", "Isabella", "Omar", "Noah", "Sarah"];
        const cities = ["London", "Dubai", "New York", "Karachi", "Singapore", "Sydney", "Berlin"];
        const projTypes = ["Investment Portal", "E-Com Store", "App Design", "SEO Strategy"];

        function triggerAlert() {
            const p = persons[Math.floor(Math.random() * persons.length)];
            const c = cities[Math.floor(Math.random() * cities.length)];
            const t = projTypes[Math.floor(Math.random() * projTypes.length)];
            
            document.getElementById('alert-text').innerText = `${p} from ${c} just hired Nazim for a ${t}!`;
            const box = document.getElementById('sales-notify');
            box.style.display = 'block';
            
            setTimeout(() => { box.style.display = 'none'; }, 5000);
        }
        setInterval(triggerAlert, 12000);

        // Smooth Page Switcher
        function navTo(id) {
            document.querySelectorAll('.view-section').forEach(v => v.classList.remove('active'));
            document.getElementById('p-' + id).classList.add('active');
            
            document.querySelectorAll('.dock-btn').forEach(b => b.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        // WhatsApp Command
        function sendInquiry() {
            const n = document.getElementById('c-name').value;
            const m = document.getElementById('c-msg').value;
            const text = `Greetings CEO Nazim! I am ${n}. Project vision: ${m}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
