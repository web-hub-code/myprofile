<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Nazim | Pro Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    
    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --bg: #030508;
            --card-bg: rgba(255, 255, 255, 0.05);
            --text: #ffffff;
            --border: rgba(255, 255, 255, 0.1);
        }

        [data-theme="light"] {
            --bg: #f0f2f5;
            --card-bg: #ffffff;
            --text: #1a1a1a;
            --border: rgba(0, 0, 0, 0.1);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: all 0.3s ease; }

        body {
            background-color: var(--bg);
            color: var(--text);
            overflow-x: hidden;
            background-attachment: fixed;
        }

        /* Theme Toggle Button */
        .theme-toggle {
            position: fixed; top: 20px; right: 20px; z-index: 1000;
            background: var(--card-bg); border: 1px solid var(--border);
            width: 45px; height: 45px; border-radius: 50%;
            display: flex; align-items: center; justify-content: center;
            cursor: pointer; box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .container { max-width: 900px; margin: 0 auto; padding: 20px; }

        /* Hero Section */
        .hero {
            background: var(--card-bg);
            backdrop-filter: blur(20px);
            padding: 60px 20px; border-radius: 40px;
            border: 1px solid var(--border); text-align: center;
            margin-top: 40px; margin-bottom: 30px;
        }

        .profile-pic {
            width: 150px; height: 150px; border-radius: 50%;
            border: 4px solid var(--primary); object-fit: cover;
            box-shadow: 0 0 25px var(--primary); margin-bottom: 20px;
        }

        h1 { font-size: clamp(2rem, 8vw, 3.5rem); font-weight: 800; margin-bottom: 10px; }
        .gradient-text { background: linear-gradient(45deg, var(--primary), #f093fb); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        /* Cards */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        .card {
            background: var(--card-bg); padding: 30px; border-radius: 25px;
            border: 1px solid var(--border); backdrop-filter: blur(10px);
        }

        /* Social Icons */
        .social-links { display: flex; justify-content: center; gap: 15px; margin-top: 25px; }
        .social-icon { 
            width: 45px; height: 45px; background: var(--card-bg); border: 1px solid var(--border);
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%; color: var(--text); font-size: 1.2rem; text-decoration: none;
        }
        .social-icon:hover { background: var(--primary); color: #000; transform: translateY(-5px); }

        .btn {
            width: 100%; padding: 15px; border-radius: 12px; border: none;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white; font-weight: bold; cursor: pointer; margin-top: 15px;
        }

        footer { text-align: center; padding: 40px 0; opacity: 0.6; font-size: 0.8rem; }
    </style>
</head>
<body data-theme="dark">

    <div class="theme-toggle" onclick="toggleTheme()">
        <i id="theme-icon" class="fas fa-moon"></i>
    </div>

    <div class="container">
        <div class="hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1><span class="gradient-text">Muhammad Nazim</span></h1>
            <p>Modern Solutions for Digital Problems</p>
            
            <div class="social-links">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </div>

        <div class="grid">
            <div class="card" data-aos="fade-up">
                <h2><i class="fas fa-magic"></i> My Mission</h2>
                <p style="margin-top: 10px;">Creating experiences that look great and work perfectly on all devices.</p>
            </div>
            
            <div class="card" data-aos="fade-up" data-aos-delay="100">
                <h2><i class="fas fa-envelope"></i> Let's Chat</h2>
                <button class="btn" onclick="window.location.href='mailto:contact@nazim.com'">Get In Touch</button>
            </div>
        </div>

        <footer data-aos="fade-in">
            © 2026 | Muhammad Nazim | Built with Gemini AI
        </footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        // Initialize Animations
        AOS.init({ duration: 1000, once: true });

        // Theme Toggle Logic
        function toggleTheme() {
            const body = document.body;
            const icon = document.getElementById('theme-icon');
            if (body.getAttribute('data-theme') === 'dark') {
                body.setAttribute('data-theme', 'light');
                icon.className = 'fas fa-sun';
            } else {
                body.setAttribute('data-theme', 'dark');
                icon.className = 'fas fa-moon';
            }
        }
    </script>
</body>
</html>
