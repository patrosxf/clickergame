<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clicker Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        #click-button {
            padding: 20px 40px;
            font-size: 24px;
        }
        #score {
            font-size: 30px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Clicker Game</h1>
    <button id="click-button">Click Me!</button>
    <div id="score">Score: 0</div>

    <script>
        let score = 0;
        const button = document.getElementById('click-button');
        const scoreDisplay = document.getElementById('score');

        button.addEventListener('click', () => {
            score++;
            scoreDisplay.innerText = `Score: ${score}`;
        });
    </script>
</body>
</html>
