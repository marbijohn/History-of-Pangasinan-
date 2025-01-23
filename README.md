<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>History of Pangasinan</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f3efe2;
            color: #333;
        }
        header {
            background: linear-gradient(90deg, #004d00, #66cc66);
            color: white;
            padding: 20px;
            text-align: center;
            font-size: 2rem;
            font-weight: bold;
        }
        nav {
            display: flex;
            justify-content: center;
            background: #006600;
            color: white;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        nav a {
            padding: 15px 20px;
            color: white;
            text-decoration: none;
            font-size: 1rem;
            font-weight: bold;
        }
        nav a:hover {
            background: #004d00;
            transition: 0.3s;
        }
        .banner {
            width: 100%;
            height: 300px;
            background: url('https://upload.wikimedia.org/wikipedia/commons/1/10/Sunrise_in_Anda%2C_Pangasinan.jpg') no-repeat center center/cover;
            position: relative;
            animation: zoomIn 10s infinite alternate;
        }
        @keyframes zoomIn {
            0% { transform: scale(1); }
            100% { transform: scale(1.1); }
        }
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2rem;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 0 20px;
        }
        .card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin: 20px 0;
            padding: 20px;
        }
        h1, h2 {
            color: #004d00;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px;
            margin-top: 20px;
            font-size: 0.9rem;
        }
        .button {
            display: inline-block;
            background: #66cc66;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s;
        }
        .button:hover {
            background: #004d00;
        }
        .accordion {
            background: #004d00;
            color: white;
            cursor: pointer;
            padding: 15px;
            text-align: left;
            border: none;
            outline: none;
            width: 100%;
            font-size: 1rem;
            transition: background 0.3s;
        }
        .accordion:hover {
            background: #003300;
        }
        .panel {
            padding: 0 15px;
            display: none;
            background: #f9f9f9;
            overflow: hidden;
        }
    </style>
</head>
<body>
    <header>
        History of Pangasinan
    </header>
    <nav>
        <a href="#overview">Overview</a>
        <a href="#origin">Origin</a>
        <a href="#culture">Culture</a>
    </nav>
    <div class="banner">
        <div class="overlay">Welcome to Pangasinan's History</div>
    </div>
    <div class="container">
        <div class="card" id="overview">
            <h2>Overview</h2>
            <img src="https://upload.wikimedia.org/wikipedia/commons/9/9d/Lingayen_Beach.jpg" alt="Lingayen Beach, Pangasinan">
            <p>Pangasinan, located in the northwest of Luzon, Philippines, is a province known for its beautiful beaches, abundant agriculture, and rich cultural heritage. Its name is derived from the phrase "panag asinan," which means "place of salt production," highlighting its historical significance as a center for salt-making.</p>
        </div>
        <button class="accordion">Learn More About Pangasinan</button>
        <div class="panel">
            <p>Pangasinan's strategic location made it a central hub for trade and commerce in pre-colonial Philippines. Today, it continues to thrive as a region rich in natural and cultural resources.</p>
        </div>
        <div class="card" id="origin">
            <h2>Origin</h2>
            <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/Pangasinan_Capitol.jpg" alt="Pangasinan Capitol">
            <p>The history of Pangasinan dates back to pre-colonial times when it was a thriving hub for trade and commerce. Early settlers engaged in trade with neighboring Asian countries such as China and Japan. Spanish colonization in the 16th century introduced Catholicism and European cultural influences, shaping the province's historical trajectory.</p>
        </div>
        <div class="card" id="culture">
            <h2>Culture</h2>
            <img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/Bangus_Festival.jpg" alt="Bangus Festival in Pangasinan">
            <p>Pangasinan boasts a vibrant culture, reflected in its festivals, cuisine, and traditions. The province is famous for its "Bangus Festival," celebrating its status as the "Milkfish Capital of the World." Its unique dialect, Pangasinense, is widely spoken alongside Ilocano and Tagalog.</p>
        </div>
    </div>
    <footer>
        &copy; 2025 History of Pangasinan. All rights reserved.
    </footer>
    <script>
        const accordions = document.querySelectorAll(".accordion");
        accordions.forEach(acc => {
            acc.addEventListener("click", function () {
                this.classList.toggle("active");
                const panel = this.nextElementSibling;
                if (panel.style.display === "block") {
                    panel.style.display = "none";
                } else {
                    panel.style.display = "block";
                }
            });
        });
    </script>
</body>
</html>
