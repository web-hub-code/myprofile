<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Pro Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #030508; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.25); }
        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }
        .card { background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--border); border-radius: 28px; padding: 25px; margin-bottom: 20px; }
        .hero { text-align: center; padding: 50px 20px; }
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 4px solid var(--primary); object-fit: cover; box-shadow: 0 0 30px rgba(0, 242, 254, 0.5); margin-bottom: 15px; }
        h1 { font-size: 2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        
        /* Fixed Bottom Nav with Facebook */
        .bottom-nav {
            position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%);
            width: 92%; background: rgba(0,0,0,0.85); backdrop-filter: blur(25px);
            border-radius: 35px; border: 1px solid var(--border);
            display: flex; justify-content: space-around; padding: 15px; z-index: 1000;
        }
        .nav-item { color: white; font-size: 1.2rem; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); }

        .copy-btn { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 15px; width: 100%; border-radius: 15px; font-weight: 700; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px; font-size: 1rem; }
        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="https://instagram.com/mr_nazim073" target="_blank" class="nav-item"><i class="fab fa-instagram"></i></a>
        <a href="https://wa.me/923000000000" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Muhammad Nazim</h1>
            <p style="color: var(--primary); letter-spacing: 2px; font-size: 0.8rem; margin-top: 5px; font-weight: 600;">PRIME SOLUTIONS EXPERT</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 10px;"><i class="fas fa-link"></i> Quick Connect</h3>
            <button class="copy-btn" onclick="copyNum()">
                <i class="fas fa-copy"></i> <span id="btn-txt">Copy Phone Number</span>
            </button>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 10px;">Facebook Profile</h3>
            <p style="font-size: 0.85rem; opacity: 0.8; margin-bottom: 15px;">Aap mujhe Facebook par bhi follow kar sakte hain.</p>
            <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" style="color: var(--primary); text-decoration: none; font-weight: bold;">Visit Facebook Profile →</a>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | ALL LINKS UPDATED</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });
        function copyNum() {
            const myNum = "+923000000000"; 
            navigator.clipboard.writeText(myNum);
            document.getElementById('btn-txt').innerText = "Number Copied!";
            setTimeout(() => { document.getElementById('btn-txt').innerText = "Copy Phone Number"; }, 2000);
        }
    </script>
</body>
</html>
