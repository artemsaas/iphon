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
            -webkit-animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        @-webkit-keyframes pulse {
            0% { -webkit-transform: scale(1); }
            50% { -webkit-transform: scale(1.1); }
            100% { -webkit-transform: scale(1); }
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
            opacity: 0;
            transform: scale(0.8);
            -webkit-transform: scale(0.8);
            transition: all 1s ease;
            -webkit-transition: all 1s ease;
        }

        .fingerprint.show {
            opacity: 1;
            transform: scale(1);
            -webkit-transform: scale(1);
        }
    </style>
    <script src="assets/js/lang.js"></script>
</head>
<body>
    <div class="content" id="image-container">
        <h2 id="title">НАЖМИ И УДЕРЖИВАЙ!</h2>
        <p id="content">Нажми <b>«Открыть ссылку»</b></p>
    </div>

    <script>
        const img = document.createElement("img");
        img.src = "assets/img/1.png";
        img.alt = "Отпечаток пальца";
        img.className = "fingerprint";

        const link = document.createElement("a");
        link.href = "https://example.com/offer123"; // Замени на свою ссылку
        link.target = "_blank";
        link.appendChild(img);

        const container = document.getElementById("image-container");
        container.appendChild(link);

        setTimeout(() => {
            img.classList.add("show");
        }, 200);
    </script>
</body>
</html>
