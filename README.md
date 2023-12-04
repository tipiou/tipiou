<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .fireworks {
            display: none;
            position: absolute;
            width: 100%;
            height: 100%;
            background: url('https://i.imgur.com/6cJQIxJ.png') repeat 0 0;
            z-index: 1000;
        }
    </style>
    <title>Page d'accueil</title>
</head>
<body>
    <h1>Bienvenue sur notre page d'accueil !</h1>

    <h2>Propositions de vidéos :</h2>
    <ul>
        <li>
            <strong>Vidéo 1</strong> - Regarder la vidéo :
            <a href="https://www.youtube.com/watch?v=sIlOV6PCb-c&t=6s" target="_blank">https://www.youtube.com/watch?v=sIlOV6PCb-c&t=6s</a>
            <button class="like-btn" onclick="toggleFireworks('fireworks1')">Like</button>
            <div id="fireworks1" class="fireworks"></div>
        </li>
        <li>
            <strong>Vidéo 2</strong> - Regarder la vidéo :
            <a href="https://www.youtube.com/watch?v=oo1VdKM7lw4&t=3s" target="_blank">https://www.youtube.com/watch?v=oo1VdKM7lw4&t=3s</a>
            <button class="like-btn" onclick="toggleFireworks('fireworks2')">Like</button>
            <div id="fireworks2" class="fireworks"></div>
        </li>
    </ul>

    <script>
        function toggleFireworks(id) {
            var fireworks = document.getElementById(id);
            fireworks.style.display = 'block';
            setTimeout(function () {
                fireworks.style.display = 'none';
            }, 2000);  // La durée de l'animation de feux d'artifice en millisecondes
        }
    </script>
</body>
</html>
