<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Приглашение на свадьбу Анны и Ивана</title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Roboto', sans-serif;
            background: #fff7f4;
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }
        .header {
            position: relative;
            height: 100vh;
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1519741497674-4113f4c107b8') no-repeat center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
            animation: fadeIn 2s ease-in-out;
        }
        .header h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 5em;
            margin-bottom: 10px;
        }
        .header p {
            font-size: 1.8em;
            font-weight: 300;
        }
        .content {
            background: white;
            padding: 50px;
            margin: 40px 20px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
            animation: slideUp 1s ease-out;
        }
        .content h2 {
            font-family: 'Great Vibes', cursive;
            font-size: 2.5em;
            color: #b76e79;
            margin-bottom: 20px;
        }
        .content p {
            font-size: 1.2em;
            margin-bottom: 20px;
        }
        .details {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        .details div {
            background: #f9e9ec;
            padding: 20px;
            border-radius: 10px;
            transition: transform 0.3s;
        }
        .details div:hover {
            transform: translateY(-5px);
        }
        .button {
            display: inline-block;
            padding: 12px 30px;
            background: linear-gradient(45deg, #b76e79, #d8a7b1);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            font-size: 1.1em;
            margin-top: 20px;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .button:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        .countdown {
            margin: 40px 0;
            font-size: 1.5em;
            color: #b76e79;
        }
        .footer {
            padding: 20px;
            background: #b76e79;
            color: white;
            text-align: center;
            font-family: 'Great Vibes', cursive;
            font-size: 1.5em;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes slideUp {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        @media (max-width: 600px) {
            .header h1 { font-size: 3em; }
            .header p { font-size: 1.2em; }
            .content { padding: 20px; }
            .content h2 { font-size: 2em; }
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Анна & Иван</h1>
        <p>Приглашаем на нашу свадьбу</p>
    </div>
    <div class="container">
        <div class="content">
            <h2>Дорогие гости!</h2>
            <p>С радостью приглашаем вас разделить с нами самый важный день нашей жизни! Пусть этот день будет наполнен любовью, смехом и незабываемыми моментами.</p>
            <div class="details">
                <div>
                    <h3>Дата</h3>
                    <p>15 июля 2025</p>
                </div>
                <div>
                    <h3>Время</h3>
                    <p>16:00</p>
                </div>
                <div>
                    <h3>Место</h3>
                    <p>Ресторан "Золотой закат"<br>ул. Солнечная, 12, Москва</p>
                </div>
            </div>
            <p>Пожалуйста, подтвердите ваше присутствие до 1 июля 2025 года.</p>
            <a href="mailto:rsvp@example.com" class="button">Подтвердить участие</a>
            <div class="countdown" id="countdown"></div>
        </div>
    </div>
    <div class="footer">
        <p>С любовью, Анна и Иван</p>
    </div>
    <script>
        const weddingDate = new Date("Jul 15, 2025 16:00:00").getTime();
        const countdown = setInterval(() => {
            const now = new Date().getTime();
            const distance = weddingDate - now;
            if (distance < 0) {
                document.getElementById("countdown").innerHTML = "Свадьба уже состоялась!";
                clearInterval(countdown);
                return;
            }
            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            document.getElementById("countdown").innerHTML = `${days} дней ${hours} часов ${minutes} минут до свадьбы!`;
        }, 1000);
    </script>
</body>
</html>
