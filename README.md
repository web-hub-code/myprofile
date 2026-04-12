<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Muhammad Nazim | Prime Solutions Master Agency</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>

    <style>
        :root {
            --primary: #4facfe; --secondary: #00f2fe; --accent: #f093fb;
            --bg: #fdfdfd; --text: #1d1d1f; --card: rgba(255, 255, 255, 0.9); --border: rgba(0, 0, 0, 0.08);
        }
        [data-theme="dark"] {
            --bg: #010204; --text: #ffffff; --card: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; transition: 0.3s; }
        body { background-color: var(--bg); color: var(--text); overflow-x: hidden; }

        /* Premium Image Slider */
        .swiper { width: 100%; height: 250px; border-radius: 0 0 40px 40px; }
        .swiper-slide img { width: 100%; height: 100%; object-fit: cover; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 30px 15px 120px; }

        .card { 
            background: var(--card); backdrop-filter: blur(20px); border: 1px solid var(--border); 
            border-radius: 30px; padding: 25px; margin-bottom: 25px; box-shadow: 0 10px 30px rgba(0,0,0,0.03);
        }

        /* Form Styling */
        .input-group { margin-bottom: 15px; }
        .input-group label { display: block; font-size: 0.8rem; margin-bottom: 5px; font-weight: 600; }
        .input-group input, .input-group textarea, .input-group select { 
            width: 100%; padding: 12px; border-radius: 12px; border: 1px solid var(--border); 
            background: rgba(0,0,0,0.02); color: var(--text); outline: none;
        }

        /* Service Grid */
        .service-box { 
            display: flex; align-items: center; gap: 15px; padding: 15px; 
            background: rgba(79, 172, 254, 0.05); border-radius: 20px; margin-bottom: 10px; cursor: pointer;
        }
        .service-box:hover { background: var(--primary); color: white; transform: scale(1.02); }

        /* Floating Theme Switch */
        .theme-toggle { position: fixed; top: 20px; right: 20px; z-index: 5000; background: white; padding: 10px; border-radius: 50%; box-shadow: 0 5px 15px rgba(0,0,0,0.1); color: var(--primary); }

        .btn-send { 
            width: 100%; padding: 18px; border-radius: 20px; border: none; 
            background: linear-gradient(45deg, var(--primary), var(--secondary)); 
            color: white; font-weight: 800; cursor: pointer; margin-top: 10px;
        }

        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 90%; background: var(--card); backdrop-filter: blur(15px); border-radius: 40px; display: flex; justify-content: space-around; padding: 15px; border: 1px solid var(--border); z-index: 4000; }
    </style>
</head>
<body data-theme="light">

    <div class="theme-toggle" onclick="toggleTheme()"><i class="fas fa-moon"></i></div>

    <div class="swiper mySwiper">
        <div class="swiper-wrapper">
            <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=800&q=80"></div>
            <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=800&q=80"></div>
            <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1551434678-e076c223a692?auto=format&fit=crop&w=800&q=80"></div>
        </div>
        <div class="swiper-pagination"></div>
    </div>

    <div class="container">
        
        <section class="card" style="text-align: center;">
            <h1 style="font-size: 2rem; font-weight: 800; background: linear-gradient(to right, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Prime Solutions</h1>
            <p style="font-size: 0.9rem; opacity: 0.7;">Modern Digital Agency by Muhammad Nazim</p>
        </section>

        <div class="card">
            <h3><i class="fas fa-briefcase"></i> Unlimited Services</h3>
            <p style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 15px;">We build everything for your business</p>
            
            <div class="service-box">
                <i class="fas fa-shopping-cart"></i>
                <div><h4>E-Commerce Stores</h4><p style="font-size: 0.7rem;">Sell products online globally.</p></div>
            </div>
            <div class="service-box">
                <i class="fas fa-chart-pie"></i>
                <div><h4>Investment Portals</h4><p style="font-size: 0.7rem;">Manage deposits & daily profits.</p></div>
            </div>
            <div class="service-box">
                <i class="fas fa-hospital"></i>
                <div><h4>Hospital Systems</h4><p style="font-size: 0.7rem;">Patient records & appointments.</p></div>
            </div>
            <div class="service-box">
                <i class="fas fa-school"></i>
                <div><h4>School/Academy Apps</h4><p style="font-size: 0.7rem;">Fee management & results.</p></div>
            </div>
        </div>

        <div class="card">
            <h3><i class="fas fa-paper-plane"></i> Get a Free Quote</h3>
            <form id="quoteForm">
                <div class="input-group">
                    <label>Your Name</label>
                    <input type="text" id="userName" placeholder="Enter your name" required>
                </div>
                <div class="input-group">
                    <label>Project Type</label>
                    <select id="projectType">
                        <option>Business Website</option>
                        <option>Investment Site</option>
                        <option>E-commerce Store</option>
                        <option>Custom App</option>
                    </select>
                </div>
                <div class="input-group">
                    <label>Contact Via</label>
                    <select id="contactMethod">
                        <option value="whatsapp">Send to WhatsApp</option>
                        <option value="email">Send to Email</option>
                    </select>
                </div>
                <div class="input-group">
                    <label>Message</label>
                    <textarea id="userMsg" rows="3" placeholder="Tell us about your project..."></textarea>
                </div>
                <button type="button" class="btn-send" onclick="sendInquiry()">SEND INQUIRY NOW</button>
            </form>
        </div>

        <div class="card" style="border-left: 5px solid #25d366;">
            <h3><i class="fas fa-check-double" style="color: #25d366;"></i> Trusted Partnership</h3>
            <p style="font-size: 0.8rem; margin-top: 10px; opacity: 0.7;">Prime Solutions ensures 100% privacy, lifelong support, and modern UI that attracts more customers to your brand.</p>
        </div>

    </div>

    <nav class="bottom-nav">
        <a href="tel:03705519562" style="color: var(--text);"><i class="fas fa-phone"></i></a>
        <a href="https://wa.me/923332637235" style="color: #25d366; font-size: 1.5rem;"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" style="color: var(--text);"><i class="fas fa-envelope"></i></a>
    </nav>

    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script>
        var swiper = new Swiper(".mySwiper", {
            pagination: { el: ".swiper-pagination", dynamicBullets: true },
            autoplay: { delay: 3000 },
            loop: true
        });

        function toggleTheme() {
            const body = document.body;
            const current = body.getAttribute('data-theme');
            body.setAttribute('data-theme', current === 'light' ? 'dark' : 'light');
        }

        function sendInquiry() {
            const name = document.getElementById('userName').value;
            const type = document.getElementById('projectType').value;
            const method = document.getElementById('contactMethod').value;
            const msg = document.getElementById('userMsg').value;
            
            const fullMsg = `Hello Prime Solutions! My name is ${name}. I am interested in a ${type}. Details: ${msg}`;
            
            if(method === 'whatsapp') {
                window.location.href = `https://wa.me/923332637235?text=${encodeURIComponent(fullMsg)}`;
            } else {
                window.location.href = `mailto:webhub262@gmail.com?subject=New Quote Request&body=${encodeURIComponent(fullMsg)}`;
            }
        }
    </script>
</body>
</html>
