<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global CEO - Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* Animated Particles Mockup */
        .bg-gradient { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 20% 30%, #002d35 0%, #010204 100%); }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Global Header Hub */
        .header-hub { display: flex; justify-content: space-between; align-items: center; padding: 12px 20px; background: var(--glass); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); margin-bottom: 25px; }
        .live-badge { font-size: 0.6rem; background: rgba(37, 211, 102, 0.15); color: #25d366; padding: 4px 10px; border-radius: 50px; font-weight: 800; border: 1px solid rgba(37, 211, 102, 0.3); }

        /* Multi-Page Sections */
        .section-view { display: none; animation: pageReveal 0.6s cubic-bezier(0.23, 1, 0.32, 1) forwards; }
        .section-view.active { display: block; }
        @keyframes pageReveal { from { opacity: 0; transform: scale(0.98) translateY(20px); } to { opacity: 1; transform: scale(1) translateY(0); } }

        /* Premium Profile Card */
        .hero-card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 45px; padding: 40px 25px; text-align: center; position: relative; overflow: hidden; }
        .hero-card::before { content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%; background: conic-gradient(from 180deg at 50% 50%, var(--primary) 0deg, transparent 360deg); opacity: 0.05; animation: rotate 10s linear infinite; }
        @keyframes rotate { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }

        .profile-pfp { width: 135px; height: 135px; border-radius: 50%; border: 4px solid var(--primary); padding: 5px; box-shadow: 0 0 40px rgba(0, 242, 254, 0.2); margin-bottom: 20px; z-index: 2; position: relative; }
        .name-title { font-size: 2.6rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Stats Branding */
        .metrics-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 15px; margin-top: 30px; }
        .metric-item h4 { font-size: 1.6rem; color: var(--primary); font-weight: 800; }
        .metric-item p { font-size: 0.55rem; opacity: 0.5; text-transform: uppercase; letter-spacing: 1px; }

        /* World Class Services */
        .glass-card { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-top: 20px; transition: 0.4s; }
        .service-row { display: flex; align-items: center; gap: 18px; margin-bottom: 20px; padding: 18px; background: rgba(255,255,255,0.02); border-radius: 25px; border: 1px solid transparent; }
        .service-row:hover { border-color: var(--primary); background: rgba(0, 242, 254, 0.05); }
        .service-row i { font-size: 1.8rem; color: var(--primary); }

        /* Ultimate Navigation Dock */
        .dock-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 480px; background: rgba(10, 10, 10, 0.9); backdrop-filter: blur(30px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 5000; box-shadow: 0 30px 60px rgba(0,0,0,0.6); }
        .dock-btn { color: white; opacity: 0.35; font-size: 1.4rem; cursor: pointer; transition: 0.4s; position: relative; }
        .dock-btn.active { opacity: 1; color: var(--primary); transform: translateY(-5px) scale(1.1); }
        .dock-btn.active::after { content: ''; position: absolute; bottom: -10px; left: 50%; transform: translateX(-50%); width: 6px; height: 6px; background: var(--primary); border-radius: 50%; box-shadow: 0 0 10px var(--primary); }

        /* CTA Buttons */
        .cta-prime { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; border-radius: 25px; width: 100%; border: none; font-weight: 800; font-size: 1.1rem; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 12px; margin-top: 25px; box-shadow: 0 15px 35px rgba(0, 242, 254, 0.25); }
    </style>
</head>
<body>

    <div class="bg-gradient"></div>

    <div class="container">
        <header class="header-hub" data-aos="fade-down">
            <div class="live-badge"><span style="animation: pulse 1s infinite;">●</span> CEO ONLINE</div>
            <div onclick="switchLanguage()" id="langSwitcher" style="background: var(--primary); color: #000; padding: 6px 15px; border-radius: 50px; font-size: 0.65rem; font-weight: 800; cursor: pointer;">URDU</div>
        </header>

        <section id="view-home" class="section-view active">
            <div class="hero-card" data-aos="zoom-out">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="profile-pfp">
                <h1 class="name-title" id="txt-name">Muhammad Nazim</h1>
                <p id="txt-tag" style="opacity: 0.7; font-weight: 300; letter-spacing: 1px;">Architect of Global Digital Ecosystems | CEO</p>
                
                <div class="metrics-grid">
                    <div class="metric-item"><h4>150+</h4><p id="m1">Global Projects</p></div>
                    <div class="metric-item"><h4>50+</h4><p id="m2">Worldwide Clients</p></div>
                    <div class="metric-item"><h4>5.0</h4><p id="m3">Elite Rating</p></div>
                </div>
            </div>

            <div class="glass-card" data-aos="fade-up">
                <h3 id="txt-miss"><i class="fas fa-crown"></i> The Vision</h3>
                <p id="txt-desc" style="font-size: 0.85rem; opacity: 0.6; margin-top: 15px; line-height: 1.7;">Duniya ki top 1 agency banne ka safar humari quality aur client trust se shuru hota hai. Hum sirif code nahi karte, hum digital empires khare karte hain.</p>
                <button class="cta-prime" onclick="navTo('contact')">EXPLORE COLLABORATION</button>
            </div>
        </section>

        <section id="view-services" class="section-view">
            <h3 style="margin-bottom: 25px; padding-left: 10px;" id="s-title"><i class="fas fa-gem"></i> Elite Solutions</h3>
            <div class="service-row">
                <i class="fas fa-code-merge"></i>
                <div><h4 id="v1">Neural Web Architectures</h4><p style="font-size: 0.75rem; opacity: 0.6;">Ultra-fast, high-security applications.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-chart-line-up"></i>
                <div><h4 id="v2">FinTech Dominance</h4><p style="font-size: 0.75rem; opacity: 0.6;">Investment portals with global scale API.</p></div>
            </div>
            <div class="service-row">
                <i class="fas fa-globe-americas"></i>
                <div><h4 id="v3">Global Market SEO</h4><p style="font-size: 0.75rem; opacity: 0.6;">Ranking businesses to #1 internationally.</p></div>
            </div>
        </section>

        <section id="view-contact" class="section-view">
            <div class="glass-card">
                <h3 id="c-title">Connect with Global CEO</h3>
                <p style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 25px;" id="c-sub">Professional inquiries for world-class projects.</p>
                
                <input type="text" id="inpName" placeholder="Business Name / Full Name" style="width: 100%; padding: 20px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none;">
                <textarea id="inpDesc" rows="3" placeholder="Define your vision..." style="width: 100%; padding: 20px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 20px; outline: none;"></textarea>
                
                <button class="cta-prime" onclick="initiateContact()">
                    <i class="fab fa-whatsapp"></i> <span id="btn-txt">PROCEED TO STRATEGY CALL</span>
                </button>
            </div>
        </section>

        <footer style="text-align: center; margin-top: 50px; opacity: 0.25; font-size: 0.7rem; letter-spacing: 1.5px;">
            PRIME SOLUTIONS: THE WORLD'S #1 AGENCY HUB © 2026<br>
            Coded with Precision by Muhammad Nazim
        </footer>
    </div>

    <nav class="dock-bar">
        <div class="dock-btn active" onclick="navTo('home')"><i class="fas fa-house-user"></i></div>
        <div class="dock-btn" onclick="navTo('services')"><i class="fas fa-layer-group"></i></div>
        <div class="dock-btn" onclick="navTo('contact')"><i class="fas fa-paper-plane"></i></div>
        <a href="tel:03705519562" class="dock-btn" style="text-decoration:none;"><i class="fas fa-phone-volume"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        let currentLang = 'en';

        function navTo(pageId) {
            document.querySelectorAll('.section-view').forEach(s => s.classList.remove('active'));
            document.getElementById('view-' + pageId).classList.add('active');
            document.querySelectorAll('.dock-btn').forEach(b => b.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        function switchLanguage() {
            const btn = document.getElementById('langSwitcher');
            if(currentLang === 'en') {
                translateUI('ur');
                btn.innerText = 'ENGLISH';
                currentLang = 'ur';
            } else {
                translateUI('en');
                btn.innerText = 'URDU';
                currentLang = 'en';
            }
        }

        function translateUI(l) {
            const dictionary = {
                en: { name:"Muhammad Nazim", tag:"Architect of Global Digital Ecosystems | CEO", m1:"Global Projects", m2:"Worldwide Clients", m3:"Elite Rating", miss:"The Vision", desc:"Duniya ki top 1 agency banne ka safar humari quality aur client trust se shuru hota hai. Hum sirif code nahi karte, hum digital empires khare karte hain.", stit:"Elite Solutions", v1:"Neural Web Architectures", v2:"FinTech Dominance", v3:"Global Market SEO", ct:"Connect with Global CEO", cs:"Professional inquiries for world-class projects.", bt:"PROCEED TO STRATEGY CALL" },
                ur: { name:"محمد ناظم", tag:"عالمی ڈیجیٹل ایکو سسٹم کے معمار | سی ای او", m1:"عالمی پراجیکٹس", m2:"دنیابھر کے کلائنٹس", m3:"اعلیٰ ترین درجہ بندی", miss:"ہمارا وژن", desc:"دنیا کی ٹاپ 1 ایجنسی بننے کا سفر ہماری معیار اور کلائنٹ کے اعتماد سے شروع ہوتا ہے۔ ہم صرف کوڈ نہیں کرتے، ہم ڈیجیٹل سلطنتیں کھڑی کرتے ہیں۔", stit:"اعلیٰ ترین سروسز", v1:"جدید ویب فن تعمیر", v2:"فنانشل ٹیکنالوجی پورٹلز", v3:"عالمی مارکیٹ ایس ای او", ct:"عالمی سی ای او سے رابطہ کریں", cs:"عالمی معیار کے پراجیکٹس کے لیے پروفیشنل رابطہ۔", bt:"سٹریٹیجی کال شروع کریں" }
            };
            const cur = dictionary[l];
            document.getElementById('txt-name').innerText = cur.name;
            document.getElementById('txt-tag').innerText = cur.tag;
            document.getElementById('m1').innerText = cur.m1;
            document.getElementById('m2').innerText = cur.m2;
            document.getElementById('m3').innerText = cur.m3;
            document.getElementById('txt-miss').innerHTML = `<i class="fas fa-crown"></i> ${cur.miss}`;
            document.getElementById('txt-desc').innerText = cur.desc;
            document.getElementById('s-title').innerHTML = `<i class="fas fa-gem"></i> ${cur.stit}`;
            document.getElementById('v1').innerText = cur.v1;
            document.getElementById('v2').innerText = cur.v2;
            document.getElementById('v3').innerText = cur.v3;
            document.getElementById('c-title').innerText = cur.ct;
            document.getElementById('c-sub').innerText = cur.cs;
            document.getElementById('btn-txt').innerText = cur.bt;
        }

        function initiateContact() {
            const name = document.getElementById('inpName').value;
            const desc = document.getElementById('inpDesc').value;
            const text = `Hello CEO Nazim! I am representing ${name}. Our vision for collaboration: ${desc}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
