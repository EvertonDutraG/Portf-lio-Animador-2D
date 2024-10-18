<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio de Animador 2D</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 10px 0;
            text-align: center;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
        }

        nav a {
            padding: 14px 20px;
            text-decoration: none;
            color: white;
            text-transform: uppercase;
            font-weight: bold;
        }

        nav a:hover {
            background-color: #555;
        }

        section {
            padding: 20px;
            display: none;
        }

        section.active {
            display: block;
        }

        .portfolio-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .portfolio-item {
            background-color: white;
            padding: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: calc(33.333% - 20px);
        }

        .portfolio-item img, .portfolio-item video {
            width: 100%;
            height: auto;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Portfólio de Everton</h1>
    </header>

    <nav>
        <a href="#about" onclick="showSection('about')">Sobre Mim</a>
        <a href="#works" onclick="showSection('works')">Trabalhos que Realizei</a>
        <a href="#portfolio" onclick="showSection('portfolio')">Portfólio</a>
    </nav>

    <section id="about" class="active">
        <h2>Sobre Mim</h2>
        <p>Olá! Meu nome é Everton e sou animador 2D especializado em animações para games, vídeos explicativos e projetos criativos. Tenho experiência com ferramentas como Spine, After Effects e Blender.</p>
    </section>

    <section id="works">
        <h2>Trabalhos que Realizei</h2>
        <ul>
            <li>Animação para uma empresa de jogos indie (2024)</li>
            <li>Projeto de animação publicitária para redes sociais (2023)</li>
            <li>Criação de personagens e animação para vídeos educativos (2022)</li>
        </ul>
    </section>

    <section id="portfolio">
        <h2>Portfólio</h2>
        <div class="portfolio-grid">
            <div class="portfolio-item">
                <img src="seu_trabalho1.jpg" alt="Projeto 1">
                <p>Animação de Personagem - Projeto 1</p>
            </div>
            <div class="portfolio-item">
                <video controls>
                    <source src="seu_video1.mp4" type="video/mp4">
                    Seu navegador não suporta vídeos.
                </video>
                <p>Vídeo de Animação - Projeto 2</p>
            </div>
            <div class="portfolio-item">
                <img src="seu_trabalho3.jpg" alt="Projeto 3">
                <p>Ilustração e Design - Projeto 3</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Everton - Todos os direitos reservados.</p>
    </footer>

    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => section.classList.remove('active'));
            
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</body>
</html>
