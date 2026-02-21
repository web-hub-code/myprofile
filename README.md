<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Professional Profile</title>
    
    <meta name="description" content="Muhammad Nazim - Professional Web Solutions & Digital Expert">
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

        /* Background Video */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.25); }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        /* Glassmorphism Cards */
        .card { 
            background: var(--glass); 
            backdrop-filter: blur(20px); 
            border: 1px solid var(--border); 
            border-radius: 28px; 
            padding: 25px; 
            margin-bottom: 20px;
        }

        .hero { text-align: center; padding: 50px 20px; }

        .profile-pic {
            width: 130px; height: 130px; border-radius: 50%;
            border: 4px solid var(--primary); object-fit: cover;
            box-shadow: 0 0 30px rgba(0, 242, 254, 0.5); margin-bottom: 15px;
        }

        h1 { font-size: 2rem; font-weight: 800; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Service Gallery */
        .gallery-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px; margin-top: 15px; }
        .gal-item { border-radius: 18px; overflow: hidden; position: relative; height: 120px; border: 1px solid var(--border); }
        .gal-item img { width: 100%; height: 100%; object-fit: cover; transition: 0.5s; }
        .gal-item:hover img { transform: scale(1.1); }

        /* Copy Button */
        .copy-btn {
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            border: none; color: white; padding: 15px; width: 100%;
            border-radius: 15px; font-weight: 700; cursor: pointer; margin-top: 10px;
            display: flex; align-items: center; justify-content: center; gap: 10px;
            font-size: 1rem;
        }

        /* Bottom Menu */
        .bottom-nav {
            position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%);
            width: 85%; background: rgba(0,0,0,0.8);
            backdrop-filter: blur(25px); border-radius: 35px; border: 1px solid var(--border);
            display: flex; justify-content: space-around; padding: 14px; z-index: 1000;
        }
        .nav-item { color: white; font-size: 1.3rem; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); transform: scale(1.2); }

        footer { text-align: center; font-size: 0.8rem; opacity: 0.4; padding: 20px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
        <a href="https://wa.me/923000000000" class="nav-item" target="_blank"><i class="fab fa-whatsapp"></i></a>
        <a href="https://instagram.com/mr_nazim073" class="nav-item" target="_blank"><i class="fab fa-instagram"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-out">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Muhammad Nazim</h1>
            <p style="color: var(--primary); letter-spacing: 2px; font-size: 0.8rem; margin-top: 5px; font-weight: 600;">PRIME SOLUTIONS & DIGITAL EXPERT</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="font-size: 1.1rem; margin-bottom: 10px;"><i class="fas fa-th-large" style="color: var(--accent);"></i> Prime Solutions</h3>
            <div class="gallery-grid">
                <div class="gal-item"><img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=400"></div>
                <div class="gal-item"><img src="https://images.unsplash.com/photo-1550745165-9bc0b252726f?w=400"></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="font-size: 1.1rem; margin-bottom: 5px;">Get In Touch</h3>
            <p style="font-size: 0.8rem; opacity: 0.7; margin-bottom: 15px;">Official number copy karke WhatsApp par rabta karein:</p>
            <button class="copy-btn" onclick="copyNum()">
                <i class="fas fa-copy"></i> <span id="btn-txt">+92 300 0000000</span>
            </button>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="font-size: 1.1rem; margin-bottom: 10px;">About Me</h3>
            <p style="font-size: 0.85rem; line-height: 1.7; opacity: 0.9;">
                Professionalism aur Excellence mera mission hai. Main modern web tech ko use karte hue innovative solutions provide karta hoon.
            </p>
        </div>

        <footer>© 2026 | MUHAMMAD NAZIM | ALL RIGHTS RESERVED</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });

        function copyNum() {
            const myNum = "+923000000000"; // Apna asli number yahan update karein
            navigator.clipboard.writeText(myNum);
            const btn = document.getElementById('btn-txt');
            btn.innerText = "Number Copied!";
            setTimeout(() => { btn.innerText = "+92 300 0000000"; }, 2000);
        }
    </script>
</body>
</html>
