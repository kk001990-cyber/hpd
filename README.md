<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Princess Day! 👑</title>
    <style>
        body {
            background: #ffd8f0;
            margin: 0;
            font-family: "Comic Sans MS", cursive;
            text-align: center;
            overflow-x: hidden;
        }

        /* GOLDEN GLOWING CROWN */
        .crown {
            font-size: 4rem;
            margin-top: 25px;
            color: #ffd700;
            text-shadow:
                0 0 10px #ffea75,
                0 0 20px #ffd700,
                0 0 35px #ffef9a,
                0 0 50px #ffe45c;
            animation: crownGlow 2s infinite alternate ease-in-out;
        }

        @keyframes crownGlow {
            0% {
                text-shadow:
                    0 0 5px #ffea75,
                    0 0 10px #ffd700,
                    0 0 20px #ffe45c;
            }
            100% {
                text-shadow:
                    0 0 20px #ffea75,
                    0 0 40px #ffd700,
                    0 0 70px #ffe45c,
                    0 0 90px #fff5b3;
            }
        }

        h1 {
            color: #ff4fa1;
            font-size: 3.2rem;
            margin-top: 10px;
            text-shadow: 2px 2px white;
            animation: pop 1.5s ease-in-out infinite alternate;
        }

        @keyframes pop {
            0% { transform: scale(1); }
            100% { transform: scale(1.07); }
        }

        .note {
            background: white;
            display: inline-block;
            padding: 20px 30px;
            margin-top: 20px;
            border-radius: 20px;
            box-shadow: 0 4px 10px rgba(255, 0, 128, 0.3);
            color: #ff2b88;
            max-width: 500px;
            font-size: 1.3rem;
            line-height: 1.5;
        }

        .sparkle {
            position: absolute;
            width: 10px;
            height: 10px;
            background: gold;
            border-radius: 50%;
            animation: sparkle 3s linear infinite;
            opacity: 0.7;
        }

        @keyframes sparkle {
            0% { transform: translateY(0) scale(1); opacity: 1; }
            100% { transform: translateY(800px) scale(0.5); opacity: 0; }
        }
    </style>
</head>
<body>

    <!-- Background Music -->
    <audio autoplay loop>
        <source src="music.mp3" type="audio/mpeg">
        Your browser does not support audio.
    </audio>

    <!-- GOLDEN GLOWING CROWN -->
    <div class="crown">👑</div>

    <h1>
        💖 Happy Princess Day! 👑
    </h1>

    <div class="note">
        ✨💗 <b>Dear Princess,</b><br><br>
        Today is a day made especially for you — full of sparkles, sweetness, and magic.  
        May your smile shine brighter than the stars and your heart glow like the sun.  
        You are cherished, adored, and truly enchanting. 👑🌸💞  
        <br><br>
        <b>Happy Princess Day!</b> 🌟💐
    </div>

    <script>
        // Falling sparkles
        for (let i = 0; i < 40; i++) {
            let s = document.createElement("div");
            s.className = "sparkle";
            s.style.left = Math.random() * window.innerWidth + "px";
            s.style.animationDelay = Math.random() * 3 + "s";
            document.body.appendChild(s);
        }
    </script>

</body>
</html>
