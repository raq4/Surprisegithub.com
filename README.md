<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Приглашение на свадьбу</title>
    <style>
        body {
            font-family: 'Times New Roman', serif;
            color: #5a4a3a;
            text-align: center;
            margin: 0;
            padding: 0;
            line-height: 1.6;
            background-image: url('IMG_7149.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            position: relative;
        }
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(249, 243, 233, 0.85);
            z-index: -1;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 40px 20px;
            position: relative;
        }
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: normal;
        }
        .names {
            font-size: 3em;
            margin: 30px 0;
            font-weight: bold;
            letter-spacing: 2px;
        }
        .date, .place, .details {
            margin: 20px 0;
            font-size: 1.5em;
        }
        .separator {
            font-size: 2em;
            margin: 20px 0;
        }
        .footer {
            margin-top: 50px;
            font-style: italic;
        }
        .map-link {
            display: inline-block;
            margin-top: 10px;
            color: #8b6b4a;
            text-decoration: none;
            border-bottom: 1px dashed;
        }
        .map-link:hover {
            color: #5a4a3a;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Приглашаем вас на нашу свадьбу</h1>
        
        <div class="names">
            <div>Константин</div>
            <div class="separator">&</div>
            <div>Алина</div>
        </div>
        
        <div class="date">
            17 июля 2025
        </div>
        
        <div class="place">
            Ресторан "Рио" <br>
            Ессентуки, улица Фридриха Энгельса, 2Ак1
        </div>
        
        <div class="details">
            Начало в 17:00
        </div>
        
        <a href="https://yandex.ru/maps/org/rio/1087377952/" class="map-link" target="_blank">
            Посмотреть на карте
        </a>
        
        <div class="footer">
            Будем рады видеть вас в этот особенный день!
        </div>
    </div>
</body>
</html>
