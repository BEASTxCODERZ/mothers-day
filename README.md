<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>MOTHER'S DAY Card for Mom</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
}

/* Background animation */
.bg {
    height: 100vh;
    background: linear-gradient(270deg, #ff9a9e, #fad0c4, #fbc2eb);
    background-size: 600% 600%;
    display: flex;
    justify-content: center;
    align-items: center;
    animation: bgMove 10s ease infinite;
}

/* Card */
.card {
    background: white;
    width: 90%;
    max-width: 450px;
    padding: 40px 30px;
    border-radius: 25px;
    text-align: center;
    box-shadow: 0 25px 50px rgba(0,0,0,0.3);
    animation: openCard 1.5s ease forwards;
    transform: scale(0);
}

/* Text */
.card h1 {
    color: #ff4d6d;
    font-size: 32px;
}

.line {
    margin-top: 10px;
    color: #777;
    animation: fadeIn 2s ease;
}

.msg {
    margin-top: 20px;
    font-size: 18px;
    color: #333;
    line-height: 1.6;
    animation: fadeIn 3s ease;
}

.from {
    margin-top: 25px;
    font-weight: bold;
    color: #ff4d6d;
    animation: fadeIn 4s ease;
}

/* Heart animation */
.heart {
    font-size: 50px;
    margin: 20px 0;
    animation: beat 1.2s infinite;
}

/* Animations */
@keyframes openCard {
    0% {
        transform: scale(0) rotateY(90deg);
    }
    100% {
        transform: scale(1) rotateY(0);
    }
}

@keyframes beat {
    0%, 100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.3);
    }
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes bgMove {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}



<div class="bg">
    <div class="card">
        <h1>🎂 Happy Mother's Day 🎂</h1>
        <p class="line">To the most loving & caring person ❤️</p>

        <div class="heart">💖</div>

        <p class="msg">
            Thank you for your endless love, 
            sacrifices and blessings.  
            May your life be filled with happiness,  
            peace and good health🌸


        </p>

        <p class="from">— With lots of love 💕</p>
    </div>
</div>

</body>
</html>



