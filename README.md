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
            --bg: rgba(3, 5, 8, 0.85); /* Overlay for video */
            --card-bg: rgba(255, 255, 255, 0.05);
            --text: #ffffff;
            --border: rgba(255, 255, 255, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: 0.3s; }

        body { background-color: #000; color: var(--text); overflow-x: hidden; }

        /* Background Video Styling */
        #bg-video {
            position: fixed; right: 0; bottom: 0;
            min-width: 100%; min-height: 100%;
            z-index: -2; object-fit: cover; filter: brightness(0.4);
        }

        .video-overlay {
            position: fixed; top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle, transparent 20%, #030508 100%);
            z-index: -1;
        }

        .container { max-width: 1000px; margin: 0 auto; padding: 20px; position: relative; z-index: 1; }

        /* Glass Cards */
        .hero, .card, .project-card {
            background: var(--card-bg);
            backdrop-filter: blur(15px);
            border: 1px solid var(--border);
            border-radius: 30px;
        }

        .hero { padding: 60px 20px; text-align: center; margin-top: 40px; margin-bottom: 30px; }

        .profile-pic {
            width: 150px; height: 150px; border-radius: 50%;
            border: 4px solid var(--primary); object-fit: cover;
            box-shadow: 0 0 30px var(--primary); margin-bottom: 20px;
        }

        h1 { font-size: clamp(2.2rem, 10vw, 3.5rem); font-weight: 800; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), #f093fb); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Gallery Grid */
        .gallery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin-top: 20px; }
        .project-card { overflow: hidden; }
        .project-card img { width: 100%; height: 200px; object-fit: cover; opacity: 0.8; transition: 0.5s; }
        .project-card:hover img { opacity: 1; transform: scale(1.1); }
        .project-info { padding: 20px; }

        /* Buttons & Socials */
        .social-links { display: flex; justify-content: center; gap: 15px; margin-top: 25px; }
        .social-icon { 
            width: 50px; height: 50px; background: var(--card-bg); border: 1px solid var(--border);
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%; color: white; font-size: 1.3rem; text-decoration: none;
        }
        .social-icon:hover { background: var(--primary); color: #000; transform: translateY(-5px); }

        .email-btn {
            display: inline-block; width: 100%; padding: 18px; border-radius: 15px; border: none;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white; font-weight: bold; cursor: pointer; text-decoration: none; text-align: center;
            font-size: 1.1rem; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.3);
        }

        footer { text-align: center; padding: 60px 0 20px; opacity: 0.6; font-size: 0.9rem; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="video-overlay"></div>

    <div class="container">
        <section class="hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1>I'm <span class="gradient-text">Muhammad Nazim</span></h1>
            <p style="margin-top: 10px; letter-spacing: 1px; opacity: 0.9;">CREATIVE DEVELOPER | DIGITAL ARCHITECT</p>
            
            <div class="social-links">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </section>

        <h2 data-aos="fade-right" style="margin: 30px 0 20px 10px; border-left: 5px solid var(--primary); padding-left: 15px;">Work & Innovation</h2>
        <div class="gallery-grid">
            <div class="project-card" data-aos="fade-up">
                <img src="https://images.unsplash.com/photo-1550745165-9bc0b252726f?auto=format&fit=crop&w=600" alt="Work 1">
                <div class="project-info">
                    <h3>Future Tech</h3>
                    <p style="font-size: 0.9rem; opacity: 0.7;">Exploring new frontiers in coding.</p>
                </div>
            </div>
            <div class="project-card" data-aos="fade-up" data-aos-delay="100">
                <img src="https://images.unsplash.com/photo-1451187580459-43490279c0fa?auto=format&fit=crop&w=600" alt="Work 2">
                <div class="project-info">
                    <h3>Clean UI</h3>
                    <p style="font-size: 0.9rem; opacity: 0.7;">Designs that speak for themselves.</p>
                </div>
            </div>
        </div>

        <div style="margin-top: 40px;" data-aos="flip-up">
            <div class="card" style="padding: 40px; text-align: center;">
                <h2>Start A Conversation</h2>
                <p style="margin: 20px 0; opacity: 0.8;">If you're looking for professional web solutions, I'm just an email away.</p>
                <a href="mailto:webhub262@gmail.com" class="email-btn">Email Me: webhub262@gmail.com</a>
            </div>
        </div>

        <footer>
            © 2026 | MUHAMMAD NAZIM | POWERED BY AI TECHNOLOGY
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
    </script>
</body>
</html>
