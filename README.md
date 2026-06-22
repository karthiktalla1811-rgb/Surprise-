<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>⚡ HAPPY 15TH BIRTHDAY TO THE CHOSEN SISTER! ⚡</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">
    <header>
        <h1>⚡ ALOHOMORA! ⚡</h1>
        <h2>Happy 15th Birthday to My Sister from Another Mother! 👑</h2>
        <p>Warning: This page contains extremely high levels of brotherly/sisterly love and pure chaos.</p>
    </header>

    <div class="section">
        <h3>🚨 EMERGENCY FLOO NETWORK INVASION!</h3>
        <p><em>*KABOOM!* Harry Potter just tumbled out of your fireplace, covered in soot, looking incredibly stressed, but holding a cake!</em></p>
        <blockquote class="hp-quote">
            "Blimey! I nearly got stuck in the plumbing! Anyway, NO TIME TO EXPLAIN. Malfoy is trying to steal your presents, Voldemort is technically gone but still being annoying, and Hagrid sat on the first cake I made. Take a deep breath, close your eyes, and blow this candle out before the Ministry tracks my illegal magic usage!"
        </blockquote>
        
        <div class="cake-container">
            <div class="candle" id="candle"><div class="flame" id="flame"></div></div>
            <div class="cake">🍰 HAPEE BIRDY 15 🍰</div>
        </div>
        <br><br>
        <button class="btn" onclick="blowCandle()">💨 Hreuffff! (Blow with maximum lung power)</button>
        <p id="cake-message"></p>
    </div>

    <div class="section">
        <h3>🎩 The Rigged Sorting Hat Game</h3>
        <p>The Sorting Hat is dynamic, sentient, and currently running on 3 hours of sleep. Choose a chaotic birthday treat to find your house:</p>
        <div id="quiz-box">
            <button class="btn" onclick="sortHouse()">A Single, Raw Potato</button>
            <button class="btn" onclick="sortHouse()">Earwax Flavoured Jellybeans</button>
            <button class="btn" onclick="sortHouse()">A Cake Made Entirely of Solid Gold</button>
            <button class="btn" onclick="sortHouse()">Spaghetti with Butterbeer Sauce</button>
        </div>
        <h4 id="sorting-result"></h4>
    </div>

    <div class="section">
        <h3>✉️ A Totally Legal, Non-Exploding Letter</h3>
        <p>Click the suspicious vibrating wax seal to open a message from my heart to yours.</p>
        
        <div class="envelope-wrapper" id="envelope" onclick="openLetter()">
            <div class="seal">✉</div>
        </div>

        <div class="letter-content" id="letter">
            <h3 class="letter-title">Dearest Sister, My Absolute Favorite Human ❤️</h3>
            <p><strong>HAPPY 15TH BIRTHDAY!</strong> 🎉</p>
            <p>Can you believe you've survived 15 whole years on this planet? Especially with me around? Honestly, it's a miracle worthy of Order of the Merlin, First Class.</p>
            <p>Even though we don’t share the same DNA, the universe knew exactly what it was doing when it made us siblings. You aren't just my "sister from another mother"—you are my chosen family, my partner-in-crime, and the person I can be 100% weird around without any judgment.</p>
            <p>Thank you for laughing at my terrible jokes, for being the brightest and most genuinely wonderful person I know, and for simply existing. I am so incredibly proud of the amazing person you are growing into. Never lose your spark, your kindness, or your absolute silliness.</p>
            <p>May your 15th year be filled with zero homework, endless snacks, and magical moments!</p>
            <p class="letter-signature">I love you to Hogwarts and back, always. ✨<br>Your Brother/Sister-in-Mischief</p>
        </div>
    </div>
</div>

<script src="script.js"></script>
</body>
</html>
@import url('https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@700&family=Metamorphous&family=Pinyon+Script&display=swap');

body {
    background-color: #1a120b;
    color: #e7cca7;
    font-family: 'Metamorphous', serif;
    text-align: center;
    margin: 0;
    padding: 20px;
    background-image: radial-gradient(rgba(0,0,0,0.3) 0%, rgba(0,0,0,0.9) 100%), url('https://www.transparenttextures.com/patterns/dark-matter.png');
}

h1, h2 {
    font-family: 'Cinzel Decorative', serif;
    color: #d4af37;
    text-shadow: 0px 0px 10px rgba(212, 175, 55, 0.5);
}

.container {
    max-width: 800px;
    margin: 0 auto;
    background: rgba(30, 22, 14, 0.9);
    padding: 30px;
    border: 4px dashed #740001;
    border-radius: 25px;
    box-shadow: 0 0 30px rgba(212, 175, 55, 0.3);
}

.btn {
    background-color: #740001;
    color: #e7cca7;
    border: 2px solid #d4af37;
    padding: 12px 24px;
    font-size: 1rem;
    cursor: pointer;
    border-radius: 50px;
    margin: 10px;
    font-family: 'Metamorphous', serif;
    transition: all 0.2s ease-in-out;
}

.btn:hover {
    background-color: #d4af37;
    color: #740001;
    transform: scale(1.1) rotate(-2deg);
    box-shadow: 0 0 15px #d4af37;
}

.section {
    margin: 40px 0;
    padding: 20px;
    border: 2px double #3a2512;
    background: rgba(0,0,0,0.2);
    border-radius: 15px;
}

.hp-quote {
    color: #d4af37;
    font-style: italic;
    background: rgba(255,255,255,0.05);
    padding: 15px;
    border-radius: 10px;
}

/* Cake Section */
.cake-container {
    position: relative;
    display: inline-block;
    margin-top: 20px;
}

.candle {
    width: 15px;
    height: 50px;
    background: linear-gradient(to right, #ff94c2, #740001);
    margin: 0 auto;
    position: relative;
    border-radius: 3px;
}

.flame {
    width: 20px;
    height: 30px;
    background: #ffcc00;
    border-radius: 50% 50% 20% 20%;
    position: absolute;
    top: -28px;
    left: -3px;
    box-shadow: 0 0 20px #ff9900;
    animation: wildFlicker 0.05s ease-in-out infinite alternate;
}

@keyframes wildFlicker {
    0% { transform: scale(1) skewX(-5deg); background: #ffcc00; }
    100% { transform: scale(1.3) skewX(5deg); background: #ff3300; }
}

.cake {
    width: 200px;
    height: 90px;
    background: #ff94c2;
    border-radius: 15px 15px 0 0;
    border: 5px solid #4a2c11;
    margin-top: 5px;
    line-height: 90px;
    font-weight: bold;
    font-size: 1.2rem;
    color: #740001;
    text-shadow: 1px 1px #fff;
}

#cake-message {
    display: none;
    color: #ff94c2;
    font-weight: bold;
    font-size: 1.2rem;
    margin-top: 15px;
}

#sorting-result {
    color: #d4af37;
    margin-top: 20px;
    font-size: 1.3rem;
}

/* Envelope Section */
.envelope-wrapper {
    margin: 40px auto;
    width: 220px;
    height: 140px;
    background: #e2d4b7;
    position: relative;
    border-radius: 5px;
    cursor: pointer;
    box-shadow: 0 10px 20px rgba(0,0,0,0.5);
    transition: transform 0.3s;
    border: 2px solid #b5a478;
}

.envelope-wrapper:hover {
    transform: scale(1.1) rotate(5deg);
}

.seal {
    width: 60px;
    height: 60px;
    background: #740001;
    border-radius: 50%;
    position: absolute;
    top: 40px;
    left: 80px;
    border: 3px dashed #d4af37;
    color: #d4af37;
    font-weight: bold;
    line-height: 60px;
    font-size: 1.8rem;
    animation: pulse 1.5s infinite;
}

@keyframes pulse {
    0 { transform: scale(1); }
    50% { transform: scale(1.05); }
    100% { transform: scale(1); }
}

.letter-content {
    display: none;
    background: #fdfaf2;
    color: #2b1d0c;
    padding: 35px;
    border-radius: 10px;
    font-family: 'Metamorphous', serif;
    font-size: 1.1rem;
    line-height: 1.8;
    border: 3px double #740001;
    box-shadow: inset 0 0 30px rgba(0,0,0,0.15);
    text-align: left;
}

.letter-title {
    text-align: center;
    color: #740001;
    margin-top: 0;
}

.letter-signature {
    text-align: right;
    font-weight: bold;
    color: #740001;
}
function blowCandle() {
    const flame = document.getElementById('flame');
    const msg = document.getElementById('cake-message');
    flame.style.display = 'none';
    msg.style.display = 'block';
    msg.innerHTML = "🎉 <em>*POP! FIZZ! BANG!*</em> 🎉<br>You blew it so hard the candle turned into a flock of rubber ducks! Harry yells, 'Brilliant!' and disappears into thin air. Your 15th year wishes are officially locked in!";
}

function sortHouse() {
    const result = document.getElementById('sorting-result');
    result.innerHTML = `🎩 <em>The Sorting Hat screams immediately:</em><br>"GRYFFINDOR! Obviously! Don't look at me like that, I didn't even need to touch your head. You're brave, fiercely loyal, crazy protective of the people you love, and honestly, a total powerhouse. 10,000 points to Gryffindor because it's your birthday!"`;
}

function openLetter() {
    const envelope = document.getElementById('envelope');
    const letter = document.getElementById('letter');
    envelope.style.display = 'none';
    letter.style.display = 'block';
}
