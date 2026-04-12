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
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: 0.3s ease; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        /* Floating Controls */
        .theme-btn { position: fixed; top: 20px; right: 20px; z-index: 3000; background: var(--card); border: 1px solid var(--border); padding: 12px; border-radius: 50%; cursor: pointer; backdrop-filter: blur(10px); color: var(--primary); }
        #scroll-path { position: fixed; top: 0; left: 0; width: 0%; height: 5px; background: linear-gradient(90deg, var(--primary), var(--accent)); z-index: 4000; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 60px 15px 120px; }

        /* Premium Card & Animated Glow */
        .card { 
            background: var(--card); backdrop-filter: blur(30px); border: 1px solid var(--border); 
            border-radius: 35px; padding: 25px; margin-bottom: 25px; position: relative;
            box-shadow: 0 10px 30px rgba(0,0,0,0.03); cursor: pointer;
        }
        .card:hover { transform: translateY(-10px); border-color: var(--primary); box-shadow: 0 20px 50px rgba(79, 172, 254, 0.2); }

        /* Detailed Service Items */
        .detail-item { background: rgba(0,0,0,0.03); border-radius: 20px; padding: 15px; margin-top: 10px; display: flex; align-items: center; gap: 15px; border: 1px solid var(--border); }
        .detail-item i { font-size: 1.5rem; color: var(--primary); }
        .detail-item h4 { font-size: 0.9rem; margin-bottom: 2px; }
        .detail-item p { font-size: 0.7rem; opacity: 0.6; }

        /* Smart Detailed Modal (Pop-up Page) */
        .modal { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: var(--bg); z-index: 5000; display: none; padding: 40px 20px; overflow-y: auto; animation: slideUp 0.5s forwards; }
        @keyframes slideUp { from { transform: translateY(100%); } to { transform: translateY(0); } }
        .close-modal { position: absolute; top: 20px; right: 20px; font-size: 1.5rem; cursor: pointer; }

        /* Trust & Verification */
        .verify-badge { display: flex; align-items: center; gap: 8px; font-size: 0.65rem; font-weight: 800; color: #25d366; background: rgba(37, 211, 102, 0.1); padding: 8px 15px; border-radius: 50px; width: fit-content; margin: 0 auto 15px; border: 1px solid rgba(37, 211, 102, 0.2); }

        /* Buttons */
        .btn-premium { display: flex; align-items: center; justify-content: center; gap: 10px; padding: 20px; border-radius: 25px; font-weight: 800; text-decoration: none; background: #25d366; color: white; margin-top: 15px; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); width: 100%; }
        
        /* Bottom Navigation Bar */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: var(--card); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .nav-link { color: var(--text); opacity: 0.5; font-size: 1.3rem; text-decoration: none; }
        .nav-link.active { color: var(--primary); opacity: 1; }
    </style>
</head>
<body data-theme="light">

    <div id="scroll-path"></div>
    <div class="theme-btn" onclick="toggleTheme()"><i class="fas fa-moon"></i></div>

    <div class="container">
        
        <section class="card" data-aos="zoom-in" style="text-align: center;">
            <div class="verify-badge"><i class="fas fa-user-shield"></i> GOOGLE VERIFIED DEVELOPER</div>
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" style="width: 125px; height: 125px; border-radius: 50%; border: 4px solid var(--primary); padding: 4px;">
            <h1 style="font-size: 2.4rem; font-weight: 800; margin-top: 15px; background: linear-gradient(135deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Muhammad Nazim</h1>
            <p style="opacity: 0.6; font-size: 0.9rem;">Founder & CEO | Prime Solutions</p>
        </section>

        <div class="card" data-aos="fade-up" onclick="openModal('service-details')">
            <h3><i class="fas fa-layer-group" style="color: var(--primary);"></i> Premium Services</h3>
            <p style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 15px;">Tap to see full details & pricing</p>
            
            <div class="detail-item">
                <i class="fas fa-code"></i>
                <div><h4>Full-Stack Development</h4><p>Custom websites with high security.</p></div>
            </div>
            <div class="detail-item">
                <i class="fas fa-chart-line"></i>
                <div><h4>Investment Platforms</h4><p>Deposit, Profit & Withdrawal logs.</p></div>
            </div>
            <div style="text-align: center; margin-top: 15px; font-size: 0.8rem; color: var(--primary); font-weight: 800;">READ MORE DETAILS <i class="fas fa-chevron-right"></i></div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-shield-alt" style="color: #25d366;"></i> Why Clients Trust Us</h3>
            <div style="margin-top: 15px;">
                <div style="display: flex; gap: 5px; color: #ffca28; margin-bottom: 10px;">
                    <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                </div>
                <p style="font-size: 0.8rem; font-style: italic; line-height: 1.5;">"Prime Solutions build quality is top-notch. They handled our Web-Hub project with extreme professionalism and security."</p>
                <p style="font-size: 0.65rem; font-weight: 800; margin-top: 10px; color: var(--primary);">— Verified Business Owner</p>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 6px solid var(--primary);">
            <h3 style="text-align: center;">Ready for Launch?</h3>
            <a href="https://wa.me/923332637235" class="btn-premium">
                <i class="fab fa-whatsapp"></i> Start WhatsApp Chat
            </a>
            <a href="tel:03705519562" style="display: block; text-align: center; margin-top: 15px; color: var(--text); text-decoration: none; font-weight: 800;">
                <i class="fas fa-phone-alt"></i> Call: 0370 5519562
            </a>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.4;">
            © 2026 PRIME SOLUTIONS | ALL RIGHTS RESERVED<br>
            Coded with Heart for Professional Excellence
        </footer>
    </div>

    <div id="service-details" class="modal">
        <i class="fas fa-times close-modal" onclick="closeModal('service-details')"></i>
        <h2 style="font-size: 2rem; margin-bottom: 20px;">Full Service Details</h2>
        
        <div style="margin-bottom: 30px;">
            <h3 style="color: var(--primary);">1. Financial Platforms</h3>
            <p style="font-size: 0.9rem; opacity: 0.7; margin-top: 10px;">Hum advanced investment sites banate hain jisme automatic profit tracking, referral systems, aur secure deposit methods (EasyPaisa/JazzCash) shamil hote hain.</p>
        </div>

        <div style="margin-bottom: 30px;">
            <h3 style="color: var(--primary);">2. E-Commerce Solutions</h3>
            <p style="font-size: 0.9rem; opacity: 0.7; margin-top: 10px;">Modern online stores with inventory management, order tracking, aur high-speed checkouts.</p>
        </div>

        <div style="margin-bottom: 30px;">
            <h3 style="color: var(--primary);">3. UI/UX Innovation</h3>
            <p style="font-size: 0.9rem; opacity: 0.7; margin-top: 10px;">Aapki website aik application ki tarah lagegi (Mobile-First approach), jaisa ke Prime Academy App.</p>
        </div>

        <button onclick="closeModal('service-details')" class="btn-premium">Back to Home</button>
    </div>

    <nav class="nav-bar">
        <a href="#" class="nav-link active"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        function toggleTheme() {
            const body = document.body;
            const icon = document.querySelector('.theme-btn i');
            if(body.getAttribute('data-theme') === 'light') {
                body.setAttribute('data-theme', 'dark');
                icon.className = 'fas fa-sun';
            } else {
                body.setAttribute('data-theme', 'light');
                icon.className = 'fas fa-moon';
            }
        }

        function openModal(id) { document.getElementById(id).style.display = 'block'; document.body.style.overflow = 'hidden'; }
        function closeModal(id) { document.getElementById(id).style.display = 'none'; document.body.style.overflow = 'auto'; }

        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("scroll-path").style.width = (winScroll / height) * 100 + "%";
        };
    </script>
</body>
</html>
