<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | CEO Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Premium Glass Card */
        .card { 
            background: var(--glass); backdrop-filter: blur(25px); 
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 28px; margin-bottom: 22px; transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative; overflow: hidden;
        }
        .card:hover { transform: translateY(-10px); border-color: var(--primary); box-shadow: 0 20px 40px rgba(0, 242, 254, 0.2); }
        
        /* Floating WhatsApp Button */
        .wa-float { position: fixed; bottom: 100px; right: 20px; background: #25d366; color: white; width: 55px; height: 55px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 30px; z-index: 1001; box-shadow: 0 10px 20px rgba(0,0,0,0.3); animation: pulse 2s infinite; text-decoration: none; }
        @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.1); } 100% { transform: scale(1); } }

        /* Hero Styling */
        .hero { text-align: center; padding: 40px 10px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 3px solid var(--primary); padding: 5px; margin-bottom: 15px; box-shadow: 0 0 30px rgba(0, 242, 254, 0.4); object-fit: cover; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.3rem; }
        
        /* Typewriter Title */
        .typewriter { font-size: 1rem; color: var(--primary); font-weight: 400; min-height: 20px; margin-top: 5px; opacity: 0.9; }

        /* Stats */
        .stats-grid { display: flex; justify-content: space-around; text-align: center; margin-top: 25px; }
        .counter { color: white; font-size: 1.8rem; font-weight: 800; display: block; }
        .stat-item p { font-size: 0.7rem; opacity: 0.6; text-transform: uppercase; letter-spacing: 1px; }

        /* Project Badge */
        .project-item { background: rgba(255,255,255,0.03); border-radius: 20px; padding: 15px; margin-top: 10px; border: 1px solid var(--border); display: flex; align-items: center; gap: 12px; }
        .project-icon { width: 40px; height: 40px; background: var(--primary); color: #000; border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 1.2rem; }

        /* Navigation */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 400px; background: rgba(10, 10, 10, 0.9); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; box-shadow: 0 10px 30px rgba(0,0,0,0.5); }
        .nav-link { color: white; font-size: 1.4rem; opacity: 0.6; transition: 0.3s; }
        .nav-link:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* Buttons */
        .btn-primary { background: linear-gradient(45deg, #00f2fe, #4facfe); color: #000; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 10px; margin-top: 15px; border: none; font-size: 1rem; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <a href="https://wa.me/923332637235" class="wa-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <nav class="nav-bar">
        <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <div class="typewriter" id="typewriter"></div>
            
            <div class="stats-grid">
                <div class="stat-item"><span class="counter" data-target="50">0</span><p>Projects</p></div>
                <div class="stat-item"><span class="counter" data-target="15">0</span><p>Global Clients</p></div>
                <div class="stat-item"><span class="counter" data-target="100">0</span><p>Success</p></div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-briefcase" style="color: var(--primary);"></i> Featured Work</h3>
            <div class="project-item">
                <div class="project-icon"><i class="fas fa-chart-pie"></i></div>
                <div><h4 style="font-size: 0.9rem;">Investment Dashboard</h4><p style="font-size: 0.7rem; opacity: 0.6;">Real-time finance tracking system.</p></div>
            </div>
            <div class="project-item">
                <div class="project-icon"><i class="fas fa-comments"></i></div>
                <div><h4 style="font-size: 0.9rem;">Live Connect Chat</h4><p style="font-size: 0.7rem; opacity: 0.6;">Firebase powered messaging app.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-bolt" style="color: var(--accent);"></i> Prime Core</h3>
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px;">
                <div style="padding: 10px; background: rgba(255,255,255,0.05); border-radius: 15px; font-size: 0.8rem; text-align: center;">🚀 React JS</div>
                <div style="padding: 10px; background: rgba(255,255,255,0.05); border-radius: 15px; font-size: 0.8rem; text-align: center;">🔥 Firebase</div>
                <div style="padding: 10px; background: rgba(255,255,255,0.05); border-radius: 15px; font-size: 0.8rem; text-align: center;">🎨 UI/UX</div>
                <div style="padding: 10px; background: rgba(255,255,255,0.05); border-radius: 15px; font-size: 0.8rem; text-align: center;">🛡️ SEO Guru</div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-bottom: 5px solid var(--primary);">
            <h2 style="text-align: center; margin-bottom: 10px;">Ready to Scale?</h2>
            <a href="https://wa.me/923332637235" class="btn-primary">
                <i class="fas fa-paper-plane"></i> Hire Prime Solutions
            </a>
            <p style="text-align: center; font-size: 0.7rem; margin-top: 15px; opacity: 0.5;">Free Consultation & Money Back Guarantee</p>
        </div>

        <footer style="text-align: center; font-size: 0.8rem; opacity: 0.3;">
            © 2026 PRIME SOLUTIONS | MADE WITH LOVE
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Typewriter Effect
        const textElement = document.getElementById('typewriter');
        const phrases = ["Digital Architect", "Founder Prime Solutions", "Full-Stack Web Developer", "UI/UX Specialist"];
        let phraseIndex = 0; let charIndex = 0;

        function type() {
            if (charIndex < phrases[phraseIndex].length) {
                textElement.innerHTML += phrases[phraseIndex].charAt(charIndex);
                charIndex++; setTimeout(type, 100);
            } else { setTimeout(erase, 2000); }
        }
        function erase() {
            if (charIndex > 0) {
                textElement.innerHTML = phrases[phraseIndex].substring(0, charIndex - 1);
                charIndex--; setTimeout(erase, 50);
            } else { phraseIndex = (phraseIndex + 1) % phrases.length; setTimeout(type, 500); }
        }
        window.onload = type;

        // Counter Logic
        const counters = document.querySelectorAll('.counter');
        counters.forEach(counter => {
            const update = () => {
                const target = +counter.getAttribute('data-target');
                const count = +counter.innerText;
                const inc = target / 200;
                if (count < target) {
                    counter.innerText = Math.ceil(count + inc);
                    setTimeout(update, 10);
                } else { counter.innerText = target + (target === 100 ? '%' : '+'); }
            };
            update();
        });
    </script>
</body>
</html>
