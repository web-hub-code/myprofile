<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Elite Identity</title>
    
    <meta name="description" content="Muhammad Nazim - Professional Web Solutions & Digital Expert">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #030508; --glass: rgba(255, 255, 255, 0.07); --border: rgba(255, 255, 255, 0.12);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; width: 100%; }

        /* Background Video Overlay */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.22); }
        .v-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 20%, #000 100%); z-index: -1; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Glass Cards */
        .card { background: var(--glass); backdrop-filter: blur(25px); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 20px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }

        .hero { text-align: center; padding: 50px 20px; }
        .profile-pic { width: 135px; height: 135px; border-radius: 50%; border: 4px solid var(--primary); object-fit: cover; box-shadow: 0 0 40px rgba(0, 242, 254, 0.4); margin-bottom: 15px; }
        
        h1 { font-size: 2.2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Skill Glowing Chips */
        .skills-grid { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 15px; }
        .skill-chip { background: rgba(255,255,255,0.05); border: 1px solid var(--border); padding: 8px 15px; border-radius: 50px; font-size: 0.85rem; display: flex; align-items: center; gap: 8px; }
        .skill-chip i { color: var(--primary); }

        /* Copy Button & Music Toggle */
        .copy-btn { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 16px; width: 100%; border-radius: 18px; font-weight: 700; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; font-size: 1rem; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.2); }
        
        .music-toggle { position: fixed; top: 20px; right: 20px; background: var(--glass); width: 45px; height: 45px; border-radius: 50%; display: flex; align-items: center; justify-content: center; border: 1px solid var(--border); z-index: 1001; color: var(--primary); cursor: pointer; }

        /* Bottom Menu */
        .bottom-nav { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; background: rgba(0,0,0,0.8); backdrop-filter: blur(25px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 1000; box-shadow: 0 20px 40px rgba(0,0,0,0.5); }
        .nav-item { color: white; font-size: 1.3rem; transition: 0.3s; opacity: 0.7; }
        .nav-item:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; padding-bottom: 20px; letter-spacing: 1px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="v-overlay"></div>

    <div class="music-toggle" onclick="toggleMusic()"><i class="fas fa-music"></i></div>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="https://instagram.com/mr_nazim073" target="_blank" class="nav-item"><i class="fab fa-instagram"></i></a>
        <a href="https://wa.me/923000000000" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Muhammad Nazim</h1>
            <p style="color: var(--primary); font-size: 0.85rem; margin-top: 8px; font-weight: 600; letter-spacing: 2px;">WEB ARCHITECT & BRANDING EXPERT</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="font-size: 1.1rem; margin-bottom: 15px;"><i class="fas fa-rocket" style="color: var(--accent);"></i> My Stack</h3>
            <div class="skills-grid">
                <div class="skill-chip"><i class="fab fa-html5"></i> HTML5</div>
                <div class="skill-chip"><i class="fab fa-css3-alt"></i> CSS3</div>
                <div class="skill-chip"><i class="fas fa-mobile-alt"></i> Responsive</div>
                <div class="skill-chip"><i class="fas fa-paint-brush"></i> UI/UX</div>
                <div class="skill-chip"><i class="fas fa-search"></i> SEO</div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="font-size: 1.1rem; margin-bottom: 10px;">Connect & Collaborate</h3>
            <p style="font-size: 0.8rem; opacity: 0.7; margin-bottom: 15px;">One click to copy official contact details.</p>
            <button class="copy-btn" onclick="copyNum()">
                <i class="fas fa-id-badge"></i> <span id="btn-txt">Copy Phone Number</span>
            </button>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="font-size: 1.1rem; margin-bottom: 10px;">Why Choose Me?</h3>
            <p style="font-size: 0.85rem; line-height: 1.7; opacity: 0.8;">
                Main "Prime Solutions" ke zariye aapke vision ko reality mein badalta hoon. Har design modern, tez, aur user-friendly hota hai.
            </p>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | THE FUTURE IS HERE</footer>
    </div>

    <audio id="bg-audio" loop>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    </audio>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });

        function copyNum() {
            const myNum = "+923000000000"; // Update with real number
            navigator.clipboard.writeText(myNum);
            const btn = document.getElementById('btn-txt');
            btn.innerText = "Number Copied!";
            setTimeout(() => { btn.innerText = "Copy Phone Number"; }, 2000);
        }

        let isPlaying = false;
        function toggleMusic() {
            const audio = document.getElementById('bg-audio');
            if (isPlaying) {
                audio.pause();
                isPlaying = false;
            } else {
                audio.play();
                isPlaying = true;
            }
        }
    </script>
</body>
</html>
