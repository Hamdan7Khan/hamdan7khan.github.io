<html>

<head>
    <title>Where is my brownie???</title>
    <script>
        document.addEventListener('DOMContentLoaded', () => {

            const yesButton = document.querySelector('#yesButton');
            const noButton = document.querySelector('#noButton');

            const moveNoButton = () => {
                const x = Math.random() * (window.innerWidth - noButton.offsetWidth);
                const y = Math.random() * (window.innerHeight - noButton.offsetHeight);

                noButton.style.position = 'absolute';
                noButton.style.left = `${x}px`;
                noButton.style.top = `${y}px`;
            };

            noButton.addEventListener('click', moveNoButton);
            noButton.addEventListener('mouseenter', moveNoButton);

        });
    </script>

    <style>
        body {
            background-color: #89cff0;
        }

        .buttons {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        #yesButton {
            margin-right: 20px;

        }

        button {
            padding: 20px;
            font-size: 23px;
            font-family: Arial;
            font-weight: bold;
            border-radius: 10px;
            border: 0;
            background-color: #f0899c;
        }
        #yesButton:hover{
            cursor: pointer;
        }
    </style>
</head>

<body>
    <div class="buttons">
        <button class="button" id="yesButton" onclick="alert('GOOD GURL');">
            Will send it soon :&#41;
        </button>
        <button class="button" id="noButton">
            no brownie for you
        </button>

    </div>
    
</body>

</html>
