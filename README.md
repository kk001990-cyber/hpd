<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Princess Pari 💗</title>

<style>
    body {
        font-family: Arial, sans-serif;
        background: linear-gradient(#ffd6eb, #ffe9f7);
        padding: 20px;
        margin: 0;
        text-align: center;
        animation: bgfade 6s infinite alternate;
    }

    @keyframes bgfade {
        from { background-color: #ffd6eb; }
        to   { background-color: #ffe1f4; }
    }

    .page {
        display: none;
        max-width: 700px;
        margin: auto;
        margin-top: 40px;
        padding: 25px;
        background: #ffffffcc;
        border-radius: 15px;
        box-shadow: 0 8px 20px #ffb7db;
        animation: float 4s ease-in-out infinite;
        line-height: 1.7;
    }

    @keyframes float {
        0% { transform: translateY(0px); }
        50% { transform: translateY(-8px); }
        100% { transform: translateY(0px); }
    }

    h1, h2 {
        color: #d63384;
        text-shadow: 0 0 10px #ff8ac9;
        animation: glow 2s infinite alternate;
    }

    @keyframes glow {
        from { text-shadow: 0 0 8px #ffa9d9; }
        to   { text-shadow: 0 0 18px #ff2fa7; }
    }

    .btn {
        display: block;
        margin: 15px auto;
        padding: 14px 25px;
        width: 250px;
        border: none;
        border-radius: 30px;
        background: #ff7fbd;
        color: white;
        font-size: 18px;
        cursor: pointer;
        box-shadow: 0 6px 15px #ffb5d9;
        transition: 0.3s;
    }

    .btn:hover {
        background: #ff4fa8;
        transform: scale(1.05);
    }

    .back-btn {
        margin-top: 25px;
        padding: 12px 20px;
        background: #ff7fbd;
        border: none;
        color: white;
        border-radius: 30px;
        font-size: 16px;
        cursor: pointer;
        box-shadow: 0 6px 15px #ffb5d9;
    }

    .back-btn:hover {
        background: #ff4fa8;
    }
</style>

</head>
<body>

<!-- Auto Background Music -->
<audio id="bgmusic" autoplay loop playsinline muted>
    <source src="your-music-file.mp3" type="audio/mp3">
</audio>

<!-- HOME PAGE -->
<div id="home" class="page" style="display: block;">
    <h1>💗 Welcome My Princess Pari 💗</h1>

    <button class="btn" onclick="showPage('note')">💌 Cute Note</button>
    <button class="btn" onclick="showPage('wish')">👑 Princess Day Wish</button>
    <button class="btn" onclick="showPage('proposal')">💘 Cute Proposal</button>
</div>

<!-- NOTE PAGE -->
<div id="note" class="page">
    <h2>💌 Ek Cute Si Note, Sirf Pari Ke Liye 💕</h2>
    <p>
        Hey Pari, 🌷😄<br><br>
        Pata hai? Aaj Princess Day hai…  
        agar maine message nahi bheja toh universe mujhe  
        “crush ka worst fan” award de deta. 😂👑<br><br>

        Tu itni sweet ho ki chocolate bhi retire ho jaaye. 🍫😌<br><br>
        Teri smile ka effect — mood +100, tension -100. 📶💗  
    </p>
    <button class="back-btn" onclick="showPage('home')">⬅ Back</button>
</div>

<!-- WISH PAGE -->
<div id="wish" class="page">
    <h2>👑✨ Happy Princess Day, Pari! ✨👑</h2>
    <p>
        Aaj ka din officially tum jaise logon ke liye hota hai —  
        jo bina effort ke duniya ko pretty aur bright bana dete hain. 🌸💗<br><br>

        Happy Princess Day to the sweetest,  
        funniest, accidental-heart-stealer princess — <strong>YOU</strong>! 👸💞  
    </p>
    <button class="back-btn" onclick="showPage('home')">⬅ Back</button>
</div>

<!-- PROPOSAL PAGE -->
<div id="proposal" class="page">
    <h2>💘 Cute Proposal for My Pari 😳💕</h2>
    <p>
        Dekho Pari…  
        agar tumhe theek lage,  
        toh main tumhe thoda sa zyada  
        pasand karna chahta hoon. 😄💘<br><br>

        Bas itna puch raha hoon —  
        <strong>kya main tumhari life mein  
        “thoda-extra-special” wala spot le sakta hoon?</strong> 😉💗<br><br>

        Pressure zero.  
        Feelings 100.  
        Vibe = cute. 😌💞  
    </p>
    <button class="back-btn" onclick="showPage('home')">⬅ Back</button>
</div>

<script>
    function showPage(pageId) {
        document.querySelectorAll('.page').forEach(page => {
            page.style.display = "none";
        });
        document.getElementById(pageId).style.display = "block";
    }

    // Auto-play fix for mobile:
    document.addEventListener("click", function() {
        const audio = document.getElementById("bgmusic");
        if (audio.muted) {
            audio.muted = false;
            audio.play();
        }
    });
</script>

</body>
</html>
