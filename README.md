<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Official Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --accent: #f093fb;
            --bg: #030508;
            --glass: rgba(255, 255, 255, 0.05);
            --border: rgba(255, 255, 255, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        
        body { background-color: var(--bg); color: white; overflow-x: hidden; width: 100%; }

        /* Video Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.25); }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 15px 15px 100px; }

        /* Glass Cards - Responsive Fix */
        .card { 
            background: var(--glass); 
            backdrop-filter: blur(15px); 
            border: 1px solid var(--border); 
            border-radius: 25px; 
            padding: 20px; 
            margin-bottom: 20px; 
            width: 100%;
        }

        .hero { text-align: center; padding: 40px 15px; }

        .profile-pic {
            width: 120px; height: 120px; border-radius: 50%;
            border: 3px solid var(--primary); object-fit: cover;
            box-shadow: 0 0 25px var(--primary); margin-bottom: 15px;
        }

        h1 { font-size: 1.8rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Copy Number Button */
        .copy-btn {
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            border: none; color: white; padding: 12px; width: 100%;
            border-radius: 12px; font-weight: 600; cursor: pointer; margin-top: 15px;
            display: flex; align-items: center; justify-content: center; gap: 10px;
        }

        /* Bottom Nav - Perfect Mobile Fit */
        .bottom-nav {
            position: fixed; bottom: 15px; left: 50%; transform: translateX(-50%);
            width: 90%; background: rgba(0,0,0,0.8);
            backdrop-filter: blur(20px); border-radius: 30px; border: 1px solid var(--border);
            display: flex; justify-content: space-around; padding: 12px; z-index: 1000;
        }
        .nav-item { color: white; font-size: 1.1rem; text-decoration: none; }

        /* Stats Grid */
        .stats-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; text-align: center; }
        .stats-grid h2 { font-size: 1.4rem; color: var(--primary); }
        .stats-grid p { font-size: 0.7rem; opacity: 0.8; }

        footer { text-align: center; font-size: 0.75rem; opacity: 0.5; margin-top: 20px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
        <a href="https://wa.me/923000000000" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="https://instagram.com/mr_nazim073" class="nav-item"><i class="fab fa-instagram"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="fade-down">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Muhammad Nazim</h1>
            <p style="font-size: 0.9rem; margin-top: 5px; opacity: 0.8;">Creative Web Developer</p>
        </section>

        <div class="card stats-grid" data-aos="fade-up">
            <div><h2>40+</h2><p>Projects</p></div>
            <div><h2>100%</h2><p>Quality</p></div>
            <div><h2>24/7</h2><p>Support</p></div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-phone-alt" style="color: var(--primary);"></i> Contact Me</h3>
            <p style="font-size: 0.85rem; margin-top: 5px; opacity: 0.7;">Click niche button par karein number copy karne ke liye:</p>
            <button class="copy-btn" onclick="copyNumber()">
                <i class="fas fa-copy"></i> <span id="num-text">+92 300 0000000</span>
            </button>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-id-card" style="color: var(--accent);"></i> About</h3>
            <p style="font-size: 0.9rem; line-height: 1.6; margin-top: 10px;">
                Main Muhammad Nazim hoon. Professional web designs aur interactive digital experiences banana meri pehchan hai.
            </p>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | MOBILE OPTIMIZED</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });

        function copyNumber() {
            const num = "+923000000000"; // Apna asli number yahan likhein
            navigator.clipboard.writeText(num);
            document.getElementById('num-text').innerText = "Copied!";
            setTimeout(() => {
                document.getElementById('num-text').innerText = "+92 300 0000000";
            }, 2000);
        }
    </script>
</body>
</html>
