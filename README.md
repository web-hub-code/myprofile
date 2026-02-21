<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Digital Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --accent: #f093fb;
            --bg: #05070a;
            --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(255, 255, 255, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }

        body {
            background-color: var(--bg);
            color: white;
            overflow-x: hidden;
            background: radial-gradient(circle at 20% 30%, #1e2a6c 0%, transparent 40%),
                        radial-gradient(circle at 80% 70%, #b21f1f 0%, transparent 40%);
            background-attachment: fixed;
        }

        .container { max-width: 900px; margin: 0 auto; padding: 20px; }

        /* Stylish Hero Section */
        .hero {
            background: var(--glass);
            backdrop-filter: blur(20px);
            padding: 50px 20px;
            border-radius: 30px;
            border: 1px solid var(--border);
            text-align: center;
            margin-top: 30px;
            margin-bottom: 30px;
            box-shadow: 0 25px 50px rgba(0,0,0,0.5);
        }

        .profile-container { position: relative; width: 160px; height: 160px; margin: 0 auto 20px; }

        .profile-pic {
            width: 100%; height: 100%;
            border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; /* Trendy organic shape */
            border: 4px solid var(--primary);
            object-fit: cover;
            animation: morph 8s ease-in-out infinite;
        }

        @keyframes morph {
            0% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
            50% { border-radius: 50% 50% 20% 80% / 25% 80% 20% 75%; }
            100% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
        }

        h1 { font-size: 2.8rem; margin-bottom: 5px; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Info Cards */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(100%, 1fr)); gap: 20px; }
        @media (min-width: 768px) { .grid { grid-template-columns: repeat(2, 1fr); } }

        .card {
            background: var(--glass);
            padding: 30px;
            border-radius: 20px;
            border: 1px solid var(--border);
            transition: 0.3s;
        }

        .card:hover { transform: translateY(-10px); border-color: var(--primary); background: rgba(255,255,255,0.06); }

        .skill-tag {
            display: inline-block;
            background: rgba(0, 242, 254, 0.1);
            color: var(--primary);
            padding: 5px 15px;
            border-radius: 50px;
            margin: 5px;
            font-size: 0.85rem;
            border: 1px solid rgba(0, 242, 254, 0.3);
        }

        /* Buttons & Socials */
        .social-links { margin-top: 20px; display: flex; justify-content: center; gap: 20px; }
        .social-icon { font-size: 1.5rem; color: white; transition: 0.3s; }
        .social-icon:hover { color: var(--primary); transform: scale(1.2); }

        .contact-btn {
            display: block; width: 100%; padding: 15px; margin-top: 20px;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            border: none; border-radius: 15px; color: white; font-weight: bold;
            text-transform: uppercase; cursor: pointer; transition: 0.3s;
        }
        .contact-btn:hover { letter-spacing: 2px; box-shadow: 0 0 20px var(--primary); }

        footer { text-align: center; margin-top: 50px; padding: 20px; font-size: 0.8rem; opacity: 0.4; }
    </style>
</head>
<body>

    <div class="container">
        <div class="hero">
            <div class="profile-container">
                <img src="Snapchat-2096615446.jpg" alt="My Profile" class="profile-pic">
            </div>
            <h1>Aapka Naam</h1>
            <p style="color: #94a3b8; letter-spacing: 1px;">CREATIVE DEVELOPER | UI/UX DESIGNER</p>
            
            <div class="social-links">
                <a href="#" class="social-icon"><i class="fab fa-github"></i></a>
                <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-icon"><i class="fab fa-facebook"></i></a>
            </div>
        </div>

        <div class="grid">
            <div class="card">
                <h3><i class="fas fa-bolt" style="color: var(--primary);"></i> My Expertise</h3>
                <p style="color: #94a3b8; margin: 15px 0;">Main digital experiences create karta hoon jo modern aur user-friendly hote hain.</p>
                <div class="skill-tag">Web Design</div>
                <div class="skill-tag">GitHub</div>
                <div class="skill-tag">Modern UI</div>
                <div class="skill-tag">SEO</div>
            </div>

            <div class="card">
                <h3><i class="fas fa-paper-plane" style="color: var(--accent);"></i> Quick Connect</h3>
                <input type="email" placeholder="Aapka Email" style="width: 100%; padding: 10px; margin-top: 15px; background: rgba(0,0,0,0.3); border: 1px solid var(--border); border-radius: 8px; color: white;">
                <button class="contact-btn">Message Bhein</button>
            </div>
        </div>

        <footer>
            DESIGNED BY YOU & GEMINI AI | 2026
        </footer>
    </div>

</body>
</html>
