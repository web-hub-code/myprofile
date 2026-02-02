<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FBH Family Youth</title>
<style>
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        margin: 0;
        padding: 0;
        background-color: #f4f7f9;
        color: #333;
        scroll-behavior: smooth;
    }
    header {
        position: relative;
        height: 70vh;
        overflow: hidden;
    }
    /* Slider */
    .slider {
        position: absolute;
        width: 100%;
        height: 100%;
    }
    .slide {
        position: absolute;
        width: 100%;
        height: 100%;
        opacity: 0;
        transition: opacity 1s ease-in-out;
        background-size: cover;
        background-position: center;
    }
    .slide.active {
        opacity: 1;
    }
    .header-text {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        text-align: center;
        z-index: 2;
    }
    .header-text h1 {
        font-size: 3em;
        margin-bottom: 10px;
        text-shadow: 2px 2px 8px rgba(0,0,0,0.7);
    }
    .header-text p {
        font-size: 1.2em;
        text-shadow: 1px 1px 6px rgba(0,0,0,0.7);
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
        .header-text h1 {
            font-size: 2em;
        }
    }
</style>
</head>
<body>

<header>
    <div class="slider">
        <div class="slide active" style="background-image:url('https://images.pexels.com/photos/459225/pexels-photo-459225.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940');"></div>
        <div class="slide" style="background-image:url('https://images.pexels.com/photos/733232/pexels-photo-733232.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940');"></div>
        <div class="slide" style="background-image:url('https://images.pexels.com/photos/591840/pexels-photo-591840.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940');"></div>
    </div>
    <div class="header-text">
        <h1>FBH Family Youth</h1>
        <p>Celebrating Gilgit Culture & Empowering Youth</p>
    </div>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#activities">Activities</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home">
    <h2>Welcome to FBH Family Youth</h2>
    <p style="text-align:center; max-width:800px; margin:auto;">
        FBH Family Youth Group celebrates the rich culture of Gilgit and empowers young people through community events, workshops, and cultural programs. Join us to learn, share, and grow!
    </p>
</section>

<section id="about">
    <h2>About Us</h2>
    <p style="text-align:center; max-width:800px; margin:auto;">
        Established in 2024, FBH Family Youth focuses on youth development while preserving Gilgit’s cultural heritage. We organize events, cultural workshops, and community programs to unite families and youth.
    </p>
</section>

<section id="activities">
    <h2>Our Activities</h2>
    <div class="activities">
        <div class="activity-card">
            <img src="https://images.pexels.com/photos/1163086/pexels-photo-1163086.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" alt="Cultural Workshops">
            <div>
                <h3>Cultural Workshops</h3>
                <p>Learn traditional Gilgit crafts, music, and dance in fun workshops.</p>
            </div>
        </div>
        <div class="activity-card">
            <img src="https://images.pexels.com/photos/325185/pexels-photo-325185.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" alt="Community Events">
            <div>
                <h3>Community Events</h3>
                <p>Engage with local families and youth through festivals and gatherings.</p>
            </div>
        </div>
        <div class="activity-card">
            <img src="https://images.pexels.com/photos/3428426/pexels-photo-3428426.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" alt="Sports Activities">
            <div>
                <h3>Sports & Fun Activities</h3>
                <p>Connect with peers through games, competitions, and recreational activities.</p>
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
    <p>&copy; 2026 FBH Family Youth. All rights reserved.</p>
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
    sections.forEach(section => observer.observe(section));

    // Slider script
    const slides = document.querySelectorAll('.slide');
    let current = 0;
    setInterval(() => {
        slides[current].classList.remove('active');
        current = (current + 1) % slides.length;
        slides[current].classList.add('active');
    }, 4000);
</script>

</body>
</html>
