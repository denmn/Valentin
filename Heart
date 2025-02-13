<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe6e6;
            padding: 50px;
            overflow: hidden;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
        }
        h1 {
            color: #ff4d4d;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #999;
            color: white;
            position: absolute;
        }
        .heart {
            position: absolute;
            color: red;
            font-size: 24px;
            animation: float 2s linear infinite;
        }
        @keyframes float {
            0% { transform: translateY(0); opacity: 1; }
            100% { transform: translateY(-100px); opacity: 0; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Gustavo, ¿quieres ser mi San Valentín? ❤️</h1>
        <button class="yes" onclick="showHearts()">Sí</button>
        <button class="no" id="noButton">No</button>
    </div>

    <script>
        document.getElementById("noButton").addEventListener("mouseover", function() {
            let x = Math.random() * window.innerWidth - 100;
            let y = Math.random() * window.innerHeight - 50;
            this.style.left = x + "px";
            this.style.top = y + "px";
        });

        function showHearts() {
            for (let i = 0; i < 10; i++) {
                let heart = document.createElement("div");
                heart.innerHTML = "❤️";
                heart.classList.add("heart");
                document.body.appendChild(heart);
                
                let x = Math.random() * window.innerWidth;
                let y = Math.random() * window.innerHeight;
                heart.style.left = `${x}px`;
                heart.style.top = `${y}px`;
                
                setTimeout(() => {
                    heart.remove();
                }, 2000);
            }
        }
    </script>
</body>
</html>
