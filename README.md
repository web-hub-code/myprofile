<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global CEO - Prime Solutions Multi-System</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* Multi-Layered Background */
        .vision-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 20% 30%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 300px; height: 300px; background: var(--primary); filter: blur(150px); opacity: 0.15; border-radius: 50%; animation: move 20s infinite alternate; }
        @keyframes move { from { transform: translate(0, 0); } to { transform: translate(100%, 100%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 15px 15px 150px; }

        /* Floating Trust Notifications */
        #sales-alert { position: fixed; top: 20px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 90%; max-width: 420px; display: none; }
        .alert-pill { background: rgba(0, 0, 0, 0.9); border: 1px solid var(--primary); padding: 12px 20px; border-radius: 50px; backdrop-filter: blur(20px); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 30px rgba(0,242,254,0.3); animation: slideDown 0.6s cubic-bezier(0.18, 0.89, 0.32, 1.28); }
        @keyframes slideDown { from { transform: translateY(-100px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

        /* Main Identity Card */
        .identity-card { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 40px; padding: 35px 25px; text-align: center; margin-bottom: 25px; border-bottom: 4px solid var(--primary); }
        .pfp-main { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; box-shadow: 0 0 40px rgba(0, 242, 254, 0.3); margin-bottom: 15px; transition: 0.5s; }
        .pfp-main:hover { transform: scale(1.05); }

        /* Tab Navigation (Modern Interface) */
        .tab-bar { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 20px; }
        .tab-item { background: var(--glass); border: 1px solid var(--border); padding: 12px 22px; border-radius: 20px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.8rem; transition: 0.3s; }
        .tab-item.active { background: var(--primary); color: #000; border-color: var(--primary); font-weight: 800; }

        /* View Content Engine */
        .view-content { display: none; }
        .view-content.active { display: block; animation: fadeIn 0.5s ease-out; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }

        /* Grid Detail Cards */
        .detail-card { background: var(--glass); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 20px; position: relative; overflow: hidden; }
        .service-row { display: flex; align-items: center; gap: 18px; margin-bottom: 20px; padding: 15px; background: rgba(255,255,255,0.02); border-radius: 20px; border-left: 3px solid var(--primary); }
        .service-row i { font-size: 1.8rem; color: var(--primary); min-width: 40px; text-align: center; }
        .service-row h4 { font-size: 1rem; margin-bottom: 3px; }
        .service-row p { font-size: 0.75rem; opacity: 0.5; }

        /* Global Footer Dock */
        .nav-dock { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.95); backdrop-filter: blur(40px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 20px; z-index: 9999; box-shadow: 0 40px 80px rgba(0,0,0,0.8); }
        .dock-link { color: white; opacity: 0.35; font-size: 1.4rem; cursor: pointer; transition: 0.4s; }
        .dock-link.active { opacity: 1; color: var(--primary); transform: translateY(-8px); }

        /* Custom Input Fields */
        .custom-input { width: 100%; background: rgba(0,0,0,0.3); border: 1px solid var(--border); border-radius: 20px; padding: 18px; color: white; margin-bottom: 12px; outline: none; transition: 0.3s; }
        .custom-input:focus { border-color: var(--primary); box-shadow: 0 0 15px rgba(0,242,254,0.1); }
        .btn-glow { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; border-radius: 20px; width: 100%; border: none; font-weight: 800; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 10px; font-size: 1rem; text-decoration: none; }
    </style>
</head>
<body>

    <div class="vision-bg"><div class="glow"></div></div>

    <div id="sales-alert">
        <div class="alert-pill">
            <i class="fas fa-shopping-bag"></i>
            <span id="alert-msg" style="font-size: 0.75rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="container">
        
        <div class="identity-card" data-aos="fade-down">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-main" alt="CEO Nazim">
            <h1 style="font-size: 2.2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
            <p style="opacity: 0.7; font-size: 0.8rem; letter-spacing: 1px;">Global CEO - Prime Solutions Agency</p>
            
            <div style="display: flex; justify-content: center; gap: 12px; margin-top: 20px;">
                <a href="https://wa.me/923332637235" class="tab-item active" style="text-decoration:none;"><i class="fab fa-whatsapp"></i> Chat Now</a>
                <a href="tel:03705519562" class="tab-item" style="text-decoration:none;"><i class="fas fa-phone"></i> 03705519562</a>
            </div>
        </div>

        <div class="tab-bar">
            <div class="tab-item active" onclick="switchView('overview', this)">Overview</div>
            <div class="tab-item" onclick="switchView('industry', this)">Industries</div>
            <div class="tab-item" onclick="switchView('features', this)">Core Features</div>
            <div class="tab-item" onclick="switchView('trust', this)">Company Trust</div>
        </div>

        <section id="view-overview" class="view-content active">
            <div class="detail-card">
                <h3><i class="fas fa-globe"></i> About Our Empire</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.7; margin-top: 15px;">
                    Prime Solutions aik international digital agency hai jo sirf website nahi, balkay poora digital ecosystem banati hai. Hum har business ki zarurat ke mutabiq custom software provide karte hain.
                </p>
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-top: 20px;">
                    <div class="service-row" style="margin:0; padding:10px;"><div><h2>150+</h2><p>Projects</p></div></div>
                    <div class="service-row" style="margin:0; padding:10px;"><div><h2>50+</h2><p>Clients</p></div></div>
                </div>
            </div>
        </section>

        <section id="view-industry" class="view-content">
            <h3 style="margin-bottom: 20px; padding-left: 10px;">What We Build</h3>
            <div class="service-row">
                <i class="fas fa-school"></i>
                <div><h4>Educational Systems</h4><p>School & College management softwares.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-hospital-user"></i>
                <div><h4>Health Care Portals</h4><p>Hospital management & Patient records.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-dumbbell"></i>
                <div><h4>GYM & Fitness Apps</h4><p>Membership tracking & workout portals.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-coins"></i>
                <div><h4>Investment Platforms</h4><p>Real-time profit & ROI dashboards.</p></div>
            </div>
        </section>

        <section id="view-features" class="view-content">
            <div class="detail-card">
                <h3><i class="fas fa-microchip"></i> Modern Technologies</h3>
                <div style="margin-top: 15px;">
                    <p style="font-size: 0.8rem; margin-bottom: 10px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> High Speed Performance</p>
                    <p style="font-size: 0.8rem; margin-bottom: 10px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> Mobile First Responsive Design</p>
                    <p style="font-size: 0.8rem; margin-bottom: 10px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> SEO Optimized Code</p>
                    <p style="font-size: 0.8rem; margin-bottom: 10px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> Advanced Data Security & Encryption</p>
                </div>
            </div>
        </section>

        <section id="view-trust" class="view-content">
            <div class="detail-card">
                <h3>Privacy & Guarantee</h3>
                <p style="font-size: 0.75rem; opacity: 0.5; margin-top: 10px; line-height: 1.6;">
                    Hum professional NDA sign karte hain taake aapka idea aur data mahfooz rahe. Hum 100% money-back guarantee aur lifetime tech support provide karte hain.
                </p>
            </div>
            
            <div class="detail-card">
                <h3>Book a Strategy Call</h3>
                <input type="text" id="u-name" class="custom-input" placeholder="Your Name" style="margin-top:15px;">
                <textarea id="u-msg" class="custom-input" rows="3" placeholder="Project details..."></textarea>
                <button class="btn-glow" onclick="startChat()">
                    <i class="fab fa-whatsapp"></i> START CONSULTATION
                </button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 40px; opacity: 0.2; font-size: 0.6rem; letter-spacing: 2px;">
            PRIME SOLUTIONS CONGLOMERATE © 2026<br>
            WORLD'S #1 RATED DIGITAL AGENCY
        </footer>
    </div>

    <nav class="nav-dock">
        <div class="dock-link active" onclick="switchView('overview', this)"><i class="fas fa-home"></i></div>
        <div class="dock-link" onclick="switchView('industry', this)"><i class="fas fa-grid-2"></i></div>
        <div class="dock-link" onclick="switchView('features', this)"><i class="fas fa-bolt"></i></div>
        <div class="dock-link" onclick="switchView('trust', this)"><i class="fas fa-user-shield"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Fake Alerts Engine
        const names = ["Ali", "Sarah", "John", "Fatima", "Chen", "Sofia", "Omar"];
        const cities = ["London", "Dubai", "New York", "Karachi", "Singapore"];
        const projs = ["School System", "Investment Site", "SEO Boost", "Gym Portal"];

        function runAlerts() {
            const n = names[Math.floor(Math.random() * names.length)];
            const c = cities[Math.floor(Math.random() * cities.length)];
            const p = projs[Math.floor(Math.random() * projs.length)];
            
            document.getElementById('alert-msg').innerText = `${n} from ${c} just booked a ${p}!`;
            const box = document.getElementById('sales-alert');
            box.style.display = 'block';
            setTimeout(() => { box.style.display = 'none'; }, 5000);
        }
        setInterval(runAlerts, 12000);

        // View Switcher
        function switchView(viewId, btn) {
            document.querySelectorAll('.view-content').forEach(v => v.classList.remove('active'));
            document.getElementById('view-' + viewId).classList.add('active');
            
            document.querySelectorAll('.tab-item, .dock-link').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');
            window.scrollTo(0,0);
        }

        // WhatsApp Link
        function startChat() {
            const name = document.getElementById('u-name').value;
            const msg = document.getElementById('u-msg').value;
            const text = `Greetings CEO Nazim! I am ${name}. Inquiry: ${msg}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
