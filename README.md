<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Founder & Owner Prime Solutions</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Progress Bar */
        #progress-bar { position: fixed; top: 0; left: 0; width: 0%; height: 4px; background: linear-gradient(to right, var(--primary), var(--accent)); z-index: 9999; }
        
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }

        .container { width: 100%; max-width: 480px; margin: 0 auto; padding: 40px 15px 120px; }

        /* Tech Stack Floating Icons */
        .tech-stack { display: flex; justify-content: center; gap: 15px; margin-top: 20px; font-size: 1.5rem; color: var(--primary); }
        .tech-stack i { animation: bounce 2s infinite ease-in-out; }
        @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }

        /* Theme Toggle */
        .theme-toggle { position: fixed; top: 20px; right: 20px; background: var(--glass); border: 1px solid var(--border); padding: 10px; border-radius: 50%; backdrop-filter: blur(10px); z-index: 1000; cursor: pointer; color: var(--primary); }

        /* Project Cards */
        .project-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 20px; }
        .project-item { background: rgba(255,255,255,0.02); border: 1px solid var(--border); border-radius: 20px; padding: 15px; text-align: center; transition: 0.3s; }
        .project-item:hover { background: var(--glass); border-color: var(--primary); transform: scale(1.05); }

        /* Floating Back to Top */
        #backToTop { position: fixed; bottom: 100px; left: 20px; background: var(--glass); border: 1px solid var(--primary); color: var(--primary); width: 45px; height: 45px; border-radius: 50%; display: none; align-items: center; justify-content: center; z-index: 1000; cursor: pointer; transition: 0.3s; }

        .card { 
            background: var(--glass); backdrop-filter: blur(30px); -webkit-backdrop-filter: blur(30px);
            border: 1px solid var(--border); border-radius: 35px; 
            padding: 30px; margin-bottom: 25px; position: relative;
        }

        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.5rem; }

        .btn-premium { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 18px; width: 100%; border-radius: 20px; font-weight: 800; border: none; font-size: 1rem; cursor: pointer; transition: 0.3s; display: flex; align-items: center; justify-content: center; gap: 10px; }
    </style>
</head>
<body>

    <div id="progress-bar"></div>
    <div class="theme-toggle" onclick="toggleTheme()"><i class="fas fa-moon"></i></div>
    <div id="backToTop" onclick="scrollToTop()"><i class="fas fa-arrow-up"></i></div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <div class="container">
        <section class="card hero" data-aos="fade-down">
            <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Nazim" style="width: 140px; border-radius: 50%; border: 2px solid var(--primary); padding: 5px; margin-bottom: 15px;">
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p id="typewriter" style="font-size: 1.1rem; color: var(--primary); font-weight: 300;"></p>
            
            <div class="tech-stack">
                <i class="fab fa-html5" style="animation-delay: 0s"></i>
                <i class="fab fa-css3-alt" style="animation-delay: 0.2s"></i>
                <i class="fab fa-js" style="animation-delay: 0.4s"></i>
                <i class="fab fa-github" style="animation-delay: 0.6s"></i>
                <i class="fas fa-fire" style="animation-delay: 0.8s"></i>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-laptop-code"></i> Recent Masterpieces</h3>
            <div class="project-grid">
                <div class="project-item"><h5>Web-Hub</h5><p style="font-size: 0.6rem; opacity: 0.5;">Official Agency</p></div>
                <div class="project-item"><h5>Pakgold</h5><p style="font-size: 0.6rem; opacity: 0.5;">Investment Portal</p></div>
                <div class="project-item"><h5>MINTCREST</h5><p style="font-size: 0.6rem; opacity: 0.5;">Branding Kit</p></div>
                <div class="project-item"><h5>Prime Academy</h5><p style="font-size: 0.6rem; opacity: 0.5;">Super App</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-left: 5px solid var(--primary);">
            <h3>Ready for New Missions</h3>
            <p style="font-size: 0.8rem; opacity: 0.7; margin-top: 10px;">Hamari priority fast delivery aur premium quality design hai. Let's talk about your idea.</p>
            <form id="devForm" style="margin-top: 20px; display: flex; flex-direction: column; gap: 10px;">
                <input type="text" id="uname" placeholder="Aapka Naam" required style="padding: 15px; border-radius: 15px; border: 1px solid var(--border); background: rgba(255,255,255,0.02); color: white; outline: none;">
                <button type="submit" class="btn-premium">GET A QUOTE VIA WHATSAPP</button>
            </form>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.3; padding-top: 20px;">
            DESIGNED & DEVELOPED BY NAZIM | © 2026
        </footer>
    </div>

    <nav style="position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 85%; max-width: 400px; background: rgba(255,255,255,0.05); backdrop-filter: blur(20px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000;">
        <a href="#" style="color: var(--primary);"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" style="color: white; opacity: 0.5;"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" style="color: white; opacity: 0.5;"><i class="fas fa-envelope"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000 });

        // Scroll Progress
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
            
            // Show Back to Top
            if (winScroll > 300) { document.getElementById("backToTop").style.display = "flex"; }
            else { document.getElementById("backToTop").style.display = "none"; }
        };

        function scrollToTop() { window.scrollTo({top: 0, behavior: 'smooth'}); }

        // Theme Toggle (Simplified)
        function toggleTheme() {
            const body = document.body;
            if(body.style.backgroundColor === "white") {
                body.style.backgroundColor = "#010204"; body.style.color = "white";
            } else {
                body.style.backgroundColor = "white"; body.style.color = "black";
            }
        }

        // Typewriter
        const text = document.getElementById('typewriter');
        const phrases = ["Founder & Owner", "Full-Stack Developer", "Prime Solutions Lead"];
        let i = 0, j = 0, isDeleting = false;
        function type() {
            const current = phrases[i];
            text.innerHTML = isDeleting ? current.substring(0, j--) : current.substring(0, j++);
            if (!isDeleting && j > current.length) { isDeleting = true; setTimeout(type, 2000); }
            else if (isDeleting && j < 0) { isDeleting = false; i = (i + 1) % phrases.length; setTimeout(type, 500); }
            else { setTimeout(type, isDeleting ? 50 : 100); }
        }
        window.onload = type;

        // WhatsApp Form
        document.getElementById('devForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const name = document.getElementById('uname').value;
            window.open(`https://wa.me/923332637235?text=Hello Nazim, I am ${name}. I want to discuss a project.`, '_blank');
        });
    </script>
</body>
</html>
