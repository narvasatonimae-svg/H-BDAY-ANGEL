# H-BDAY ANGEL
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FOR MY B-DAY BABY BOY</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Times New Roman, serif;
}

body {
    min-height: 100vh;
    overflow: hidden;
    background: linear-gradient(135deg, #d763e1, #460150);
}

/* =========================
   GENERAL
========================= */

.screen {
    display: none;
    width: 100%;
    min-height: 100vh;
    justify-content: center;
    align-items: center;
    padding: 20px;
}

.screen.active {
    display: flex;
}

/* =========================
   ENVELOPE CARD
========================= */

.envelope-card {
    width: 100%;
    max-width: 420px;
    padding: 40px 30px;
    text-align: center;
    background: rgba(255,255,255,0.96);
    border-radius: 30px;
    box-shadow: 0 20px 50px rgba(0,0,0,0.20);
    animation: appear 0.8s ease;
}

.main-confettiball {
    font-size: 80px;
    animation: heartbeat 1.2s infinite;
}

.envelope-card h1 {
    color: #a806d9;
    margin: 15px 0;
    font-size: 32px;
}

.envelope-card p {
    color: #555;
    line-height: 1.6;
    margin-bottom: 20px;
}

.envelope-card h3 {
    color: #444;
    margin-bottom: 15px;
}

.envelope-card input {
    width: 100%;
    padding: 15px;
    border-radius: 15px;
    border: 2px solid #bc0ff6;
    outline: none;
    text-align: center;
    font-size: 16px;
    margin-bottom: 15px;
}

.envelope-card input:focus {
    border-color: #840a9a;
}

button {
    border: none;
    padding: 14px 25px;
    border-radius: 30px;
    background: #66048d;
    color: rgb(34, 33, 21);
    font-size: 16px;
    cursor: pointer;
    transition: 0.3s;
}

button:hover {
    background: #d150f5;
    transform: scale(1.06);
}

#errorMessage {
    color: #d598e4;
    font-weight: bold;
    margin-top: 15px;
}

/* =========================
   FLOATING BACKGROUND SUNFLOWERS
========================= */

.background-confettiball {
    position: fixed;
    bottom: -50px;
    pointer-events: none;
    animation: backgroundFloat linear forwards;
    z-index: 0;
}

/* =========================
   ANIMATIONS
========================= */

@keyframes sunflowerFloat {
    0%, 100% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.2);
    }
}

@keyframes appear {
    from {
        opacity: 0;
        transform: translateY(30px) scale(0.95);
    }

    to {
        opacity: 1;
        transform: translateY(0) scale(1);
    }
}

@keyframes confettiballFloat {
    from {
        bottom: -60px;
        opacity: 1;
        transform: rotate(0deg);
    }

    to {
        bottom: 110%;
        opacity: 0;
        transform: rotate(360deg);
    }
}

@keyframes backgroundFloat {
    from {
        transform: translateY(0) rotate(0deg);
        opacity: 0;
    }

    20% {
        opacity: 0.8;
    }

    to {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
    }
}

@keyframes confettiFall {
    from {
        transform: translateY(-50px) rotate(0deg);
        opacity: 1;
    }

    to {
        transform: translateY(110vh) rotate(720deg);
        opacity: 0;
    }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 600px) {

    .envelope-card {
        padding: 30px 20px;
    }

    .envelope-card h1 {
        font-size: 28px;
    }

    .main-confettiball {
        font-size: 65px;
    }

    .surprise-card {
        padding: 30px 20px;
    }

    .surprise-card h1 {
        font-size: 25px;
    }

    .message {
        font-size: 15px;
    }
}

/* =========================
   SURPRISE SCREEN
========================= */

.surprise-card {
    width: 100%;
    max-width: 650px;
    max-height: 90vh;
    overflow-y: auto;
    padding: 45px 35px;
    text-align: center;
    background: rgba(255,255,255,0.96);
    border-radius: 30px;
    box-shadow: 0 20px 50px rgba(0,0,0,0.20);
    animation: appear 0.8s ease;
    position: relative;
    z-index: 2;
}

.big-gift {
    font-size: 75px;
    animation: heartbeat 1.2s infinite;
}

.surprise-card h1 {
    color: #e99bf7;
    margin: 15px 0 25px;
    font-size: 34px;
}

.message {
    color: #555;
    line-height: 1.7;
    margin: 0 auto 18px;
    font-size: 17px;
}

.love-title {
    color: #e3c8ea;
    margin-top: 25px;
}

.background-heart,
.background-emoji {
    position: fixed;
    bottom: -60px;
    pointer-events: none;
    z-index: 0;
    animation: backgroundFloat linear forwards;
}

@keyframes heartbeat {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.12); }
}

</style>
</head>

<body>

<!-- =========================================
ENVELOPE CARD SCREEN
========================================= -->

<section id="envelopeScreen" class="screen active">

    <div class="envelope-card">

        <div class="main-birthday-gift">
            🎁
        </div>

        <h1> Are you Readyyy!!! </h1>

        <p>
            I'm sorry, luv. I can onlly do like this e.
            <br>
            Simple but I didn't want to let you down.
        </p>

        <h3> Press it babyyyy </h3>

        <button onclick="showSurprise()">
            Open it Angel 🥳
        </button>

    </div>

</section>

<!-- =========================================
     SURPRISE SCREEN
========================================= -->

<section id="surpriseScreen" class="screen">

    <div class="surprise-card">

        <div class="big-birthday-cake">
            🎂
        </div>

        <h1>
            HAPPY 21st BIRTHDAY MY BELOVED BOY.🎉
        </h1>

        <p class="message">
            Oji koooo, happyy happpyyy birthday sayoooo!!
            I'm really grateful and thanking God because
            you made it. The age of 21 is a big milestone!
            Also I'm so happy that I am still the one who 
            can celebrate this day with you.
        </p>

        <p class="message">
            I know you have time to grow up and mature to be a man
            but I know you're really trying. I know my words are
            painful for you annd to make you feel worthless.
            I guess we shoudn't talk when we're angry... 
            but I'll try too.
        </p>

        <p class="message">
            Just promise me, please choose to stay, choose to 
            prioritize important things, choose to repect 
            important people to you, and choose yourself... 
        </p>

        <p class="message">
           Because that can be a reason to make you
           responsible and mature enough. I know and 
           I belive you'll become better. We'll both
           better for each other 💛💜
        </p>

        <p class="message">
            I hope we can celebrate this again together.
            More birthdays and monthsarys to come my luv. 💗
        </p>
        
        <h2 class="love-title">
            You're always my Yellow 💛 my Purple💜

            Always so proud of you and I love you my Angel😘

            Enjoy tomorrow, Happy Birthday!!
        </h2>

        <br><br>

        <span style="font-size: 35px;">
            🎊🎉
        </span>

    </div>

</section>

  
/*========================================= */
   PRESS ENTER TO OPEN                       
*/========================================= */
<script>
document
    .getElementById("envelopeScreen") 
    .addEventListener("click", function(event) {

        if (event.target.tagName !== "GIFT") {
            openSurprise();
        }

    });

/* =========================================
   SHOW SURPRISE
========================================= */

function showSurprise() {

    document
        .getElementById("envelopeScreen")
        .classList.remove("active");


    document
        .getElementById("surpriseScreen")
        .classList.add("active");


    createConfetti();

    startBackgroundHearts();

}

/* =========================================
   CONFETTI
========================================= */

function createConfetti() {

    const emojis = [
        "🎊",
        "🎉",
        "🎁",
        "🎂",
        "💝"
    ];


    for (let i = 0; i < 60; i++) {

        const confetti =
            document.createElement("div");


        confetti.textContent =
            emojis[
                Math.floor(
                    Math.random() * emojis.length
                )
            ];


        confetti.style.position =
            "fixed";


        confetti.style.left =
            Math.random() * 100 + "vw";


        confetti.style.top =
            "-50px";


        confetti.style.fontSize =
            Math.random() * 20 + 15 + "px";


        confetti.style.zIndex =
            "9999";


        confetti.style.pointerEvents =
            "none";


        confetti.style.animation =
            `confettiFall ${
                Math.random() * 3 + 2
            }s linear forwards`;


        document.body.appendChild(confetti);


        setTimeout(function() {

            confetti.remove();

        }, 6000);

    }

}

/* =========================================
   BACKGROUND FLOATING SUNFLOWERS
========================================= */

function startBackgroundHearts() {

    setInterval(function() {

        const heart =
            document.createElement("div");


        heart.classList.add(
            "background-heart"
        );


        const emojis= [
           "🎊",
           "🎉",
           "🎁",
           "🎂",
           "💝"
        ];


        heart.textContent =
            emojis[
                Math.floor(
                    Math.random() * emojis.length
                )
            ];


        heart.style.position = "fixed";
        heart.style.left =
            Math.random() * 100 + "vw";
        heart.style.bottom = "-50px";
        heart.style.fontSize =
            Math.random() * 25 + 15 + "px";
        heart.style.zIndex = "0";
        heart.style.pointerEvents = "none";
        heart.style.animation =
            `backgroundFloat ${Math.random() * 4 + 4}s linear forwards`;


        document.body.appendChild(heart);


        setTimeout(function() {

            heart.remove();

        }, 9000);


    }, 500);

}


/* =========================================
   BACKGROUND SUNFLOWERS START
========================================= */

setInterval(function() {

    const surpriseScreen =
        document.getElementById(
            "surpriseScreen"
        );

    if (surpriseScreen.classList.contains("active")) {

        const emoji =
            document.createElement("div");


        emoji.classList.add(
            "background-emoji"
        );


        emoji.textContent = "🌻";


        emoji.style.left =
            Math.random() * 100 + "vw";


        emoji.style.fontSize =
            Math.random() * 20 + 15 + "px";


        emoji.style.animationDuration =
            Math.random() * 5 + 5 + "s";


        document.body.appendChild(emoji);


        setTimeout(function() {

            emoji.remove();

        }, 10000);

    }

}, 900);

</script>

</body>
</html>
