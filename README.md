<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Prime Solutions | Global IT Enterprise & Agency</title>
    
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

        /* CEO Aura Background */
        .agency-aura { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #001f24 0%, #010204 100%); }
        .glow { position: absolute; width: 400px; height: 400px; background: var(--primary); filter: blur(180px); opacity: 0.1; border-radius: 50%; animation: move 20s infinite alternate; }
        @keyframes move { from { transform: translate(-10%, -10%); } to { transform: translate(50%, 50%); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 10px 15px 160px; }

        /* Mega Header */
        .agency-header { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 45px; padding: 45px 25px; text-align: center; margin-bottom: 25px; border-bottom: 5px solid var(--primary); }
        .pfp-ceo { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); padding: 6px; box-shadow: 0 0 50px rgba(0, 242, 254, 0.3); margin-bottom: 20px; }
        .brand-name { font-size: 2.8rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; }

        /* Tabs System */
        .tabs-container { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 15px; scrollbar-width: none; margin-bottom: 25px; }
        .tab-trigger { background: var(--glass); border: 1px solid var(--border); padding: 14px 28px; border-radius: 25px; color: white; cursor: pointer; white-space: nowrap; font-size: 0.85rem; transition: 0.3s; font-weight: 600; }
        .tab-trigger.active { background: var(--primary); color: #000; border-color: var(--primary); box-shadow: 0 0 20px rgba(0,242,254,0.3); }

        /* View Panes */
        .view-pane { display: none; }
        .view-pane.active { display: block; animation: fadeInUp 0.5s ease; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }

        /* Cards Style */
        .feature-card { background: var(--glass); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 20px; transition: 0.3s; overflow: hidden; }
        .feature-card:hover { transform: scale(1.02); background: rgba(0,242,254,0.04); }
        .card-img { width: 100%; height: 200px; object-fit: cover; margin-bottom: 0; border-bottom: 1px solid var(--border); }
        
        .calc-box { background: rgba(0,242,254,0.05); border: 1px dashed var(--primary); border-radius: 30px; padding: 25px; text-align: center; margin-top: 20px; }
        .btn-action { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 22px; border-radius: 25px; width: 100%; border: none; font-weight: 800; cursor: pointer; font-size: 1rem; text-decoration: none; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 20px; }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 92%; max-width: 480px; background: rgba(5, 5, 5, 0.98); backdrop-filter: blur(45px); border-radius: 60px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 22px; z-index: 9999; }
        .nav-icon { color: white; opacity: 0.35; font-size: 1.5rem; cursor: pointer; transition: 0.4s; }
        .nav-icon.active { opacity: 1; color: var(--primary); transform: translateY(-10px); }
    </style>
</head>
<body>

    <div class="agency-aura"><div class="glow"></div></div>

    <div class="container">
        <header class="agency-header" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" class="pfp-ceo" alt="Muhammad Nazim CEO">
            <div class="brand-name">PRIME SOLUTIONS</div>
            <p style="opacity: 0.6; font-size: 0.85rem; letter-spacing: 2px; font-weight: 300;">GLOBAL ENTERPRISE AGENCY</p>
        </header>

        <div class="tabs-container">
            <div class="tab-trigger active" onclick="navTo('home', this)">Agency</div>
            <div class="tab-trigger" onclick="navTo('works', this)">Portfolio</div>
            <div class="tab-trigger" onclick="navTo('solutions', this)">Solutions</div>
            <div class="tab-trigger" onclick="navTo('calculator', this)">Price Calc</div>
        </div>

        <section id="pane-home" class="view-pane active">
            <div class="feature-card">
                <i class="fas fa-microchip" style="font-size: 2rem; color: var(--primary); margin-bottom:15px;"></i>
                <h3>CEO Vision</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; line-height: 1.8; margin-top: 10px;">
                    Under the leadership of Muhammad Nazim, Prime Solutions is redefining digital excellence through AI and high-end automation.
                </p>
            </div>
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                <div class="feature-card" style="text-align:center;"><h2>200+</h2><p style="font-size:0.6rem;">PROJECTS</p></div>
                <div class="feature-card" style="text-align:center;"><h2>100%</h2><p style="font-size:0.6rem;">SUCCESS</p></div>
            </div>
        </section>

        <section id="pane-works" class="view-pane">
            <div class="feature-card" style="padding:0;">
                <img src="Screenshot_2026-04-15-09-59-25-00.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:var(--primary)">Core Infrastructure</h4>
                    <p style="font-size:0.75rem; opacity:0.6;">Advanced backend and UI solutions for global scale.</p>
                </div>
            </div>
            <div class="feature-card" style="padding:0;">
                <img src="Screenshot_2026-04-15-10-01-13-43.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:var(--accent)">Prime Academy</h4>
                    <p style="font-size:0.75rem; opacity:0.6;">Futuristic E-Learning dashboard and management system.</p>
                </div>
            </div>
            <div class="feature-card" style="padding:0;">
                <img src="Screenshot_2026-04-15-10-04-08-81.png" class="card-img">
                <div style="padding:20px;">
                    <h4 style="color:#ffd700">MintCrestGold</h4>
                    <p style="font-size:0.75rem; opacity:0.6;">Luxury Fin-Tech dashboard for ROI and gold investments.</p>
                </div>
            </div>
        </section>

        <section id="pane-solutions" class="view-pane">
            <div class="feature-card"><h3>Digital Transformation</h3><p style="font-size:0.8rem; opacity:0.5;">Custom software for healthcare and finance.</p></div>
            <div class="feature-card"><h3>AI Integration</h3><p style="font-size:0.8rem; opacity:0.5;">Smart bots and automated workflows.</p></div>
        </section>

        <section id="pane-calculator" class="view-pane">
            <div class="feature-card">
                <h3>Project Estimator</h3>
                <div class="calc-box"><p id="quote-display" style="font-size: 1.5rem; font-weight: 800; color: var(--primary);">$0.00</p></div>
                <button class="btn-action" onclick="window.location.href='https://wa.me/923332637235'">Consult CEO</button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 50px; opacity: 0.2; font-size: 0.6rem;">
            PRIME SOLUTIONS GLOBAL © 2026 | CEO: MUHAMMAD NAZIM
        </footer>
    </div>

    <nav class="bottom-nav">
        <div class="nav-icon active" onclick="navTo('home', this)"><i class="fas fa-building"></i></div>
        <div class="nav-icon" onclick="navTo('works', this)"><i class="fas fa-layer-group"></i></div>
        <div class="nav-icon" onclick="navTo('solutions', this)"><i class="fas fa-rocket"></i></div>
        <div class="nav-icon" onclick="navTo('calculator', this)"><i class="fas fa-calculator"></i></div>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        function navTo(paneId, btn) {
            document.querySelectorAll('.view-pane').forEach(p => p.classList.remove('active'));
            document.getElementById('pane-' + paneId).classList.add('active');
            document.querySelectorAll('.tab-trigger, .nav-icon').forEach(b => b.classList.remove('active'));
            btn.classList.add('active');
            window.scrollTo(0,0);
            if(paneId === 'calculator') runCalculator();
        }
        function runCalculator() {
            let price = 500;
            const interval = setInterval(() => {
                price += Math.floor(Math.random() * 50);
                document.getElementById('quote-display').innerText = '$' + price + '.00';
                if(price > 1200) clearInterval(interval);
            }, 50);
        }
    </script>
</body>
</html>
