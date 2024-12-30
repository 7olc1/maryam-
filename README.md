<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maryam's Space</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom, #ffffff, #ffe0b2);
            overflow: hidden;
        }
        .moon {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 200px;
            height: 200px;
            background: #f5deb3;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 0 50px rgba(0, 0, 0, 0.2);
            font-size: 24px;
            font-weight: bold;
            color: #555;
            text-align: center;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background: orange;
            transform: rotate(45deg);
            animation: float 4s infinite;
        }
        .heart:before,
        .heart:after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            background: orange;
            border-radius: 50%;
        }
        .heart:before {
            top: -10px;
            left: 0;
        }
        .heart:after {
            left: -10px;
            top: 0;
        }
        @keyframes float {
            0% {
                transform: translateY(0) rotate(45deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(45deg);
                opacity: 0;
            }
        }
        .heart:nth-child(1) {
            top: 70%;
            left: 20%;
            animation-duration: 3s;
        }
        .heart:nth-child(2) {
            top: 50%;
            left: 40%;
            animation-duration: 4s;
            animation-delay: 1s;
        }
        .heart:nth-child(3) {
            top: 60%;
            left: 70%;
            animation-duration: 5s;
            animation-delay: 2s;
        }
    </style>
</head>
<body>
    <div class="moon">Maryam</div>

    <!-- Floating hearts -->
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>

    <!-- Audio player -->
    <audio autoplay loop>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
</body>
</html>
