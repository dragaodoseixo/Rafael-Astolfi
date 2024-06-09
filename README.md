<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FitPro - Exercícios Combinados</title>
    <style>
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #e0e0e0;
            color: #333;
        }
        .container {
            max-width: 1200px;
            margin: auto;
            background: #ffffff;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-bottom: 20px;
            border-bottom: 2px solid #ff4c4c;
        }
        .header img {
            max-width: 150px;
        }
        .navbar {
            display: flex;
            justify-content: space-around;
            background: #ff4c4c;
            padding: 10px 0;
            margin-bottom: 20px;
        }
        .navbar a {
            color: white;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 4px;
        }
        .navbar a:hover {
            background: #e04343;
        }
        .streak {
            text-align: center;
            margin-bottom: 20px;
        }
        .streak p {
            font-size: 18px;
            color: #ff4c4c;
        }
        h2 {
            color: #ff4c4c;
        }
        .exercise-section {
            margin-bottom: 40px;
        }
        .exercise-section h3 {
            color: #ff4c4c;
            margin-bottom: 10px;
        }
        .exercise-group {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .exercise-card {
            background: #f7f7f7;
            border: 2px solid #ff4c4c;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
            width: 48%;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            align-items: center;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .exercise-card.completed {
            background-color: #d4edda;
            border-color: #28a745;
        }
        .exercise-card img {
            max-width: 100%;
            border-radius: 8px;
        }
        .exercise-info {
            text-align: left;
            width: 100%;
            margin-bottom: 10px;
        }
        .exercise-info h4 {
            color: #333;
            margin-bottom: 5px;
        }
        .exercise-info p {
            margin: 5px 0;
        }
        .video-wrapper {
            width: 100%;
            position: relative;
            padding-bottom: 56.25%; /* 16:9 */
            height: 0;
            margin-bottom: 10px;
        }
        .video-wrapper iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 0;
        }
        .footer {
            text-align: center;
            margin-top: 20px;
            font-size: 14px;
            color: #aaa;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <img src="https://cdn.discordapp.com/attachments/783465009682055213/1249052791838867577/DALLE_2024-06-08_14.29.23_-_A_logo_for_a_fitness_brand_with_the_name_FitPro_using_a_neutral_style_relatively_simple_and_minimalistic_with_a_more_vibrant_red_and_white_color_.webp?ex=66668f4f&is=66653dcf&hm=772d968e02d2a3f47f13e6e5f527d71663a624388fd887524a976645e54f7d0c&" alt="FitPro Logo">
        </div>

        <div class="navbar">
            <a href="#support">Suporte ao Cliente</a>
            <a href="#consulting">Consultorias</a>
            <a href="#diet">Dieta</a>
        </div>

        <div class="streak">
            <p>Sua sequência de exercícios: <span id="streak-count">0</span> dias</p>
        </div>

        <h2>Exercícios Combinados</h2>

        <div class="exercise-section">
            <h3>Alterne esses exercícios</h3>
            <div class="exercise-group">
                <div class="exercise-card" onclick="toggleCompletion(this)">
                    <div class="exercise-info">
                        <h4>Afundo no Smith</h4>
                        <p>Séries: 3x8</p>
                        <p>Carga: 0kg</p>
                    </div>
                    <div class="video-wrapper">
                        <iframe src="https://www.youtube.com/embed/VuEGdXCTqk0" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="exercise-card" onclick="toggleCompletion(this)">
                    <div class="exercise-info">
                        <h4>Agachamento</h4>
                        <p>Séries: 3x10</p>
                        <p>Carga: 0kg</p>
                    </div>
                    <div class="video-wrapper">
                        <iframe src="https://www.youtube.com/embed/NvpIfoeIEd4" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        </div>

        <div class="exercise-section">
            <h3>Alterne esses exercícios</h3>
            <div class="exercise-group">
                <div class="exercise-card" onclick="toggleCompletion(this)">
                    <div class="exercise-info">
                        <h4>Cadeira Extensora Unilateral</h4>
                        <p>Séries: 3x15</p>
                        <p>Carga: 0kg</p>
                    </div>
                    <div class="video-wrapper">
                        <iframe src="https://www.youtube.com/embed/Os_byCyi6MI" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="exercise-card" onclick="toggleCompletion(this)">
                    <div class="exercise-info">
                        <h4>Desenvolvimento com Halteres</h4>
                        <p>Séries: 3x12</p>
                        <p>Carga: Ajustável</p>
                    </div>
                    <div class="video-wrapper">
                        <iframe src="https://www.youtube.com/embed/MmHTcVK-1tU" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        </div>

        <div class="footer">
            &copy; 2024 FitPro. Todos os direitos reservados.
        </div>
    </div>

    <script>
        let streakCount = 0;

        function toggleCompletion(card) {
            if (!card.classList.contains('completed')) {
                card.classList.add('completed');
                streakCount++;
            } else {
                card.classList.remove('completed');
                streakCount--;
            }
            updateStreakCount();
        }

        function updateStreakCount() {
            document.getElementById('streak-count').innerText = streakCount;
        }
    </script>
</body>
</html>
