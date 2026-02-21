<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Mobile-Friendly Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --bg: #080a12;
            --glass: rgba(255, 255, 255, 0.05);
            --border: rgba(255, 255, 255, 0.1);
        }

        * {
            margin: 0; padding: 0; box-sizing: border-box;
            font-family: 'Outfit', sans-serif;
        }

        body {
            background-color: var(--bg);
            color: white;
            overflow-x: hidden;
            background: radial-gradient(circle at top right, #1a2a6c, transparent),
                        radial-gradient(circle at bottom left, #b21f1f, transparent);
            background-attachment: fixed;
            line-height: 1.6;
        }

        .container { 
            max-width: 1100px; 
            margin: 0 auto; 
            padding: 20px; /* Mobile par padding kam ki hai */
        }

        /* Hero Section */
        .hero {
            background: var(--glass);
            backdrop-filter: blur(15px);
            padding: 40px 20px;
            border-radius: 20px;
            border: 1px solid var(--border);
            text-align: center;
            margin-bottom: 25px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.3);
        }

        .profile-pic {
            width: 120px; height: 120px;
            border-radius: 50%;
            border: 3px solid var(--primary);
            box-shadow: 0 0 20px var(--primary);
            margin-bottom: 15px;
            object-fit: cover;
        }

        h1 { 
            font-size: clamp(2rem, 8vw, 3.5rem); /* Ye text ko mobile par chota rakhta hai */
            background: linear-gradient(to right, #00f2fe, #4facfe); 
            -webkit-background-clip: text; 
            -webkit-text-fill-color: transparent; 
        }
        
        /* Responsive Grid */
        .grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(100%, 1fr)); /* Mobile par 1 column */
            gap: 20px; 
        }

        /* Desktop par 2 columns ho jayenge */
        @media (min-width: 768px) {
            .grid { grid-template-columns: repeat(2, 1fr); }
            .container { padding: 40px; }
        }
        
        .card {
            background: var(--glass);
            padding: 25px;
            border-radius: 20px;
            border: 1px solid var(--border);
            backdrop-filter: blur(10px);
        }

        /* Skill Bars */
        .skill-bar {
            background: rgba(255,255,255,0.1);
            height: 8px;
            border-radius: 5px;
            margin: 10px 0 20px 0;
            overflow: hidden;
        }

        .skill-progress {
            background: linear-gradient(to right, var(--primary), var(--secondary));
            height: 100%;
        }

        /* Projects Gallery */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr)); /* Mobile par images choti aur adjust hongi */
            gap: 12px;
        }

        .project-img {
            width: 100%;
            border-radius: 12px;
            border: 1px solid var(--border);
        }

        /* Form Controls */
        .contact-input {
            width: 100%;
            padding: 12px;
            margin: 8px 0;
            background: rgba(255,255,255,0.07);
            border: 1px solid var(--border);
            border-radius: 10px;
            color: white;
            font-size: 16px; /* Mobile par zoom rokne ke liye 16px zaroori hai */
        }

        .btn-glow {
            width: 100%; /* Mobile par full width button */
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            border: none;
            padding: 15px;
            color: white;
            font-weight: bold;
            border-radius: 15px;
            cursor: pointer;
            margin-top: 10px;
        }

        @media (min-width: 768px) {
            .btn-glow { width: auto; padding: 15px 40px; }
        }

        footer { text-align: center; margin-top: 40px; opacity: 0.5; font-size: 0.8rem; padding-bottom: 20px; }

    </style>
</head>
<body>

    <div class="container">
        <div class="hero">
            <img src="https://via.placeholder.com/150" alt="Profile" class="profile-pic">
            <h1>MERA NAAM</h1>
            <p style="color: #cbd5e1; margin-top: 10px;">Mobile & Web Enthusiast</p>
            <div style="display: flex; justify-content: center; gap: 20px; margin-top: 15px; font-size: 1.5rem;">
                <a href="#" style="color: white;"><i class="fab fa-github"></i></a>
                <a href="#" style="color: white;"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>

        <div class="grid">
            <div class="card">
                <h2><i class="fas fa-user-astronaut"></i> About Me</h2>
                <p style="font-size: 0.95rem; color: #94a3b8; margin-top: 10px;">
                    Ye website ab fully responsive hai! Aap ise mobile par check karein, ye perfect dikhegi.
                </p>
            </div>

            <div class="card">
                <h2><i class="fas fa-code"></i> Skills</h2>
                <p>Web Design (90%)</p>
                <div class="skill-bar"><div class="skill-progress" style="width: 90%;"></div></div>
                <p>Mobile Layout (95%)</p>
                <div class="skill-bar"><div class="skill-progress" style="width: 95%;"></div></div>
            </div>
        </div>

        <div class="card" style="margin-top: 20px;">
            <h2><i class="fas fa-th-large"></i> Projects</h2>
            <div class="gallery">
                <img src="https://via.placeholder.com/300x200" class="project-img" alt="Work 1">
                <img src="https://via.placeholder.com/300x200" class="project-img" alt="Work 2">
            </div>
        </div>

        <div class="card" style="margin-top: 20px;">
            <h2><i class="fas fa-envelope"></i> Contact</h2>
            <input type="text" class="contact-input" placeholder="Naam">
            <textarea class="contact-input" rows="3" placeholder="Message"></textarea>
            <button class="btn-glow">Send Message</button>
        </div>

        <footer>
            <p>© 2026 Developed by You | Optimized for Mobile</p>
        </footer>
    </div>

</body>
</html>
