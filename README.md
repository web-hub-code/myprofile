<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Nazim | Official Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --accent: #f093fb;
            --bg: #030508;
            --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(255, 255, 255, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }

        body {
            background-color: var(--bg);
            color: white;
            overflow-x: hidden;
            background: radial-gradient(circle at 10% 10%, #1e2a6c 0%, transparent 30%),
                        radial-gradient(circle at 90% 90%, #b21f1f 0%, transparent 30%);
            background-attachment: fixed;
        }

        .container { max-width: 900px; margin: 0 auto; padding: 20px; }

        /* Hero Section */
        .hero {
            background: var(--glass);
            backdrop-filter: blur(25px);
            padding: 60px 20px;
            border-radius: 40px;
            border: 1px solid var(--border);
            text-align: center;
            margin-top: 20px;
            margin-bottom: 30px;
            box-shadow: 0 25px 60px rgba(0,0,0,0.6);
            animation: slideIn 1s ease-out;
        }

        @keyframes slideIn { from { opacity: 0; transform: scale(0.9); } to { opacity: 1; transform: scale(1); } }

        .profile-container { position: relative; width: 160px; height: 160px; margin: 0 auto 25px; }

        .profile-pic {
            width: 100%; height: 100%;
            border-radius: 50%;
            border: 4px solid var(--primary);
            object-fit: cover;
            box-shadow: 0 0 30px rgba(0, 242, 254, 0.5);
            transition: 0.5s;
        }

        .profile-pic:hover { transform: rotate(5deg) scale(1.05); }

        h1 { 
            font-size: clamp(2.2rem, 10vw, 3.5rem); 
            background: linear-gradient(to right, var(--primary), var(--accent)); 
            -webkit-background-clip: text; 
            -webkit-text-fill-color: transparent; 
            font-weight: 800;
        }

        /* Social Icons */
        .social-links { display: flex; justify-content: center; gap: 15px; margin-top: 25px; flex-wrap: wrap; }
        .social-icon { 
            width: 50px; height: 50px; background: var(--glass); 
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%; border: 1px solid var(--border);
            color: white; font-size: 1.3rem; transition: 0.4s; text-decoration: none;
        }
        .social-icon:hover { 
            background: var(--primary); color: #000; 
            transform: translateY(-8px); box-shadow: 0 15px 25px rgba(0,242,254,0.4);
        }

        /* Content Grid */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(100%, 1fr)); gap: 20px; }
        @media (min-width: 768px) { .grid { grid-template-columns: repeat(2, 1fr); } }

        .card {
            background: var(--glass);
            padding: 35px;
            border-radius: 25px;
            border: 1px solid var(--border);
            backdrop-filter: blur(15px);
            transition: 0.3s;
        }
        .card:hover { border-color: var(--primary); background: rgba(255,255,255,0.06); }

        .submit-btn {
            width: 100%; padding: 15px; border-radius: 12px; border: none;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white; font-weight: bold; cursor: pointer; transition: 0.3s;
            text-transform: uppercase; letter-spacing: 1px;
        }
        .submit-btn:hover { letter-spacing: 3px; box-shadow: 0 5px 20px var(--primary); }

        footer { text-align: center; margin: 60px 0 20px; font-size: 0.8rem; opacity: 0.5; letter-spacing: 2px; }
    </style>
</head>
<body>

    <div class="container">
        <div class="hero">
            <div class="profile-container">
                <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            </div>
            <h1>Muhammad Nazim</h1>
            <p style="color: #94a3b8; font-size: 1.1rem; margin-top: 10px; font-weight: 300;">Digital Creator | Web Explorer</p>
            
            <div class="social-links">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-icon" title="Facebook"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-icon" title="Instagram"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-icon" title="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                <a href="https://wa.me/923000000000" target="_blank" class="social-icon" title="WhatsApp"><i class="fab fa-whatsapp"></i></a>
            </div>
        </div>

        <div class="grid">
            <div class="card">
                <h2 style="color: var(--primary); margin-bottom: 15px;"><i class="fas fa-user"></i> About Me</h2>
                <p style="color: #cbd5e1; line-height: 1.8;">
                    Main Muhammad Nazim hoon. Mujhe nayi technology explore karne aur modern digital designs banane ka junoon hai. Ye website meri GitHub journey ka pehla qadam hai.
                </p>
            </div>

            <div class="card">
                <h2 style="color: var(--accent); margin-bottom: 15px;"><i class="fas fa-paper-plane"></i> Quick Contact</h2>
                <p style="color: #94a3b8; margin-bottom: 15px; font-size: 0.9rem;">Mujhse rabta karne ke liye click karein:</p>
                <button type="button" class="submit-btn" onclick="window.location.href='mailto:your-email@example.com'">Say Hello</button>
            </div>
        </div>

        <footer>
            © 2026 | MUHAMMAD NAZIM | DESIGNED WITH AI
        </footer>
    </div>

</body>
</html>
