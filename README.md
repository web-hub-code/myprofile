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

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Multi-Page Logic */
        .page-content { display: none; animation: slideUp 0.5s ease forwards; }
        .page-content.active { display: block; }
        @keyframes slideUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }

        /* Top Bar */
        .top-nav { display: flex; justify-content: space-between; align-items: center; padding: 15px 20px; background: var(--glass); backdrop-filter: blur(15px); border-radius: 50px; border: 1px solid var(--border); margin-bottom: 25px; }

        /* Modern Cards */
        .card { background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 20px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); box-shadow: 0 10px 30px rgba(0, 242, 254, 0.1); }

        /* Stats Branding */
        .stat-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px; margin-top: 25px; text-align: center; }
        .stat-val { color: var(--primary); font-size: 1.5rem; font-weight: 800; }
        .stat-label { font-size: 0.6rem; opacity: 0.5; text-transform: uppercase; }

        /* Floating Nav */
        .dock { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 450px; background: rgba(10,10,10,0.8); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 20px 50px rgba(0,0,0,0.5); }
        .dock-item { color: white; opacity: 0.4; font-size: 1.3rem; cursor: pointer; transition: 0.3s; }
        .dock-item.active { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* Buttons */
        .btn-global { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; border-radius: 22px; border: none; font-weight: 800; cursor: pointer; width: 100%; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 15px; }
        
        /* AI Assistant */
        .ai-bubble { position: fixed; bottom: 100px; right: 20px; background: var(--primary); color: #000; padding: 10px 15px; border-radius: 20px 20px 0 20px; font-size: 0.7rem; font-weight: 800; z-index: 999; animation: float 3s infinite; }
        @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-8px); } }
    </style>
</head>
<body>

    <div class="ai-bubble">CEO Nazim is Online! 🟢</div>

    <div class="container">
        <div class="top-nav">
            <span style="font-weight: 800; color: var(--primary); font-size: 0.8rem;">PRIME SOLUTIONS GLOBAL</span>
            <button onclick="toggleLang()" id="lBtn" style="background:var(--primary); border:none; padding:5px 12px; border-radius:50px; font-weight:800; font-size:0.6rem; cursor:pointer;">URDU</button>
        </div>

        <div id="p-home" class="page-content active">
            <div class="card" style="text-align: center;">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" style="width: 120px; height: 120px; border-radius: 50%; border: 3px solid var(--primary); margin-bottom: 15px;">
                <h1 style="font-size: 2.3rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;" id="n-txt">Muhammad Nazim</h1>
                <p style="opacity: 0.7;" id="t-txt">Founder & Global CEO | Prime Solutions</p>
                
                <div class="stat-grid">
                    <div><div class="stat-val">150+</div><div class="stat-label" id="s1">Success Projects</div></div>
                    <div><div class="stat-val">50+</div><div class="stat-label" id="s2">Global Partners</div></div>
                    <div><div class="stat-val">5.0</div><div class="stat-label" id="s3">Client Rating</div></div>
                </div>
            </div>
            
            <div class="card">
                <h3 id="a-h"><i class="fas fa-rocket"></i> Agency Mission</h3>
                <p id="a-p" style="font-size: 0.8rem; opacity: 0.6; margin-top: 10px; line-height: 1.6;">Hum dunya ki top 1 agency banne ke liye commit hain, har project ko international standards ke mutabiq build karte hain.</p>
                <button class="btn-global" onclick="navTo('contact')">Let's Talk Business</button>
            </div>
        </div>

        <div id="p-services" class="page-content">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-layer-group"></i> World-Class Services</h3>
            <div class="card">
                <h4>FinTech & Investment</h4>
                <p style="font-size: 0.75rem; opacity: 0.6;">Secure financial ecosystems with real-time profit tracking.</p>
            </div>
            <div class="card">
                <h4>Enterprise E-Commerce</h4>
                <p style="font-size: 0.75rem; opacity: 0.6;">Multi-vendor stores with global payment integration.</p>
            </div>
            <div class="card">
                <h4>AI-Driven Development</h4>
                <p style="font-size: 0.75rem; opacity: 0.6;">Smart applications with automated logic and high speed.</p>
            </div>
        </div>

        <div id="p-contact" class="page-content">
            <div class="card">
                <h3 id="c-h">Direct CEO Inquiry</h3>
                <p id="c-p" style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 20px;">Your data is secured with professional NDA.</p>
                <input type="text" id="cName" placeholder="Full Name" style="width: 100%; padding: 18px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px; outline: none;">
                <textarea id="cMsg" rows="3" placeholder="Describe your project vision..." style="width: 100%; padding: 18px; border-radius: 20px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 15px; outline: none;"></textarea>
                <button class="btn-global" onclick="sendInquiry()">
                    <i class="fab fa-whatsapp"></i> START PROJECT NOW
                </button>
            </div>
        </div>

        <footer style="text-align: center; opacity: 0.3; font-size: 0.7rem;">
            WORLD'S TOP RATED AGENCY | PRIME SOLUTIONS © 2026
        </footer>
    </div>

    <nav class="dock">
        <div class="dock-item active" onclick="navTo('home')"><i class="fas fa-house"></i></div>
        <div class="dock-item" onclick="navTo('services')"><i class="fas fa-shapes"></i></div>
        <div class="dock-item" onclick="navTo('contact')"><i class="fas fa-paper-plane"></i></div>
        <a href="tel:03705519562" class="dock-item" style="text-decoration:none;"><i class="fas fa-phone"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000 });
        let currentLang = 'en';

        function navTo(page) {
            document.querySelectorAll('.page-content').forEach(p => p.classList.remove('active'));
            document.getElementById('p-'+page).classList.add('active');
            document.querySelectorAll('.dock-item').forEach(i => i.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        function toggleLang() {
            const btn = document.getElementById('lBtn');
            if(currentLang === 'en') {
                updateText('ur');
                btn.innerText = 'ENGLISH';
                currentLang = 'ur';
            } else {
                updateText('en');
                btn.innerText = 'URDU';
                currentLang = 'en';
            }
        }

        function updateText(l) {
            const data = {
                en: { n:"Muhammad Nazim", t:"Founder & Global CEO | Prime Solutions", s1:"Success Projects", s2:"Global Partners", s3:"Client Rating", ah:"Agency Mission", ap:"We are committed to being the world's top 1 agency, building every project to international standards.", ch:"Direct CEO Inquiry", cp:"Your data is secured with professional NDA." },
                ur: { n:"محمد ناظم", t:"بانی اور عالمی سی ای او | پرائم سلوشنز", s1:"کامیاب پراجیکٹس", s2:"عالمی شراکت دار", s3:"کلائنٹ ریٹنگ", ah:"ایجنسی کا مشن", ap:"ہم دنیا کی ٹاپ 1 ایجنسی بننے کے لیے پرعزم ہیں، ہر پراجیکٹ کو بین الاقوامی معیار کے مطابق بناتے ہیں۔", ch:"براہ راست سی ای او انکوائری", cp:"آپ کا ڈیٹا پروفیشنل NDA کے ساتھ محفوظ ہے۔" }
            };
            const d = data[l];
            document.getElementById('n-txt').innerText = d.n;
            document.getElementById('t-txt').innerText = d.t;
            document.getElementById('s1').innerText = d.s1;
            document.getElementById('s2').innerText = d.s2;
            document.getElementById('s3').innerText = d.s3;
            document.getElementById('a-h').innerText = d.ah;
            document.getElementById('a-p').innerText = d.ap;
            document.getElementById('c-h').innerText = d.ch;
            document.getElementById('c-p').innerText = d.cp;
        }

        function sendInquiry() {
            const n = document.getElementById('cName').value;
            const m = document.getElementById('cMsg').value;
            window.location.href = `https://wa.me/923332637235?text=Hello CEO Nazim! I am ${n}. Vision: ${m}`;
        }
    </script>
</body>
</html>
