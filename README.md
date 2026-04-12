<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Global Prime Solutions 2026</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Floating AI Assistant Mockup */
        .ai-assistant { position: fixed; bottom: 100px; right: 20px; background: var(--primary); color: #000; padding: 10px 15px; border-radius: 20px 20px 0 20px; font-size: 0.7rem; font-weight: 800; z-index: 5000; box-shadow: 0 5px 15px rgba(0,242,254,0.4); animation: bounce 2s infinite; }
        @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-5px); } }

        /* Page Layouts */
        .page-section { display: none; animation: fadeIn 0.5s ease; }
        .page-section.active { display: block; }
        @keyframes fadeIn { from { opacity: 0; transform: scale(0.95); } to { opacity: 1; transform: scale(1); } }

        .card { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 20px; position: relative; overflow: hidden; }

        /* Global Stats Bar */
        .global-bar { display: flex; justify-content: space-between; margin-bottom: 25px; padding: 10px; border-radius: 50px; background: rgba(255,255,255,0.02); border: 1px solid var(--border); }
        .g-stat { font-size: 0.6rem; opacity: 0.6; font-weight: 800; }

        /* Portfolio Grid */
        .project-card { background: rgba(0,0,0,0.3); border-radius: 20px; padding: 15px; border: 1px solid var(--border); margin-bottom: 15px; }
        .tag { display: inline-block; padding: 4px 10px; border-radius: 50px; font-size: 0.5rem; background: var(--primary); color: #000; margin-bottom: 10px; font-weight: 800; }

        /* Custom UI Buttons */
        .btn-glow { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; border: none; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; }
        
        /* Bottom Sticky Nav */
        .tab-bar { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: rgba(10,10,10,0.9); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 4000; }
        .tab-icon { color: white; opacity: 0.4; font-size: 1.2rem; cursor: pointer; }
        .tab-icon.active { color: var(--primary); opacity: 1; }
    </style>
</head>
<body>

    <div class="ai-assistant" id="aiBubble">Hi! I'm Nazim's AI. Need a website?</div>

    <div class="container">
        
        <div class="global-bar">
            <span class="g-stat"><i class="fas fa-globe"></i> GLOBAL STATUS: ACTIVE</span>
            <span class="g-stat"><i class="fas fa-clock"></i> RESPONSE: 30 MINS</span>
        </div>

        <section id="home" class="page-section active">
            <div class="card" style="text-align: center;">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" style="width: 110px; height: 110px; border-radius: 50%; border: 3px solid var(--primary); margin-bottom: 15px;">
                <h1 style="font-size: 2.2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
                <p style="opacity: 0.7; font-size: 0.9rem;">Expert Full-Stack Developer & Founder</p>
                
                <div style="display: flex; justify-content: center; gap: 20px; margin-top: 20px;">
                    <div><h3 style="color: var(--primary);">150+</h3><p style="font-size: 0.5rem; opacity: 0.5;">LIVE PROJECTS</p></div>
                    <div><h3 style="color: var(--primary);">50+</h3><p style="font-size: 0.5rem; opacity: 0.5;">CLIENTS</p></div>
                    <div><h3 style="color: var(--primary);">100%</h3><p style="font-size: 0.5rem; opacity: 0.5;">SUCCESS</p></div>
                </div>
            </div>

            <div class="card">
                <h3><i class="fas fa-microchip"></i> Prime Tech Stack</h3>
                <div style="display: flex; flex-wrap: wrap; gap: 8px; margin-top: 15px;">
                    <span style="background: rgba(255,255,255,0.05); padding: 5px 12px; border-radius: 50px; font-size: 0.7rem; border: 1px solid var(--border);">React.js</span>
                    <span style="background: rgba(255,255,255,0.05); padding: 5px 12px; border-radius: 50px; font-size: 0.7rem; border: 1px solid var(--border);">Firebase</span>
                    <span style="background: rgba(255,255,255,0.05); padding: 5px 12px; border-radius: 50px; font-size: 0.7rem; border: 1px solid var(--border);">Node.js</span>
                    <span style="background: rgba(255,255,255,0.05); padding: 5px 12px; border-radius: 50px; font-size: 0.7rem; border: 1px solid var(--border);">Python</span>
                </div>
            </div>
        </section>

        <section id="portfolio" class="page-section">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-briefcase"></i> Master Portfolio</h3>
            <div class="project-card">
                <span class="tag">INVESTMENT PLATFORM</span>
                <h4>PakGold Official Portal</h4>
                <p style="font-size: 0.7rem; opacity: 0.6; margin-top: 5px;">Features: Live Profit Tracking, Auto-Deposit, Admin Dashboard.</p>
                <button style="background: transparent; border: 1px solid var(--primary); color: var(--primary); padding: 5px 15px; border-radius: 50px; margin-top: 10px; font-size: 0.6rem;">VIEW CASE STUDY</button>
            </div>
            <div class="project-card">
                <span class="tag">ECOMMERCE</span>
                <h4>Prime Mart Global</h4>
                <p style="font-size: 0.7rem; opacity: 0.6; margin-top: 5px;">Features: Multi-vendor, Secure Stripe Payment, Order Tracking.</p>
                <button style="background: transparent; border: 1px solid var(--primary); color: var(--primary); padding: 5px 15px; border-radius: 50px; margin-top: 10px; font-size: 0.6rem;">VIEW CASE STUDY</button>
            </div>
        </section>

        <section id="contact" class="page-section">
            <div class="card">
                <h3><i class="fas fa-envelope"></i> Hire Prime Solutions</h3>
                <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 20px;">Direct access to Muhammad Nazim</p>
                
                <input type="text" id="client" placeholder="Your Name" style="width: 100%; padding: 15px; border-radius: 15px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px;">
                <select id="service" style="width: 100%; padding: 15px; border-radius: 15px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); color: white; margin-bottom: 12px;">
                    <option>Investment Website</option>
                    <option>E-Commerce Store</option>
                    <option>Business Branding</option>
                </select>
                <button class="btn-glow" onclick="orderNow()">
                    <i class="fab fa-whatsapp"></i> START PROJECT
                </button>
            </div>
        </section>

        <footer style="text-align: center; opacity: 0.3; font-size: 0.7rem; margin-top: 30px;">
            VERIFIED PRIME SOLUTIONS HUB 2026<br>
            PRIVACY SECURED | LIFETIME SUPPORT
        </footer>

    </div>

    <nav class="tab-bar">
        <div class="tab-icon active" onclick="navigate('home')"><i class="fas fa-th-large"></i></div>
        <div class="tab-icon" onclick="navigate('portfolio')"><i class="fas fa-rocket"></i></div>
        <div class="tab-icon" onclick="navigate('contact')"><i class="fas fa-comment-alt"></i></div>
        <a href="tel:03705519562" class="tab-icon" style="text-decoration: none;"><i class="fas fa-phone"></i></a>
    </nav>

    <script>
        function navigate(id) {
            document.querySelectorAll('.page-section').forEach(p => p.classList.remove('active'));
            document.getElementById(id).classList.add('active');
            document.querySelectorAll('.tab-icon').forEach(t => t.classList.remove('active'));
            event.currentTarget.classList.add('active');
            window.scrollTo(0,0);
        }

        function orderNow() {
            const name = document.getElementById('client').value;
            const type = document.getElementById('service').value;
            const text = `Hello Nazim! My name is ${name}. I want to discuss an ${type}.`;
            window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(text)}`;
        }

        // AI Bubble Animation
        const messages = ["Need a Pro Website?", "I'm Online Now!", "Check my Work!", "Free Quote?"];
        let i = 0;
        setInterval(() => {
            document.getElementById('aiBubble').innerText = messages[i];
            i = (i + 1) % messages.length;
        }, 4000);
    </script>
</body>
</html>
