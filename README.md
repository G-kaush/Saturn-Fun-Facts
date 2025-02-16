# Saturn-Fun-Facts
GenAI 101 workshop
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Saturn Facts</title>
    <style>
        body {
            background: linear-gradient(135deg, #f3e5ab, #e0c68c, #d6cfc4);
            font-family: Arial, sans-serif;
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        #fact-container {
            text-align: center;
        }

        #fact {
            background-color: #f9f3e8; /* Soft beige */
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            margin-bottom: 20px;
        }

        button {
            background-color: #d4af37; /* Golden */
            color: #f3e5ab; /* Pale yellow */
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #c49a2a; /* Darker golden on hover */
        }
    </style>
</head>
<body>
    <div id="fact-container">
        <div id="fact">Click the button to get a random fact about Saturn!</div>
        <button id="fact-button">Get Random Fact</button>
    </div>
    <script>
        const facts = [
            "Saturn is the sixth planet from the Sun and the second-largest in the solar system.",
            "It is famous for its stunning rings, which are made up of ice and rock particles.",
            "Saturn has a total of 82 moons, with Titan being the largest and even larger than the planet Mercury.",
            "The planet is a gas giant, primarily composed of hydrogen and helium.",
            "Saturn has the lowest density of all the planets; it could float in water if a body of water large enough existed.",
            "A day on Saturn lasts about 10.7 hours, but a year on Saturn takes about 29.5 Earth years.",
            "Saturn's winds can reach speeds of up to 1,100 miles per hour (1,800 kilometers per hour).",
            "The planet has a faint ring system that extends far beyond its main rings.",
            "Saturn's atmosphere features storms, including a giant storm that can be seen from Earth.",
            "The planet's iconic yellow and gold hues are due to the presence of ammonia crystals in its upper atmosphere."
        ];

        document.getElementById('fact-button').addEventListener('click', function() {
            const randomIndex = Math.floor(Math.random() * facts.length);
            document.getElementById('fact').textContent = facts[randomIndex];
        });
    </script>
</body>
</html>
