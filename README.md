<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Константин & Алина | 17.07.2025</title>
    <style>
        body {
            background-color: #1A1A1A;
            background-image: url('data:image/png;base64,...'); /* Зернистая текстура как на ваших картинках */
            color: #FFF;
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 40px;
            text-align: center;
        }
        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            letter-spacing: 2px;
        }
        h2 {
            font-size: 1.8rem;
            color: #D4AF37; /* Золотой акцент */
            margin: 30px 0;
        }
        .timeline {
            margin: 40px 0;
            text-align: left;
            display: inline-block;
        }
        .timeline p {
            font-size: 1.2rem;
            margin: 15px 0;
            position: relative;
            padding-left: 30px;
        }
        .timeline p:before {
            content: "";
            position: absolute;
            left: 0;
            top: 50%;
            transform: translateY(-50%);
            width: 10px;
            height: 10px;
            background: #D4AF37;
            border-radius: 50%;
        }
        .map-button {
            background: transparent;
            border: 1px solid #D4AF37;
            color: #FFF;
            padding: 12px 25px;
            margin-top: 20px;
            cursor: pointer;
            transition: all 0.3s;
        }
        .map-button:hover {
            background: #D4AF37;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Главный экран -->
        <section>
            <h1>КОНСТАНТИН & АЛИНА</h1>
            <h2>17 ИЮЛЯ 2025</h2>
            <p>Дорогие наши родные и друзья! Мы женимся!</p>
        </section>

        <!-- Тайминг -->
        <section>
            <h1>ТАЙМИНГ</h1>
            <div class="timeline">
                <p>17:00 — Сбор гостей</p>
                <p>18:00 — Бракосочетание</p>
                <p>19:00 — Банкет</p>
                <p>21:00 — Первый танец</p>
                <p>22:00 — Свадебный торт</p>
            </div>
        </section>

        <!-- Локация -->
        <section>
            <h1>ЛОКАЦИЯ</h1>
            <p>Ресторан "Рио"</p>
            <p>Ессентуки, ул. Фридриха Энгельса, 2Ак1</p>
            <button class="map-button">ПОСТРОИТЬ МАРШРУТ</button>
        </section>
    </div>
</body>
</html>
