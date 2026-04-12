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
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background: var(--bg); color: white; overflow-x: hidden; }

        /* Animated Background Particles Mockup */
        .bg-glow { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: radial-gradient(circle at 50% 50%, #1a1a2e 0%, #010204 100%); }
        .orb { position: absolute; width: 300px; height: 300px; background: var(--primary); filter: blur(150px); opacity: 0.15; border-radius: 50%; animation: float 15s infinite; }

        @keyframes float { 0%, 100% { transform: translate(0, 0); } 50% { transform: translate(100px, 50px); } }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        /* World Class Header */
        .top-status { display: flex; justify-content: space-between; align-items: center; padding: 12px 20px; background: var(--glass); border-radius: 50px; border: 1px solid var(--border); margin-bottom: 25px; backdrop-filter: blur(10px); }
        .live-dot { height: 8px; width: 8px; background: #25d366; border-radius: 50%; display: inline-block; box-shadow: 0 0 10px #25d366; animation: pulse 1.5s infinite; }

        /* Mega Hero Card */
        .hero-card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 40px; padding: 35px; text-align: center; position: relative; overflow: hidden; }
        .pfp { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); padding: 5px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.3); margin-bottom: 15px; }
        .name-gradient { font-size: 2.5rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Stats Grid */
        .stats { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 15px; margin-top: 30px; }
        .stat-box h3 { font-size: 1.5rem; color: var(--primary); }
        .stat-box p { font-size: 0.6rem; opacity: 0.5; text-transform: uppercase; }

        /* Service Infinity Grid */
        .card { background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-top: 25px; transition: 0.3s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }
        .service-link { display: flex; align-items: center; gap: 15px; margin-bottom: 15px; padding: 15px; background: rgba(255,255,255,0.02); border-radius: 20px; }

        /* Advanced Footer Nav */
        .nav-dock { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 450px; background: rgba(10, 10, 10, 0.85); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 25px 50px rgba(0,0,0,0.5); }
        .nav-item { font-size: 1.4rem; color: white; opacity: 0.4; cursor: pointer; transition: 0.3s; }
        .nav-item.active { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* UI Buttons */
        .prime-btn { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; border-radius: 25px; width: 100%; border: none; font-weight: 800; font-size: 1rem; cursor: pointer; display: flex; justify-content: center; align-items: center; gap: 10px; margin-top: 20px; }
    </style>
</head>
<body>

    <div class="bg-glow">
        <div class="orb" style="top: 10%; left: -10%;"></div>
        <div class="orb" style="bottom: 10%; right: -10%; background: var(--accent);"></div>
    </div>

    <div class="container">
        
        <div class="top-status">
            <span style="font-size: 0.7rem; font-weight: 800; letter-spacing: 1px;"> <span class="live-dot"></span> TOP 1 GLOBAL AGENCY</span>
            <button onclick="toggleLang()" id="langBtn" style="background: var(--primary); color:#000; border:none; padding:5px 12px; border-radius:50px; font-size:0.6rem; font-weight:800; cursor:pointer;">URDU</button>
        </div>

        <section id="home" class="hero-card" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" class="pfp">
            <h1 class="name-gradient" id="m-name">Muhammad Nazim</h1>
            <p id="m-tag" style="opacity: 0.7; font-size: 0.9rem;">Architect of Digital Ecosystems | CEO</p>
            
            <div class="stats">
                <div class="stat-box"><h3>150+</h3><p id="s1">Projects</p></div>
                <div class="stat-box"><h3>50+</h3><p id="s2">Global Clients</p></div>
                <div class="stat-box"><h3>5.0</h3><p id="s3">Rating ★</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 id="serv-h" style="margin-bottom: 20px;"><i class="fas fa-gem" style="color: var(--primary);"></i> Premium Solutions</h3>
            <div class="service-link">
                <i class="fas fa-code-branch" style="color: var(--primary);"></i>
                <div><h4 id="v1">Next-Gen Web Apps</h4><p style="font-size: 0.7rem; opacity: 0.6;">High-performance React & AI apps.</p></div>
            </div>
            <div class="service-link">
                <i class="fas fa-vault" style="color: var(--primary);"></i>
                <div><h4 id="v2">FinTech Portals</h4><p style="font-size: 0.7rem; opacity: 0.6;">Secure investment & crypto systems.</p></div>
            </div>
            <div class="service-link">
                <i class="fas fa-bullseye" style="color: var(--primary);"></i>
                <div><h4 id="v3">Global Brand SEO</h4><p style="font-size: 0.7rem; opacity: 0.6;">Dominating Google worldwide.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 id="cont-h">Launch a Project</h3>
            <p id="cont-p" style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 20px;">Direct bridge to Prime Solutions CEO</p>
            <input type="text" id="clientName" placeholder="Full Name" style="width: 100%; padding: 18px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none;">
            <textarea id="projectDetails" rows="3" placeholder="Describe your vision..." style="width: 100%; padding: 18px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 15px; outline: none;"></textarea>
            <button class="prime-btn" onclick="sendToCEO()">
                <i class="fab fa-whatsapp"></i> <span id="btn-t">START CONVERSATION</span>
            </button>
        </div>

        <footer style="text-align: center; margin-top: 40px; opacity: 0.3; font-size: 0.7rem; letter-spacing: 1px;">
            PRIME SOLUTIONS GLOBAL HUB © 2026<br>
            Coded for Excellence by Nazim
        </footer>
    </div>

    <nav class="nav-dock">
        <div class="nav-item active" onclick="navigate('home')"><i class="fas fa-home-alt"></i></div>
        <div class="nav-item" onclick="navigate('services')"><i class="fas fa-shapes"></i></div>
        <div class="nav-item" onclick="navigate('contact')"><i class="fas fa-envelope-open-text"></i></div>
        <a href="tel:03705519562" class="nav-item" style="text-decoration:none;"><i class="fas fa-phone-alt"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        let lang = 'en';

        function toggleLang() {
            const btn = document.getElementById('langBtn');
            if(lang === 'en') {
                setLang('ur');
                btn.innerText = 'ENGLISH';
                lang = 'ur';
            } else {
                setLang('en');
                btn.innerText = 'URDU';
                lang = 'en';
            }
        }

        function setLang(l) {
            const t = {
                en: { name:"Muhammad Nazim", tag:"Architect of Digital Ecosystems | CEO", s1:"Projects", s2:"Global Clients", s3:"Rating ★", v1:"Next-Gen Web Apps", v2:"FinTech Portals", v3:"Global Brand SEO", ch:"Launch a Project", cp:"Direct bridge to Prime Solutions CEO", bt:"START CONVERSATION" },
                ur: { name:"محمد ناظم", tag:"ڈیجیٹل ایکو سسٹم کے معمار | سی ای او", s1:"پراجیکٹس", s2:"عالمی کلائنٹس", s3:"درجہ بندی ★", v1:"جدید ویب ایپس", v2:"فنانشل پورٹلز", v3:"گلوبل برانڈ ایس ای او", ch:"پراجیکٹ شروع کریں", cp:"پرائم سلوشنز سی ای او سے براہ راست رابطہ", bt:"بات چیت شروع کریں" }
            };
            const cur = t[l];
            document.getElementById('m-name').innerText = cur.name;
            document.getElementById('m-tag').innerText = cur.tag;
            document.getElementById('s1').innerText = cur.s1;
            document.getElementById('s2').innerText = cur.s2;
            document.getElementById('s3').innerText = cur.s3;
            document.getElementById('v1').innerText = cur.v1;
            document.getElementById('v2').innerText = cur.v2;
            document.getElementById('v3').innerText = cur.v3;
            document.getElementById('cont-h').innerText = cur.ch;
            document.getElementById('cont-p').innerText = cur.cp;
            document.getElementById('btn-t').innerText = cur.bt;
        }

        function sendToCEO() {
            const name = document.getElementById('clientName').value;
            const details = document.getElementById('projectDetails').value;
            const text = `Hello CEO Nazim! My name is ${name}. I have a vision: ${details}`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }
    </script>
</body>
</html>
