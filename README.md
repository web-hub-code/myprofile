<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Prime Solutions | Global Digital Agency & IT Enterprise</title>
    
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

        /* Infinity Background */
        .agency-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow-sphere { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: move 15s infinite alternate; }
        @keyframes move { from { transform: translate(-10%, -10%); } to { transform: translate(40%, 40%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 15px 15px 160px; }

        /* Corporate Trust Alerts */
        #agency-alert { position: fixed; top: 15px; left: 50%; transform: translateX(-50%); z-index: 10000; width: 92%; max-width: 420px; display: none; }
        .alert-pill { background: rgba(0, 0, 0, 0.95); border: 1px solid var(--primary); padding: 12px 20px; border-radius: 50px; backdrop-filter: blur(25px); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 40px rgba(0,242,254,0.3); animation: slideDown 0.6s ease; }
        @keyframes slideDown { from { transform: translateY(-100px); } to { transform: translateY(0); } }

        /* Company Identity */
        .company-header { background: var(--glass); backdrop-filter: blur(35px); border: 1px solid var(--border); border-radius: 40px; padding: 40px 25px; text-align: center; margin-bottom: 25px; border-bottom: 5px solid var(--primary); }
        .pfp-ceo { width: 135px; height: 135px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; box-shadow: 0 0 40px rgba(0, 242, 254, 0.3); margin-bottom: 20px; }
        .brand-title { font-size: 2.5rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Multi-Tab Navigation */
        .agency-tabs { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 25px; }
        .tab-btn { background: var(--glass); border: 1px solid var(--border); padding: 12px 25px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.8rem; transition: 0.3s; }
        .tab-btn.active { background: var(--primary); color: #000; border-color: var(--primary); font-weight: 800; }

        /* Sections Logic */
        .section-view { display: none; }
        .section-view.active { display: block; animation: zoomReveal 0.5s ease; }
        @keyframes zoomReveal { from { opacity: 0; transform: scale(0.95); } to { opacity: 1; transform: scale(1); } }

        /* Corporate Cards */
        .corp-card { background: var(--glass); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 20px; position: relative; overflow: hidden; }
        .service-row { display: flex; align-items: center; gap: 18px; margin-bottom: 20px; padding: 15px; background: rgba(255,255,255,0.02); border-radius: 20px; transition: 0.3s; border: 1px solid transparent; }
        .service-row:hover { border-color: var(--primary); background: rgba(0,242,254,0.05); }
        .service-row i { font-size: 1.8rem; color: var(--primary); min-width: 45px; }

        /* Interactive Footer Dock */
        .dock-bar { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.98); backdrop-filter: blur(45px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 22px; z-index: 9999; box-shadow: 0 40px 80px rgba(0,0,0,1); }
        .dock-item { color: white; opacity: 0.35; font-size: 1.5rem; cursor: pointer; transition: 0.4s; }
        .dock-item.active { opacity: 1; color: var(--primary); transform: translateY(-10px); }

        /* Buttons & Inputs */
        .corp-input { width: 100%; background: rgba(255,255,255,0.04); border: 1px solid var(--border); border-radius: 20px; padding: 20px; color: white; margin-bottom: 15px; outline: none; }
        .btn-mega { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 22px; border-radius: 25px; width: 100%; border: none; font-weight: 800; cursor: pointer; font-size: 1rem; text-decoration: none; display: flex; justify-content: center; align-items: center; gap: 10px; }
    </style>
</head>
<body>

    <div class="agency-bg"><div class="glow-sphere"></div></div>

    <div id="agency-alert">
        <div class="alert-pill">
            <i class="fas fa-briefcase" style="color: var(--primary);"></i>
            <span id="alert-msg" style="font-size: 0.75rem; font-weight: 600;"></span>
        </div>
    </div>

    <div class="container">
        
        <header class="company-header" data-aos="fade-down">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-ceo" alt="CEO Muhammad Nazim">
            <div class="brand-title">PRIME SOLUTIONS</div>
            <p style="opacity: 0.6; font-size: 0.85rem; margin-top: 5px; letter-spacing: 1px;">Global IT Conglomerate & Agency</p>
            <div style="display: flex; justify-content: center; gap: 12px; margin-top: 25px;">
                <a href="https://wa.me/923332637235" class="tab-btn active" style="text-decoration:none;"><i class="fab fa-whatsapp"></i> Inquiry</a>
                <a href="tel:03705519562" class="tab-btn" style="text-decoration:none;"><i class="fas fa-phone"></i> Direct Office</a>
            </div>
        </header>

        <div class="agency-tabs">
            <div class="tab-btn active" onclick="navTo('home', this)">Agency Overview</div>
            <div class="tab-btn" onclick="navTo('divs', this)">Our Divisions</div>
            <div class="tab-btn" onclick="navTo('strategy', this)">Strategy</div>
            <div class="tab-btn" onclick="navTo('contact', this)">B2B Support</div>
        </div>

        <section id="view-home" class="section-view active">
            <div class="corp-card" data-aos="fade-up">
                <h3><i class="fas fa-building"></i> Company Profile</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.8; margin-top: 15px;">
                    Prime Solutions aik international digital agency hai jo dunya bhar ke businesses ko advanced IT solutions provide karti hai. Humari company ka vision digital transformation ko asaan aur profitable banana hai.
                </p>
                <div style="display: flex; justify-content: space-around; margin-top: 25px;">
                    <div style="text-align:center;"><h2>150+</h2><p style="font-size:0.6rem; opacity:0.5;">ENTERPRISES</p></div>
                    <div style="text-align:center;"><h2>50+</h2><p style="font-size:0.6rem; opacity:0.5;">COUNTRIES</p></div>
                </div>
            </div>
        </section>

        <section id="view-divs" class="section-view">
            <h3 style="margin-bottom: 20px; padding-left: 10px;">Our Specialized Units</h3>
            <div class="service-row">
                <i class="fas fa-university"></i>
                <div><h4>Edu-Tech Systems</h4><p>High-end software for Schools & Universities.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-heart-pulse"></i>
                <div><h4>Health-Care IT</h4><p>Complete Hospital & Clinic Management Portals.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-chart-area"></i>
                <div><h4>Fin-Tech Solutions</h4><p>Secure Investment & Banking dashboards.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-store"></i>
                <div><h4>Retail Ecosystems</h4><p>E-Commerce & Inventory Management for Brands.</p></div>
            </div>
        </section>

        <section id="view-strategy" class="section-view">
            <div class="corp-card">
                <h3>The Prime Method</h3>
                <div style="margin-top: 20px;">
                    <div style="margin-bottom: 15px;">
                        <h5 style="color:var(--primary);">01. Discovery Phase</h5>
                        <p style="font-size:0.75rem; opacity:0.5;">Client ki business requirements ko detail mein analyze karna.</p>
                    </div>
                    <div style="margin-bottom: 15px;">
                        <h5 style="color:var(--primary);">02. Core Architecture</h5>
                        <p style="font-size:0.75rem; opacity:0.5;">Scalable aur secure coding systems design karna.</p>
                    </div>
                    <div>
                        <h5 style="color:var(--primary);">03. Global Deployment</h5>
                        <p style="font-size:0.75rem; opacity:0.5;">Dunya bhar mein servers par live karna 100% security ke saath.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="view-contact" class="section-view">
            <div class="corp-card">
                <h3>Corporate Inquiry</h3>
                <p style="font-size: 0.75rem; opacity: 0.4; margin-bottom: 20px;">Send a formal request for your company project.</p>
                <input type="text" id="brand-name" class="corp-input" placeholder="Company/Brand Name">
                <textarea id="project-scope" class="corp-input" rows="3" placeholder="Project Scope..."></textarea>
                <button class="btn-mega" onclick="contactAgency()">
                    <i class="fab fa-whatsapp"></i> REQUEST PROPOSAL
                </button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 40px; opacity: 0.2; font-size: 0.6rem; letter-spacing: 2px;">
            PRIME SOLUTIONS GLOBAL CONGLOMERATE © 2026<br>
            FOUNDED & LED BY MUHAMMAD NAZIM
        </footer>
    </div>

    <nav class="dock-bar">
        <div class="dock-item active" onclick="navTo('home', this)"><i class="fas fa-building"></i></div>
        <div class="dock-item" onclick="navTo('divs', this)"><i class="fas fa-layer-group"></i></div>
        <div class="dock-item" onclick="navTo('strategy', this)"><i class="fas fa-chess-knight"></i></div>
        <div class="dock-item" onclick="navTo('contact', this)"><i class="fas fa-envelope-open-text"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Corporate Alert Logic
        const clients = ["Ahmad", "Sarah", "Dr. Wilson", "CEO Mike", "Li", "Fatima", "Sofia"];
        const places = ["Dubai", "New York", "London", "Singapore", "Berlin", "Sydney"];
        const units = ["Edu-Tech System", "Investment Portal", "Health Software", "Brand App"];

        function fireAlert() {
            const c = clients[Math.floor(Math.random() * clients.length)];
            const p = places[Math.floor(Math.random() * places.length)];
            const u = units[Math.floor(Math.random() * units.length)];
            
            document.getElementById('alert-msg').innerText = `${c} from ${p} just partnered with Prime Solutions for ${u}!`;
            const box = document.getElementById('agency-alert');
            box.style.display = 'block';
            setTimeout(() => { box.style.display = 'none'; }, 5000);
        }
        setInterval(fireAlert, 15000);

        // Multi-View Navigation
        function navTo(viewId, btn) {
            document.querySelectorAll('.section-view').forEach(v => v.classList.remove('active'));
            document.getElementById('view-' + viewId).classList.add('active');
            
            document.querySelectorAll('.tab-btn, .dock-item').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');
            window.scrollTo(0,0);
        }

        // B2B WhatsApp Strategy
        function contactAgency() {
            const brand = document.getElementById('brand-name').value;
            const scope = document.getElementById('project-scope').value;
            const text = `Greetings Prime Solutions HQ! We are ${brand}. Requesting proposal for: ${scope}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
