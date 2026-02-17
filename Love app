<!DOCTYPE html>
<html>
<head>
<title>Irritating Husband Care App</title>

<style>
body {
    font-family: Arial, sans-serif;
    background: linear-gradient(to right, #ffe6f0, #fff0f5);
    text-align: center;
    padding: 30px;
    overflow: hidden;
}

/* Floating Hearts */
.heart {
    position: fixed;
    bottom: -10px;
    color: #ff4da6;
    font-size: 20px;
    animation: floatUp 5s linear infinite;
}

@keyframes floatUp {
    0% { transform: translateY(0); opacity: 1; }
    100% { transform: translateY(-800px); opacity: 0; }
}

.card {
    background: white;
    padding: 20px;
    border-radius: 20px;
    box-shadow: 0px 5px 15px rgba(0,0,0,0.2);
    max-width: 400px;
    margin: auto;
    position: relative;
    z-index: 10;
}

button {
    background: #ff4da6;
    color: white;
    border: none;
    padding: 10px 15px;
    margin: 5px;
    border-radius: 20px;
    cursor: pointer;
}

button:hover {
    background: #e60073;
}

.hidden {
    display: none;
}
</style>
</head>

<body>

<!-- Background Music -->
<audio id="bgMusic" loop>
  <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
</audio>

<div class="card">
    <h2>⚠️ Wife On Periods Mode Activated</h2>
    <h3 id="wifeName">My Queen HerNameHere 👑</h3>
    <button onclick="startApp()">Start Irritating Me 😏</button>

    <div id="questionArea" class="hidden"></div>
</div>

<script>

let step = 0;

// Floating Hearts Generator
setInterval(() => {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 15 + "px";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 5000);
}, 500);

function startApp() {
    document.querySelector("button").style.display = "none";
    document.getElementById("bgMusic").play();
    showQuestion();
}

function showQuestion() {
    let area = document.getElementById("questionArea");
    area.classList.remove("hidden");

    if (step === 0) {
        area.innerHTML = `
        <h3>Are you angry because of me or hormones, HerNameHere? 😅</h3>
        <button onclick="nextStep('Because of you 😡')">Because of you</button>
        <button onclick="nextStep('Hormones CEO 🧠')">Hormones</button>
        <button onclick="nextStep('I don’t know 🤷')">I don’t know</button>
        `;
    }

    else if (step === 1) {
        area.innerHTML = `
        <h3>On scale 1-10 how much chocolate do you need right now? 🍫</h3>
        <button onclick="alert('Okay manageable 😌')">5</button>
        <button onclick="alert('Urgent chocolate required 🍫')">8</button>
        <button onclick="alert('RUNNING TO STORE NOW 🏃‍♂️🍫')">100</button>
        <br><br>
        <button onclick="nextStep()">Next Question</button>
        `;
    }

    else if (step === 2) {
        area.innerHTML = `
        <h3>What does my Queen want right now? 👑</h3>
        <button onclick="alert('Head massage loading 💆‍♀️')">Head Massage</button>
        <button onclick="alert('Ordering food now 🍜')">Food</button>
        <button onclick="alert('Okay I will be silent 🤐')">Silence</button>
        <button onclick="alert('Cuddles activated 🤗')">Cuddles</button>
        <br><br>
        <button onclick="nextStep()">Final Surprise</button>
        `;
    }

    else {
        area.innerHTML = `
        <h3>
        HerNameHere ❤️<br><br>
        Even if you shout at me…<br>
        Even if you ignore me…<br><br>
        I love you extra during these days.<br>
        Because I know it's not easy for you 🥺
        </h3>
        <button onclick="confetti()">Press if you love your irritating husband 💕</button>
        `;
    }
}

function nextStep(answer) {
    if(answer){
        alert("Noted: " + answer);
    }
    step++;
    showQuestion();
}

function confetti() {
    alert("Mission Successful 🎉 Wife slightly happy 😌❤️");
}

</script>

</body>
</html>
