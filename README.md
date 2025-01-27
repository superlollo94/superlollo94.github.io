<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Architetto - [Lorenzo Zecchini]</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            color: #ffffff;
            background-color: #121212;
            overflow-x: hidden;
        }

        .logo-screen {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #1a1a1a;
        }

        .logo-screen img {
            max-width: 400px;
        }

        .content {
            padding: 20px;
            text-align: center;
        }

        .content h1 {
            margin: 20px 0;
        }

        .gallery {
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            max-width: 100%;
            margin: 20px auto;
        }

        .gallery img {
            max-height: 400px;
            margin: 0 10px;
            transition: transform 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.05);
        }

        .contacts {
            margin-top: 40px;
            background-color: #1f1f1f;
            padding: 20px;
            border-radius: 8px;
        }

        .contacts a {
            color: #1a454e;
            text-decoration: none;
        }

        .contacts a:hover {
            text-decoration: underline;
        }

    </style>
</head>
<body>
    <!-- Logo Screen -->
    <div class="logo-screen" id="logo-screen">
        <img src="Logo Mio Definitivo_BW.png" alt="Logo.png" id="logo.png">
    </div>

    <!-- Content Section -->
    <div class="content">
        <h1>Architetto Lorenzo Zecchini</h1>
        <p>Benvenuto nel mio spazio online</p>

        <!-- Gallery Section -->
        <div class="gallery">
            <img src="project1.jpg" alt="Progetto 1">
            <img src="project2.jpg" alt="Progetto 2">
            <img src="project3.jpg" alt="Progetto 3">
        </div>

        <!-- Contacts Section -->
        <div class="contacts">
            <h2>Contatti</h2>
            <p>Email: <a href="mailto:zecchinilorenzo.architettura@gmail.com">zecchinilorenzo.architettura@gmail.com</a></p>
            <p>Telefono: <a href="tel:+393775753829">+39 377 575 3829</a></p>
            <p>Indirizzo: Bertinoro, FC, 47032, Italia</p>
            <p>Instagram: <a href="https://www.instagram.com/lz_architettura?igsh=MXFwNm4xZjRncDh5eg==" target="_blank">@lz_architettura</a></p>
        </div>
    </div>

    <script>
        // Smooth scroll effect when leaving the logo screen
        window.addEventListener("DOMContentLoaded", () => {
            const logoScreen = document.getElementById("logo-screen");
            if (!logoScreen) {
                console.error("Logo screen element not found.");
                return;
            }
            console.log("Logo screen element found. Initializing transition...");
            setTimeout(() => {
                console.log("Starting fade-out effect for logo screen.");
                logoScreen.style.transition = "opacity 1s";
                logoScreen.style.opacity = "0";
                setTimeout(() => {
                    console.log("Hiding logo screen after fade-out.");
                    logoScreen.style.display = "none";
                }, 1000);
            }, 2000);
        });
    </script>
</body>
</html>
