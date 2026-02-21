<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Nazim | Elite Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    
    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --accent: #f093fb;
            --bg: rgba(3, 5, 8, 0.9);
            --card-bg: rgba(255, 255, 255, 0.05);
            --text: #ffffff;
            --border: rgba(255, 255, 255, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }

        body { background-color: #000; color: var(--text); overflow-x: hidden; }

        /* Custom Cursor */
        #cursor {
            width: 20px; height: 20px; border: 2px solid var(--primary);
            border-radius: 50%; position: fixed; pointer-events: none;
            z-index: 9999; transition: transform 0.1s ease, background 0.3s ease;
        }

        /* Video & Particles Background */
        #bg-video {
            position: fixed; top: 0; left: 0; min-width: 100%; min-height: 100%;
            z-index: -2; object-fit: cover; filter: brightness(0.3);
        }

        #particles-js {
            position: fixed; width: 100%; height: 100%; z-index: -1;
        }

        .container { max-width: 900px; margin: 0 auto; padding: 20px; position: relative; }

        /* Glass Hero Section */
        .hero {
            background: var(--card-bg); backdrop-filter: blur(20px);
            padding: 50px 20px; border-radius: 35px; border: 1px solid var(--border);
            text-align: center; margin-top: 50px; box-shadow: 0 20px 50px rgba(0,0,0,0.5);
        }

        .profile-pic {
            width: 140px; height: 140px; border-radius: 50%;
            border: 4px solid var(--primary); object-fit: cover;
            box-shadow: 0 0 30px var(--primary); margin-bottom: 20px;
        }

        h1 { font-size: clamp(2.2rem, 10vw, 3.5rem); font-weight: 800; line-height: 1.1; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Social Icons */
        .social-links { display: flex; justify-content: center; gap: 15px; margin-top: 25px; }
        .social-icon { 
            width: 50px; height: 50px; background: var(--card-bg); 
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%; border: 1px solid var(--border);
            color: white; font-size: 1.3rem; text-decoration: none; transition: 0.4s;
        }
        .social-icon:hover { background: var(--primary); color: #000; transform: scale(1.2); }

        /* Info Grid */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; margin-top: 30px; }
        .card {
            background: var(--card-bg); padding: 30px; border-radius: 25px;
            border: 1px solid var(--border); backdrop-filter: blur(10px);
        }

        .email-btn {
            display: inline-block; width: 100%; padding: 18px; border-radius: 15px; border: none;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white; font-weight: bold; text-decoration: none; text-align: center;
            font-size: 1.1rem; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.3);
        }

        footer { text-align: center; padding: 60px 0 20px; opacity: 0.5; font-size: 0.8rem; }

        /* Mobile Adjustments */
        @media (max-width: 600px) {
            * { cursor: auto; } /* Mobile par cursor hide na ho */
            #cursor { display: none; }
            .hero { padding: 40px 15px; }
        }
    </style>
</head>
<body>

    <div id="cursor"></div>
    <div id="particles-js"></div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <div class="container">
        <section class="hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>Hi, I'm <span class="gradient-text">Muhammad Nazim</span></h1>
            <p style="margin-top: 10px; font-weight: 300; letter-spacing: 2px;">DIGITAL SOLUTIONS EXPERT</p>
            
            <div class="social-links">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </section>

        <div class="grid">
            <div class="card" data-aos="fade-right">
                <h2 style="color: var(--primary); margin-bottom: 10px;"><i class="fas fa-code"></i> Tech Passion</h2>
                <p style="opacity: 0.8;">Creating seamless digital experiences using modern tools and AI-driven insights.</p>
            </div>
            <div class="card" data-aos="fade-left">
                <h2 style="color: var(--accent); margin-bottom: 10px;"><i class="fas fa-paper-plane"></i> Quick Contact</h2>
                <a href="mailto:webhub262@gmail.com" class="email-btn">webhub262@gmail.com</a>
            </div>
        </div>

        <footer>
            © 2026 | MUHAMMAD NAZIM | DESIGNED BY GEMINI AI
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Custom Cursor Logic
        const cursor = document.querySelector('#cursor');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
        });

        // Hover Effect for Cursor
        document.querySelectorAll('a, button').forEach(el => {
            el.addEventListener('mouseenter', () => {
                cursor.style.transform = 'scale(2.5)';
                cursor.style.background = 'rgba(0, 242, 254, 0.2)';
            });
            el.addEventListener('mouseleave', () => {
                cursor.style.transform = 'scale(1)';
                cursor.style.background = 'transparent';
            });
        });

        // Particles Effect
        particlesJS("particles-js", {
            "particles": {
                "number": { "value": 80 },
                "color": { "value": "#00f2fe" },
                "shape": { "type": "circle" },
                "opacity": { "value": 0.5 },
                "size": { "value": 3 },
                "move": { "enable": true, "speed": 2 }
            },
            "interactivity": {
                "events": { "onhover": { "enable": true, "mode": "repulse" } }
            }
        });
    </script>
</body>
</html>
