<html lang="ur" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>کمائی کے پلانز</title>
    <style>
        body {
            font-family: 'Noto Nastaliq Urdu', Tahoma, Geneva, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
            scroll-behavior: smooth;
        }

        header {
            background: linear-gradient(135deg, #4facfe, #00f2fe);
            color: white;
            text-align: center;
            padding: 80px 20px;
        }
        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }
        header p {
            font-size: 1.3em;
        }

        nav {
            background-color: #007acc;
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 12px 20px;
            font-weight: bold;
            border-radius: 5px;
            transition: background 0.3s;
        }
        nav a:hover {
            background-color: #005fa3;
        }

        section {
            padding: 60px 20px;
            max-width: 1000px;
            margin: auto;
        }
        h2 {
            text-align: center;
            color: #007acc;
            margin-bottom: 40px;
        }

        .plans {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }
        .plan-card {
            background-color: white;
            border-radius: 15px;
            padding: 25px;
            text-align: center;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .plan-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.2);
        }
        .plan-card h3 {
            color: #007acc;
            margin-bottom: 15px;
        }
        .plan-card p {
            margin-bottom: 20px;
        }
        .plan-card button {
            padding: 10px 20px;
            background-color: #007acc;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s;
        }
        .plan-card button:hover {
            background-color: #005fa3;
        }

        form input, form textarea {
            width: 100%;
            padding: 12px;
            margin: 8px 0 20px 0;
            border-radius: 8px;
            border: 1px solid #ccc;
        }
        form button {
            padding: 12px 25px;
            background-color: #007acc;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s;
        }
        form button:hover {
            background-color: #005fa3;
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
    <h1>کمائی کے پلانز</h1>
    <p>اپنی محنت کے مطابق بہترین پلان کا انتخاب کریں اور کمائی شروع کریں!</p>
</header>

<nav>
    <a href="#home">ہوم</a>
    <a href="#plans">پلانز</a>
    <a href="#contact">رابطہ کریں</a>
</nav>

<section id="home">
    <h2>خوش آمدید!</h2>
    <p style="text-align:center; max-width:800px; margin:auto;">
        ہم آپ کے لیے مختلف کمائی کے پلانز پیش کرتے ہیں تاکہ آپ اپنی محنت اور ٹائم کے مطابق بہترین پلان کا انتخاب کریں اور آسانی سے کمائی شروع کریں۔
    </p>
</section>

<section id="plans">
    <h2>کمائی کے پلانز</h2>
    <div class="plans">
        <div class="plan-card">
            <h3>ابتدائی پلان</h3>
            <p>روزانہ کی معمولی کمائی کے لیے، کم سرمایہ، آسان شروعات۔</p>
            <p>قیمت: 500 روپے</p>
            <button>اب شامل ہوں</button>
        </div>
        <div class="plan-card">
            <h3>معیاری پلان</h3>
            <p>روزانہ مستحکم کمائی کے لیے، درمیانہ سرمایہ، بہتر منافع۔</p>
            <p>قیمت: 1500 روپے</p>
            <button>اب شامل ہوں</button>
        </div>
        <div class="plan-card">
            <h3>پریمیم پلان</h3>
            <p>زیادہ منافع اور پروفیشنل کمائی کے لیے، اعلی سرمایہ، بہترین نتائج۔</p>
            <p>قیمت: 3000 روپے</p>
            <button>اب شامل ہوں</button>
        </div>
    </div>
</section>

<section id="contact">
    <h2>رابطہ کریں</h2>
    <form>
        <input type="text" placeholder="آپ کا نام" required>
        <input type="email" placeholder="آپ کا ای میل" required>
        <textarea rows="5" placeholder="پیغام" required></textarea>
        <button type="submit">پیغام بھیجیں</button>
    </form>
</section>

<footer>
    <p>&copy; 2026 کمائی کے پلانز۔ تمام حقوق محفوظ ہیں۔</p>
</footer>

</body>
</html>
