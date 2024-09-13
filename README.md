<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heart Button with Message</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffe4e1;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            flex-direction: column;
        }

        /* Container for hearts and button */
        .button-container {
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 20px;
        }

        /* Red button in the middle */
        #heartButton {
            padding: 15px 30px;
            background-color: red;
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 18px;
            cursor: pointer;
            z-index: 1;
        }

        /* Hearts surrounding the button */
        .heart {
            position: absolute;
            font-size: 30px;
            color: #FF1493;
            animation: float 4s infinite ease-in-out;
        }

        .heart:nth-child(1) {
            top: -30px;
            left: -40px;
            animation-delay: 0.2s;
        }

        .heart:nth-child(2) {
            top: -30px;
            right: -40px;
            animation-delay: 0.4s;
        }

        .heart:nth-child(3) {
            bottom: -30px;
            left: -40px;
            animation-delay: 0.6s;
        }

        .heart:nth-child(4) {
            bottom: -30px;
            right: -40px;
            animation-delay: 0.8s;
        }

        /* Animation for floating hearts */
        @keyframes float {
            0% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-15px);
            }
            100% {
                transform: translateY(0);
            }
        }

        /* Message that appears after clicking */
        #message {
            display: none;
            font-size: 24px;
            color: #FF6347;
            text-align: center;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <!-- Container with button and hearts -->
    <div class="button-container">
        <!-- Red Button -->
        <button id="heartButton">Press Me</button>

        <!-- Hearts around the button -->
        <div class="heart">❤️</div>
        <div class="heart">❤️</div>
        <div class="heart">❤️</div>
        <div class="heart">❤️</div>
    </div>

    <!-- Message that appears after button is clicked -->
    <div id="message">I want to butt fuck you till I cum inside!</div>

    <script>
        // JavaScript to show message after button click
        const heartButton = document.getElementById('heartButton');
        const message = document.getElementById('message');

        heartButton.addEventListener('click', () => {
            message.style.display = 'block'; // Show the message
        });
    </script>

</body>
</html>
