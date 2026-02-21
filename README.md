<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Official Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
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

        body {
            background-color: var(--bg);
            color: white;
            overflow-x: hidden;
            background: radial-gradient(circle at 10% 10%, #1e2a6c 0%, transparent 30%),
                        radial-gradient(circle at 90% 90%, #b21f1f 0%, transparent 30%);
            background-attachment: fixed;
            line-height: 1.6;
        }

        .container { width: 100%; max-width: 900px; margin: 0 auto; padding: 15px; }

        /* Hero Section - Mobile Optimized */
        .hero {
            background: var(--glass);
            backdrop-filter: blur(25px);
            padding: 40px 15px;
            border-radius: 25px;
            border: 1px solid var(--border);
            text-align: center;
            margin-top: 10px;
            margin-bottom: 20px;
            box-shadow: 0 15px 40px rgba(0,0,0,0.6);
        }

        .profile-container { position: relative; width: 140px; height: 140px; margin: 0 auto 20px; }

        .profile-pic {
            width: 100%; height: 100%;
            border-radius: 50%;
            border: 3px solid var(--primary);
            object-fit: cover;
            box-shadow: 0 0 25px rgba(0, 242, 254, 0.4);
        }

        h1 { 
            font-size: clamp(1.8rem, 8vw, 3rem); 
            background: linear-gradient(to right, var(--primary), var(--accent)); 
            -webkit-background-clip: text; 
            -webkit-text-fill-color: transparent; 
            font-weight: 800;
            line-height: 1.2;
        }

        /* Social Icons - Bigger for Mobile touch */
        .social-links { display: flex; justify-content: center; gap: 12px; margin-top: 25px; flex-wrap: wrap; }
        .social-icon { 
            width: 45px; height: 45px; background: var(--glass); 
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%; border: 1px solid var(--border);
            color: white; font-size: 1.2rem; transition: 0.3s; text-decoration: none;
        }
        .social-icon:active { transform: scale(0.9); background: var(--primary); color: #000; }

        /* Responsive Grid */
        .grid { display: flex; flex-direction: column; gap: 15px; }
        
        @media (min-width: 768px) {
            .grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 20px; }
            .container { padding: 30px; }
        }

        .card {
            background: var(--glass);
            padding: 25px;
            border-radius: 20px;
            border: 1px solid var(--border);
            backdrop-filter: blur(15px);
        }

        .submit-btn {
            width: 100%; padding: 14px; border-radius: 12px; border: none;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white; font-weight: bold; cursor: pointer; font-size: 1rem;
            text-transform: uppercase;
        }

        footer { text-align: center; margin: 40px 0 20px; font-size: 0.75rem; opacity: 0.5; letter-spacing: 1px; }
    </style>
</head>
<body>

    <div class="container">
        <div class="hero">
            <div class="profile-container">
                <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            </div>
            <h1>Muhammad Nazim</h1>
            <p style="color: #94a3b8; font-size: 1rem; margin-top: 8px;">Digital Creator & Web Explorer</p>
            
            <div class="social-links">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
                <a href="https://wa.me/923000000000" target="_blank" class="social-icon"><i class="fab fa-whatsapp"></i></a>
            </div>
        </div>

        <div class="grid">
            <div class="card">
                <h2 style="color: var(--primary); font-size: 1.3rem; margin-bottom: 12px;"><i class="fas fa-user"></i> About Me</h2>
                <p style="color: #cbd5e1; font-size: 0.95rem;">
                    Muhammad Nazim here. Main modern tech aur sleek designs ka deewana hoon. Ye website meri mobile-optimized digital identity hai.
                </p>
            </div>

            <div class="card">
                <h2 style="color: var(--accent); font-size: 1.3rem; margin-bottom: 12px;"><i class="fas fa-paper-plane"></i> Contact</h2>
                <button type="button" class="submit-btn" onclick="window.location.href='mailto:your-email@gmail.com'">Say Hello</button>
            </div>
        </div>

        <footer>
            © 2026 | MUHAMMAD NAZIM | FULLY RESPONSIVE
        </footer>
    </div>

</body>
</html>
