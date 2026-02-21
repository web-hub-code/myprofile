<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Portfolio | AI Powered</title>
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
        }

        .container { max-width: 1100px; margin: 0 auto; padding: 40px 20px; }

        /* Floating Animation */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        /* Hero Section */
        .hero {
            background: var(--glass);
            backdrop-filter: blur(15px);
            padding: 60px;
            border-radius: 30px;
            border: 1px solid var(--border);
            text-align: center;
            margin-bottom: 40px;
            box-shadow: 0 20px 50px rgba(0,0,0,0.3);
            animation: float 5s ease-in-out infinite;
        }

        .profile-pic {
            width: 150px; height: 150px;
            border-radius: 50%;
            border: 4px solid var(--primary);
            box-shadow: 0 0 30px var(--primary);
            margin-bottom: 20px;
            object-fit: cover;
        }

        h1 { font-size: 3.5rem; background: linear-gradient(to right, #00f2fe, #4facfe); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        
        /* Stats/Skills Section */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        
        .card {
            background: var(--glass);
            padding: 30px;
            border-radius: 20px;
            border: 1px solid var(--border);
            transition: 0.4s;
            backdrop-filter: blur(10px);
        }

        .card:hover {
            transform: scale(1.03) translateY(-5px);
            border-color: var(--primary);
            box-shadow: 0 10px 30px rgba(0, 242, 254, 0.2);
        }

        .skill-bar {
            background: rgba(255,255,255,0.1);
            height: 10px;
            border-radius: 5px;
            margin: 15px 0;
            overflow: hidden;
        }

        .skill-progress {
            background: linear-gradient(to right, var(--primary), var(--secondary));
            height: 100%;
            border-radius: 5px;
        }

        /* Gallery/Projects */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .project-img {
            width: 100%;
            border-radius: 15px;
            cursor: pointer;
            filter: grayscale(50%);
            transition: 0.5s;
        }

        .project-img:hover { filter: grayscale(0%); transform: rotate(2deg); }

        /* Contact Section */
        .contact-input {
            width: 100%;
            padding: 15px;
            margin: 10px 0;
            background: rgba(255,255,255,0.05);
            border: 1px solid var(--border);
            border-radius: 10px;
            color: white;
            outline: none;
        }

        .btn-glow {
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            border: none;
            padding: 15px 40px;
            color: white;
            font-weight: bold;
            border-radius: 30px;
            cursor: pointer;
            box-shadow: 0 5px 20px rgba(0, 242, 254, 0.4);
            transition: 0.3s;
        }

        .btn-glow:hover { letter-spacing: 2px; box-shadow: 0 10px 40px var(--primary); }

        /* Footer */
        footer { text-align: center; margin-top: 60px; opacity: 0.6; padding-bottom: 20px; }

    </style>
</head>
<body>

    <div class="container">
        <div class="hero">
            <img src="https://via.placeholder.com/150" alt="Profile" class="profile-pic">
            <h1>MERA NAAM</h1>
            <p style="font-size: 1.2rem; margin: 15px 0; color: #cbd5e1;">Future Web Developer & Creative Innovator</p>
            <div style="display: flex; justify-content: center; gap: 20px; font-size: 1.5rem;">
                <a href="#" style="color: white;"><i class="fab fa-github"></i></a>
                <a href="#" style="color: white;"><i class="fab fa-instagram"></i></a>
                <a href="#" style="color: white;"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>

        <div class="grid">
            <div class="card">
                <h2><i class="fas fa-rocket"></i> My Mission</h2>
                <p style="color: #94a3b8; margin-top: 15px; line-height: 1.7;">
                    Main technology ke zariye mushkil masail ka hal nikalna chahta hoon. Ye website meri pehli koshish hai digital duniya mein apni jagah banane ki.
                </p>
            </div>

            <div class="card">
                <h2><i class="fas fa-bolt"></i> Power Stats</h2>
                <p>Coding Skills</p>
                <div class="skill-bar"><div class="skill-progress" style="width: 90%;"></div></div>
                <p>UI Design</p>
                <div class="skill-bar"><div class="skill-progress" style="width: 75%;"></div></div>
                <p>GitHub Management</p>
                <div class="skill-bar"><div class="skill-progress" style="width: 85%;"></div></div>
            </div>
        </div>

        <div class="card" style="margin-top: 20px;">
            <h2><i class="fas fa-images"></i> My Creative Works</h2>
            <div class="gallery">
                <img src="https://via.placeholder.com/300x200" alt="P1" class="project-img">
                <img src="https://via.placeholder.com/300x200" alt="P2" class="project-img">
                <img src="https://via.placeholder.com/300x200" alt="P3" class="project-img">
            </div>
        </div>

        <div class="card" style="margin-top: 20px; text-align: center;">
            <h2><i class="fas fa-paper-plane"></i> Let's Connect</h2>
            <p>Mujhse baat karne ke liye niche form bharein!</p>
            <input type="text" class="contact-input" placeholder="Aapka Naam">
            <input type="email" class="contact-input" placeholder="Aapka Email">
            <textarea class="contact-input" rows="4" placeholder="Aapka Message"></textarea>
            <button class="btn-glow">BHEJ DEIN</button>
        </div>

        <footer>
            <p>Built with ❤️ by You & Gemini AI | 2026</p>
        </footer>
    </div>

</body>
</html>
