# Meme
Meme
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Joke Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f8ff;
            text-align: center;
        }
        .container {
            padding: 20px;
            border: 2px solid #ccc;
            border-radius: 10px;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            background-color: #4CAF50;
            color: white;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #45a049;
        }
        .joke {
            font-size: 18px;
            margin: 20px 0;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Random Joke Generator</h1>
        <p class="joke" id="joke">Loading a joke...</p>
        <button onclick="generateJoke()">Get New Joke</button>
    </div>

    <script>
        const jokes = [
            "Why don't skeletons fight each other? They don't have the guts!",
            "I told my wife she was drawing her eyebrows too high. She looked surprised!",
            "Why don’t some couples go to the gym? Because some relationships don’t work out!",
            "I used to play piano by ear, but now I use my hands.",
            "Parallel lines have so much in common. It’s a shame they’ll never meet.",
            "I told my computer I needed a break, and now it won’t stop sending me Kit-Kats!"
        ];

        function generateJoke() {
            const randomIndex = Math.floor(Math.random() * jokes.length);
            document.getElementById('joke').textContent = jokes[randomIndex];
        }

        // Load an initial joke
        generateJoke();
    </script>

</body>
</html>
