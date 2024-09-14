- 👋 Hi, I’m @Yahuza624
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Yahuza624/Yahuza624 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Car Business - Featured Models</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1em;
        }
        .car-models {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            margin: 20px;
        }
        .car {
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            width: 250px;
            margin: 10px;
            padding: 15px;
            text-align: center;
        }
        .car img {
            width: 100%;
            border-bottom: 1px solid #ddd;
            margin-bottom: 15px;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
        #chatbot {
            position: fixed;
            bottom: 50px;
            right: 20px;
            background-color: #333;
            color: white;
            padding: 15px;
            border-radius: 10px;
            display: none;
        }
        #chatbot.open {
            display: block;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to Car Business</h1>
        <p>Explore Our Featured Car Models</p>
    </header>

    <section class="car-models">
        <div class="car">
            <img src="bmw.jpg" alt="BMW">
            <h2>BMW</h2>
            <p>Price: $40,000</p>
        </div>
        <div class="car">
            <img src="toyota_camry.jpg" alt="Toyota Camry">
            <h2>Toyota Camry</h2>
            <p>Price: $30,000</p>
        </div>
        <div class="car">
            <img src="toyota_tacoma.jpg" alt="Toyota Tacoma">
            <h2>Toyota Tacoma</h2>
            <p>Price: $35,000</p>
        </div>
        <div class="car">
            <img src="toyota_tundra.jpg" alt="Toyota Tundra">
            <h2>Toyota Tundra</h2>
            <p>Price: $45,000</p>
        </div>
        <div class="car">
            <img src="benz.jpg" alt="Mercedes Benz">
            <h2>Mercedes Benz</h2>
            <p>Price: $50,000</p>
        </div>l
    </section>

    <footer>
        <p>&copy; 2024 Car Business. All rights reserved.</p>
    </footer>

    <!-- Chatbot Section -->
    <div id="chatbot">
        <p>Hello! How can I help you today?</p>
        <input type="text" id="userInput" placeholder="Type your inquiry here...">
        <button onclick="sendMessage()">Send</button>
        <div id="response"></div>
    </div>

    <button onclick="toggleChat()">Chat with us</button>

    <script>
        function toggleChat() {
            const chatbot = document.getElementById('chatbot');
            chatbot.classList.toggle('open');
        }

        function sendMessage() {
            const userMessage = document.getElementById('userInput').value;
            const responseDiv = document.getElementById('response');
            
            // Basic response simulation
            if (userMessage.toLowerCase().includes('price')) {
                responseDiv.innerHTML = '<p>Prices start at $30,000. Let me know if you want more details!</p>';
            } else {
                responseDiv.innerHTML = '<p>Thank you for your inquiry! We will get back to you soon.</p>';
            }

            document.getElementById('userInput').value = ''; // Clear input
        }
    </script>

</body>
</html>
