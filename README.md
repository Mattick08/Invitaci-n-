<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Vale, ¿quieres ser mi San Valentín?</title>
    <style>
        body {
            background-color: #ffebee;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
            margin: 0;
        }
        .container {
            text-align: center;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
        }
        h1 {
            color: #e91e63;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4081;
            color: white;
        }
        .no {
            background-color: #ddd;
            color: black;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Mi Vale, ¿quieres ser mi San Valentín?</h1>
        <div class="buttons">
            <button class="yes" onclick="alert('¡Sabía que dirías que sí! 💖')">Sí</button>
            <button class="no" onmouseover="moveNoButton()">No</button>
        </div>
    </div>

    <script>
        function moveNoButton() {
            let noButton = document.querySelector(".no");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            noButton.style.left = x + "px";
            noButton.style.top = y + "px";
        }
    </script>
</body>
</html>
