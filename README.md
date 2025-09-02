<h1>DAVI DE MELLO DINIZ GOMES</h1>

[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-de-souza-bento-davi-511957305/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/lucas.sdbento/)
[![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/channels/@lucarg0)

![DAVI DE MELLO GitHub stats](https://github-readme-stats.vercel.app/api?username=DMelloD-gif&show_icons=true&theme=highcontrast)

<h2>Habilidade em:</h2>

[![My Skills](https://skillicons.dev/icons?i=python&theme=dark)](https://skillicons.dev)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/debysouza/debysouza/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/debysouza/debysouza/output/github-contribution-grid-snake.svg">
  <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/debysouza/debysouza/output/github-contribution-grid-snake.svg">
</picture>

--

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dino do Chrome - Animação</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            background-color: #f7f7f7;
        }
        .dino {
            position: absolute;
            bottom: 10px;
            left: 50px;
            width: 50px;
            height: 50px;
            background-color: #333;
            border-radius: 10px 10px 0 0;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }
        .dino:before {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 12px;
            width: 25px;
            height: 10px;
            background-color: #333;
            border-radius: 50%;
        }
        .ground {
            position: absolute;
            bottom: 0;
            width: 100%;
            height: 10px;
            background-color: #888;
        }
        @keyframes jump {
            0% { bottom: 10px; }
            50% { bottom: 100px; }
            100% { bottom: 10px; }
        }
        .jumping {
            animation: jump 1s ease-in-out infinite;
        }
    </style>
</head>
<body>
    <div class="dino"></div>
    <div class="ground"></div>

    <script>
        const dino = document.querySelector('.dino');
        let isJumping = false;

        document.addEventListener('keydown', () => {
            if (!isJumping) {
                isJumping = true;
                dino.classList.add('jumping');
                setTimeout(() => {
                    dino.classList.remove('jumping');
                    isJumping = false;
                }, 1000);
            }
        });
    </script>
</body>
</html>
