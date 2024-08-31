<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>4 Meses Juntos - Generador de Cartas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: #e0f2f1; /* Fondo verde claro */
            margin: 0;
        }

        .container {
            background: #ffffff;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            width: 100%;
            max-width: 600px;
            text-align: center;
        }

        h1 {
            color: #00796b; /* Verde oscuro */
            margin-bottom: 10px;
        }

        h2 {
            color: #004d40; /* Verde más oscuro */
            margin-bottom: 20px;
            font-size: 1.2em;
        }

        button {
            background: linear-gradient(45deg, #004d40, #00796b); /* Verde oscuro a verde más claro */
            color: #ffffff;
            border: none;
            padding: 12px;
            border-radius: 8px;
            cursor: pointer;
            width: 100%;
            font-size: 1.1em;
            transition: background 0.3s ease;
        }

        button:hover {
            background: linear-gradient(45deg, #00796b, #004d40); /* Inversión de los colores al pasar el ratón */
            transform: scale(1.05);
        }

        .output {
            margin-top: 20px;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 10px;
            background: #f1f8e9; /* Fondo verde pálido */
            white-space: pre-wrap;
            text-align: left;
            font-size: 1.1em;
            line-height: 1.6;
            color: #004d40; /* Texto verde oscuro */
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>4 Meses Juntos</h1>
        <h2>¡Generador de Cartas de Amor para Nico!</h2>
        <button onclick="generateLetter()">Generar Carta</button>
        <div class="output" id="letterOutput"></div>
    </div>

    <script>
        function generateLetter() {
            const letters = [
                `Querido Nico,

                💚 Hoy celebramos 4 meses juntos, y cada día a tu lado ha sido un regalo invaluable. Tu amor y apoyo han hecho que estos meses sean maravillosos.

                No hay palabras suficientes para expresar cuánto significas para mí. Desde nuestro primer encuentro hasta ahora, cada momento contigo ha sido especial.

                Gracias por ser mi roca y mi alegría. Estoy ansiosa por seguir construyendo recuerdos hermosos contigo.

                Con todo mi cariño,
                [Tu Nombre] 💙`,

                `Amor mío Nico,

                🌿 ¡Feliz 4 meses! Estos meses han sido un viaje increíble lleno de amor y felicidad. Tu presencia en mi vida ha traído una luz especial.

                Cada día contigo es una nueva aventura y estoy agradecida por cada momento compartido. No puedo esperar a ver qué nos depara el futuro juntos.

                Con todo mi amor,
                [Tu Nombre] 💚`,

                `Querido Nico,

                🌈 ¡4 meses juntos y mi amor por ti sigue creciendo! Cada instante contigo es un tesoro, y estos meses han sido los más felices de mi vida.

                Eres mi compañero/a perfecto/a y cada día a tu lado es un regalo. Gracias por estar siempre a mi lado y hacer que cada momento sea especial.

                Con amor eterno,
                [Tu Nombre] 💙`,

                // Puedes seguir agregando más cartas aquí
            ];

            const randomIndex = Math.floor(Math.random() * letters.length);
            document.getElementById('letterOutput').innerText = letters[randomIndex];
        }
    </script>
</body>
</html>
