<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | CEO Prime Solutions</title>
    
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

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.1); }
        .overlay-mesh { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-image: radial-gradient(var(--primary) 0.5px, transparent 0.5px); background-size: 30px 30px; opacity: 0.1; z-index: -1; }

        .container { width: 100%; max-width: 480px; margin: 0 auto; padding: 40px 15px 120px; }

        /* Premium Glass Card */
        .card { 
            background: var(--glass); backdrop-filter: blur(30px); -webkit-backdrop-filter: blur(30px);
            border: 1px solid var(--border); border-radius: 40px; 
            padding: 35px; margin-bottom: 30px; transition: 0.5s cubic-bezier(0.2, 1, 0.3, 1);
            position: relative; overflow: hidden;
        }
        .card:hover { transform: translateY(-10px); border-color: var(--primary); box-shadow: 0 20px 50px rgba(0, 242, 254, 0.15); }

        /* Hero Styling */
        .hero { text-align: center; }
        .profile-container { position: relative; width: 160px; height: 160px; margin: 0 auto 25px; }
        .profile-pic { width: 100%; height: 100%; border-radius: 50%; border: 2px solid var(--primary); padding: 8px; object-fit: cover; }
        .status-badge { position: absolute; bottom: 12px; right: 12px; width: 22px; height: 22px; background: #25d366; border: 4px solid var(--bg); border-radius: 50%; box-shadow: 0 0 15px #25d366; }

        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.6rem; letter-spacing: -1px; }

        /* Form Controls */
        .input-group { margin-bottom: 15px; }
        .form-control { width: 100%; padding: 18px; border-radius: 20px; border: 1px solid var(--border); background: rgba(255,255,255,0.02); color: white; outline: none; transition: 0.3s; }
        .form-control:focus { border-color: var(--primary); background: rgba(255,255,255,0.05); }

        /* Navigation */
        .nav-bar { position: fixed; bottom: 25px; left: 50%; transform: translateX(-50%); width: 90%; max-width: 420px; background: rgba(255, 255, 255, 0.05); backdrop-filter: blur(25px); border-radius: 50px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; }
        .nav-link { color: rgba(255,255,255,0.6); font-size: 1.5rem; transition: 0.4s; }
        .nav-link:hover { color: var(--primary); transform: scale(1.3); }

        /* Main CTA Button */
        .btn-premium { background: linear-gradient(45deg, var(--primary), var(--secondary)); color: #000; padding: 20px; width: 100%; border-radius: 25px; font-weight: 800; text-decoration: none; display: flex; align-items: center; justify-content: center; gap: 12px; border: none; font-size: 1.1rem; cursor: pointer; }

        .wa-float { position: fixed; bottom: 100px; right: 25px; background: #25d366; color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 32px; z-index: 1001; box-shadow: 0 10px 30px rgba(37, 211, 102, 0.3); animation: float 3s ease-in-out infinite; }
        @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-15px); } }
    </style>
</head>
<body>

    <div id="progress-bar"></div>
    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay-mesh"></div>

    <a href="https://wa.me/923332637235" class="wa-float" target="_blank"><i class="fab fa-whatsapp"></i></a>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <div style="background: rgba(0,242,254,0.1); color: var(--primary); display: inline-block; padding: 6px 18px; border-radius: 50px; font-size: 0.65rem; font-weight: 800; margin-bottom: 20px; letter-spacing: 1px;">VERIFIED PRIME AGENCY</div>
            <div class="profile-container">
                <img src="Screenshot_2026-04-12-10-02-54-39.png" alt="Muhammad Nazim" class="profile-pic">
                <div class="status-badge"></div>
            </div>
            <h1 class="gradient-text">Muhammad Nazim</h1>
            <p id="typewriter" style="font-size: 1.1rem; min-height: 25px; margin-top: 10px; opacity: 0.8; font-weight: 300;"></p>
        </section>

        <div class="card" data-aos="fade-up" style="display: flex; justify-content: space-around; text-align: center; padding: 25px;">
            <div><h2 style="color: var(--primary);">50+</h2><p style="font-size: 0.6rem; opacity: 0.5;">PROJECTS</p></div>
            <div><h2 style="color: var(--primary);">100%</h2><p style="font-size: 0.6rem; opacity: 0.5;">SECURITY</p></div>
            <div><h2 style="color: var(--primary);">24/7</h2><p style="font-size: 0.6rem; opacity: 0.5;">SUPPORT</p></div>
        </div>

        <div class="card" data-aos="fade-up" id="contact">
            <h3 style="margin-bottom: 25px; text-align: center; font-weight: 800;"><i class="fas fa-paper-plane" style="color: var(--primary);"></i> GET A QUOTE</h3>
            <form id="mainInquiryForm">
                <div class="input-group"><input type="text" id="name" class="form-control" placeholder="Aapka Naam" required></div>
                <div class="input-group">
                    <select id="service" class="form-control" style="background: #0a0a0a;" required>
                        <option value="" disabled selected>Service Choose Karein</option>
                        <option value="Web Development">Full Web Development</option>
                        <option value="UI/UX Design">Elite UI/UX Design</option>
                        <option value="SEO Ranking">SEO & Google Growth</option>
                        <option value="Custom Plugin">Custom Plugin / App</option>
                    </select>
                </div>
                <div class="input-group"><textarea id="details" class="form-control" placeholder="Project ki detail likhein..." rows="3" required></textarea></div>
                <button type="submit" class="btn-premium">SUBMIT INQUIRY</button>
            </form>
        </div>

        <div class="card" data-aos="fade-up" style="text-align: center; border-bottom: 5px solid var(--primary);">
            <h4 style="margin-bottom: 15px; font-size: 0.9rem; opacity: 0.7;">TRUSTED BY GLOBAL PARTNERS</h4>
            <div style="display: flex; justify-content: center; gap: 20px; font-size: 1.5rem; opacity: 0.4;">
                <i class="fab fa-stripe"></i> <i class="fab fa-google"></i> <i class="fab fa-paypal"></i> <i class="fas fa-shield-alt"></i>
            </div>
        </div>

        <footer style="text-align: center; font-size: 0.7rem; opacity: 0.3; margin-top: 20px;">
            PRIME SOLUTIONS © 2026 | ALL RIGHTS RESERVED
        </footer>
    </div>

    <nav class="nav-bar">
        <a href="#" class="nav-link"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope-open"></i></a>
    </nav>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1200, once: true });

        // Scroll Progress
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("progress-bar").style.width = scrolled + "%";
        };

        // Professional Typewriter
        const text = document.getElementById('typewriter');
        const phrases = ["Digital Architect", "Founder Prime Solutions", "Full-Stack Web Guru", "UI/UX Specialist"];
        let i = 0, j = 0, isDeleting = false;

        function type() {
            const current = phrases[i];
            if (isDeleting) {
                text.innerHTML = current.substring(0, j - 1);
                j--;
            } else {
                text.innerHTML = current.substring(0, j + 1);
                j++;
            }
            if (!isDeleting && j === current.length) { isDeleting = true; setTimeout(type, 2000); }
            else if (isDeleting && j === 0) { isDeleting = false; i = (i + 1) % phrases.length; setTimeout(type, 500); }
            else { setTimeout(type, isDeleting ? 50 : 100); }
        }
        window.onload = type;

        // Form Submission to WhatsApp
        document.getElementById('mainInquiryForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const name = document.getElementById('name').value;
            const service = document.getElementById('service').value;
            const details = document.getElementById('details').value;
            const message = `*PRIME SOLUTIONS INQUIRY*%0A%0A*Name:* ${name}%0A*Service:* ${service}%0A*Details:* ${details}%0A%0A_Sent via Official Portfolio_`;
            window.open(`https://wa.me/923332637235?text=${message}`, '_blank');
        });
    </script>
</body>
</html>
