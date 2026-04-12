<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Prime Solutions Infinity</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #4facfe; --secondary: #00f2fe; --accent: #f093fb;
            --bg: #fdfdfd; --text: #1d1d1f; --card: rgba(255, 255, 255, 0.9); --border: rgba(0, 0, 0, 0.08);
            --glow: rgba(79, 172, 254, 0.2);
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
            --glow: rgba(255, 255, 255, 0.05);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: 0.4s cubic-bezier(0.4, 0, 0.2, 1); }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        /* Floating Controls & Progress */
        #scroll-tracker { position: fixed; top: 0; left: 0; width: 0%; height: 5px; background: linear-gradient(90deg, var(--primary), var(--accent)); z-index: 9999; }
        .theme-switcher { position: fixed; top: 20px; right: 20px; z-index: 3000; background: var(--card); border: 1px solid var(--border); padding: 12px; border-radius: 50%; cursor: pointer; backdrop-filter: blur(15px); color: var(--primary); box-shadow: 0 10px 20px rgba(0,0,0,0.1); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 60px 15px 120px; }

        /* Infinity Cards */
        .card { 
            background: var(--card); backdrop-filter: blur(30px); border: 1px solid var(--border); 
            border-radius: 35px; padding: 28px; margin-bottom: 25px; position: relative;
            box-shadow: 0 15px 35px rgba(0,0,0,0.03); overflow: hidden;
        }
        .card:hover { transform: translateY(-10px); border-color: var(--primary); box-shadow: 0 25px 50px var(--glow); }

        /* Hero Styling */
        .verify-tag { display: flex; align-items: center; gap: 8px; font-size: 0.65rem; font-weight: 800; color: #25d366; background: rgba(37, 211, 102, 0.1); padding: 8px 15px; border-radius: 50px; width: fit-content; margin: 0 auto 15px; border: 1px solid rgba(37, 211, 102, 0.2); }
        .profile-pfp { width: 130px; height: 130px; border-radius: 50%; border: 4px solid var(--primary); padding: 5px; margin-bottom: 15px; }

        /* Clickable Service Sections */
        .service-item { background: rgba(0,0,0,0.02); border: 1px solid var(--border); border-radius: 20px; padding: 18px; margin-top: 12px; display: flex; align-items: center; gap: 15px; cursor: pointer; transition: 0.3s; }
        .service-item:hover { background: var(--primary); color: white; transform: scale(1.02); }
        .service-item i { font-size: 1.4rem; }

        /* Premium Modals (Virtual Pages) */
        .smart-modal { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: var(--bg); z-index: 5000; display: none; padding: 40px 25px; overflow-y: auto; animation: slideIn 0.5s ease-out; }
        @keyframes slideIn { from { transform: translateY(100%); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .close-btn { position: absolute; top: 25px; right: 25px; font-size: 1.8rem; cursor: pointer; color: var(--primary); }

        /* Statistics & Trust */
        .stat-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-top: 15px; }
        .stat-card { background: rgba(79, 172, 254, 0.05); padding: 15px; border-radius: 20px; text-align: center; border: 1px solid var(--border); }
        .stat-card h2 { color: var(--primary); font-size: 1.8rem; }

        /* Bottom Menu */
        .bottom-nav { position: fixed; bottom: 30px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 420px; background: var(--card); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .nav-link { color: var(--text); opacity: 0.5; font-size: 1.4rem; text-decoration: none; }
        .nav-link.active { color: var(--primary); opacity: 1; transform: translateY(-5px); }

        .btn-cta { display: flex; align-items: center; justify-content: center; gap: 12px; padding: 22px; border-radius: 28px; font-weight: 800; text-decoration: none; background: #25d366; color: white; margin-top: 20px; box-shadow: 0 10px 25px rgba(37, 211, 102, 0.3); width: 100%; font-size: 1.1rem; }
    </style>
</head>
<body data-theme="light">

    <div id="scroll-tracker"></div>
    <div class="theme-switcher" onclick="toggleTheme()"><i class="fas fa-moon"></i></div>

    <div class="container">
        
        <section class="card" data-aos="zoom-in" style="text-align: center;">
            <div class="verify-tag"><i class="fas fa-certificate"></i> OFFICIAL VERIFIED OWNER</div>
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pfp">
            <h1 style="font-size: 2.5rem; font-weight: 800; letter-spacing: -1px; background: linear-gradient(135deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
            <p style="opacity: 0.6; font-weight: 400;">Founder & CEO | Prime Solutions Agency</p>
            
            <div class="stat-grid">
                <div class="stat-card"><h2>50+</h2><p style="font-size: 0.6rem;">PROJECTS</p></div>
                <div class="stat-card"><h2>100%</h2><p style="font-size: 0.6rem;">TRUSTED</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-rocket" style="color: var(--primary);"></i> Premium Solutions</h3>
            <p style="font-size: 0.75rem; opacity: 0.5; margin-bottom: 15px;">Click items to explore details</p>
            
            <div class="service-item" onclick="openPage('web-page')">
                <i class="fas fa-code"></i>
                <div><h4>Full-Stack Web Development</h4><p>High speed, clean code, SEO ready.</p></div>
            </div>
            
            <div class="service-item" onclick="openPage('fin-page')">
                <i class="fas fa-vault"></i>
                <div><h4>Investment Platforms</h4><p>Secure profit, deposit & withdraw logs.</p></div>
            </div>

            <div class="service-item" onclick="openPage('app-page')">
                <i class="fas fa-mobile-screen"></i>
                <div><h4>Mobile-Style UI/UX</h4><p>Make websites look like premium apps.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-user-shield" style="color: #25d366;"></i> Why We Are Best?</h3>
            <ul style="list-style: none; margin-top: 15px;">
                <li style="font-size: 0.85rem; margin-bottom: 12px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> 100% Secure Transaction & Privacy</li>
                <li style="font-size: 0.85rem; margin-bottom: 12px;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> Professional NDA Agreement</li>
                <li style="font-size: 0.85rem;"><i class="fas fa-check-circle" style="color: var(--primary);"></i> 24/7 VIP Maintenance Support</li>
            </ul>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 8px solid var(--primary);">
            <h3 style="text-align: center;">Let's Talk Success</h3>
            <a href="https://wa.me/923332637235" class="btn-cta">
                <i class="fab fa-whatsapp"></i> Chat on WhatsApp
            </a>
            <a href="tel:03705519562" style="display: block; text-align: center; margin-top: 15px; color: var(--text); text-decoration: none; font-weight: 800;">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
        </div>

        <footer style="text-align: center; font-size: 0.75rem; opacity: 0.4;">
            © 2026 PRIME SOLUTIONS | EXCELLENCE IN CODE<br>
            Designed & Developed by Muhammad Nazim
        </footer>
    </div>

    <div id="web-page" class="smart-modal">
        <i class="fas fa-times close-btn" onclick="closePage('web-page')"></i>
        <h2 style="color: var(--primary); margin-bottom: 20px;">Web Development Details</h2>
        <p style="line-height: 1.8; opacity: 0.8;">Hum modern technlogies jaise HTML, CSS, JS, aur Firebase use karte hain. Aapka project GitHub Pages ya Netlify par fast hosting ke saath setup kiya jayega.</p>
        <div class="stat-card" style="margin-top: 20px;"><h4>99.9% Server Uptime</h4></div>
        <button onclick="closePage('web-page')" class="btn-cta" style="background: var(--primary);">Back to Home</button>
    </div>

    <div id="fin-page" class="smart-modal">
        <i class="fas fa-times close-btn" onclick="closePage('fin-page')"></i>
        <h2 style="color: var(--primary); margin-bottom: 20px;">Financial Systems</h2>
        <p style="line-height: 1.8; opacity: 0.8;">Investment websites (Pakgold Style) humari specialty hain. Hum Real-time Dashboards, Daily Profit Tracking, aur Secure Withdrawal logs implement karte hain.</p>
        <button onclick="closePage('fin-page')" class="btn-cta" style="background: var(--primary);">Back to Home</button>
    </div>

    <div id="app-page" class="smart-modal">
        <i class="fas fa-times close-btn" onclick="closePage('app-page')"></i>
        <h2 style="color: var(--primary); margin-bottom: 20px;">UI/UX Innovation</h2>
        <p style="line-height: 1.8; opacity: 0.8;">Hum websites ko simple browser sites se badal kar mobile apps jaisa look dete hain (Bottom Navigation, Smooth Icons, App-Feel Buttons).</p>
        <button onclick="closePage('app-page')" class="btn-cta" style="background: var(--primary);">Back to Home</button>
    </div>

    <nav class="bottom-nav">
        <a href="#" class="nav-link active"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope-open-text"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Theme Toggle
        function toggleTheme() {
            const body = document.body;
            const icon = document.querySelector('.theme-switcher i');
            if(body.getAttribute('data-theme') === 'light') {
                body.setAttribute('data-theme', 'dark');
                icon.className = 'fas fa-sun';
            } else {
                body.setAttribute('data-theme', 'light');
                icon.className = 'fas fa-moon';
            }
        }

        // Virtual Page Handlers
        function openPage(id) { document.getElementById(id).style.display = 'block'; document.body.style.overflow = 'hidden'; }
        function closePage(id) { document.getElementById(id).style.display = 'none'; document.body.style.overflow = 'auto'; }

        // Scroll Tracking
        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("scroll-tracker").style.width = (winScroll / height) * 100 + "%";
        };
    </script>
</body>
</html>
