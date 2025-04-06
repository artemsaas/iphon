<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TT 18+</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            overflow: hidden;
        }

        .content {
            position: relative;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        h2 {
            font-size: 64px;
            margin-bottom: 10px;
            padding: 10px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.1);
            }
            100% {
                transform: scale(1);
            }
        }

        p {
            font-size: 48px;
            margin-bottom: 10px;
            padding: 10px;
        }

        .fingerprint {
            width: 600px;
            height: auto;
            cursor: pointer;
        }
    </style>
    <script src="assets/js/lang.js"></script>
</head>
<body>
    <div class="content">
        <h2 id="title">НАЖМИ И УДЕРЖИВАЙ!</h2>
        <p id="content">Нажми <b>«Открыть ссылку»</b></p>
        <a href="https://offers.affimelody.com/click?pid=77565&offer_id=840" target="_blank">
            <img class="fingerprint" src="assets/img/1.png" alt="Отпечаток пальца">
        </a>
    </div>
</body>
</html>
