<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MELİKE</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: url('https://www.transparenttextures.com/patterns/love-heart.png'), linear-gradient(135deg, #ff7e79, #ffb199);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            overflow: hidden;
        }
        .container {
            max-width: 600px;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.2);
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
        }
        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            font-family: 'Georgia', serif;
        }
        p {
            font-size: 1.5em;
            line-height: 1.6;
            margin: 20px 0;
        }
        a {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 1.2em;
            color: #ffb199;
            background-color: white;
            border-radius: 25px;
            text-decoration: none;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: background-color 0.3s, color 0.3s;
        }
        a:hover {
            background-color: #ffb199;
            color: white;
        }
        .heart {
            position: absolute;
            color: red;
            font-size: 24px;
            animation: float 4s infinite;
        }
        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0); }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>MELİKE</h1>
        <p>
            Bu zor günleri beraber atlatacağız.  
            Seni çok seviyorum, sadece bana güven.  
            Hayatımın anlamı, evleneceğim kadın ♥️
        </p>
        <a href="#">Sonsuza Kadar Birlikte</a>
    </div>
    
    <!-- Kalp Animasyonu -->
    <div id="hearts"></div>

    <script>
        const heartContainer = document.getElementById('hearts');
        for (let i = 0; i < 15; i++) {
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 2 + 2 + 's';
            heart.style.opacity = Math.random();
            heartContainer.appendChild(heart);
        }
    </script>
</body>
</html>
