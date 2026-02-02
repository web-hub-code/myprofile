<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FBH Family Youth Group</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f7f9;
            color: #333;
            scroll-behavior: smooth;
        }
        header {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
            position: relative;
        }
        header h1 {
            font-size: 3em;
            margin: 0 0 10px 0;
            animation: fadeInDown 1s ease forwards;
        }
        header p {
            font-size: 1.2em;
            animation: fadeInUp 1s ease forwards;
        }

        @keyframes fadeInDown {
            0% {opacity:0; transform: translateY(-50px);}
            100% {opacity:1; transform: translateY(0);}
        }
        @keyframes fadeInUp {
            0% {opacity:0; transform: translateY(50px);}
            100% {opacity:1; transform: translateY(0);}
        }

        nav {
            background-color: #007acc;
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 15px 20px;
            font-weight: bold;
            border-radius: 5px;
            transition: background 0.3s, transform 0.2s;
        }
        nav a:hover {
            background-color: #005fa3;
            transform: scale(1.1);
        }

        section {
            padding: 80px 20px;
            max-width: 1000px;
            margin: auto;
            opacity: 0;
            transform: translateY(50px);
            transition: all 1s ease;
        }
        section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        h2 {
            color: #007acc;
            text-align: center;
            margin-bottom: 50px;
        }

        .activities {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }
        .activity-card {
            background-color: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .activity-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        .activity-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.2);
        }
        .activity-card div {
            padding: 20px;
        }

        form input, form textarea {
            width: 100%;
            padding: 12px;
            margin: 8px 0 20px 0;
            border-radius: 8px;
            border: 1px solid #ccc;
            transition: border 0.3s;
        }
        form input:focus, form textarea:focus {
            border-color: #007acc;
            outline: none;
        }
        form button {
            padding: 12px 25px;
            background-color: #007acc;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s, transform 0.2s;
        }
        form button:hover {
            background-color: #005fa3;
            transform: scale(1.05);
        }

        footer {
            background-color: #007acc;
            color: white;
            text-align: center;
            padding: 30px 20px;
            margin-top: 40px;
        }

        @media(max-width: 600px){
            nav {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Family Youth Group</h1>
        <p>Connecting youth and families for a brighter future</p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#activities">Activities</a>
        <a href="#contact">Contact</a>
    </nav>

    <section id="home">
        <h2>Welcome to Our Group</h2>
        <p style="text-align:center; max-width:800px; margin:auto;">We are a community-focused youth group aiming to empower young people and build strong family bonds. Join us for events, workshops, and fun activities!</p>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p style="text-align:center; max-width:800px; margin:auto;">Family Youth Group started in 2024 with a mission to create a safe and inspiring space for youth. We believe in teamwork, learning, and community support.</p>
    </section>

    <section id="activities">
        <h2>Our Activities</h2>
        <div class="activities">
            <div class="activity-card">
                <img src="https://images.unsplash.com/photo-1531497865140-1636d62e2034?auto=format&fit=crop&w=800&q=80" alt="Workshop">
                <div>
                    <h3>Workshops</h3>
                    <p>Skill-building workshops for leadership, creativity, and personal growth.</p>
                </div>
            </div>
            <div class="activity-card">
                <img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?auto=format&fit=crop&w=800&q=80" alt="Community Service">
                <div>
                    <h3>Community Service</h3>
                    <p>Participate in local community projects and volunteer opportunities.</p>
                </div>
            </div>
            <div class="activity-card">
                <img src="https://images.unsplash.com/photo-1554288245-9cda7f9e18b6?auto=format&fit=crop&w=800&q=80" alt="Sports & Events">
                <div>
                    <h3>Sports & Events</h3>
                    <p>Fun sports, competitions, and social events to connect with peers.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="5" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2026 Family Youth Group. All rights reserved.</p>
    </footer>

    <script>
        // Scroll animation
        const sections = document.querySelectorAll('section');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting){
                    entry.target.classList.add('visible');
                }
            });
        }, {threshold: 0.2});

        sections.forEach(section => {
            observer.observe(section);
        });
    </script>
</body>
</html>
