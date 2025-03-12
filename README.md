<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cyberpunk Tech Showcase</title>
    <style>
        body {
            background-color: black;
            color: #00ff00;
            font-family: 'Courier New', monospace;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        h1 {
            font-size: 3rem;
            text-shadow: 0 0 10px #00ff00;
        }
        .container {
            padding: 50px;
        }
        .projects {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        .project-card {
            background: rgba(0, 255, 0, 0.2);
            border: 1px solid #00ff00;
            padding: 20px;
            margin: 20px;
            width: 300px;
            box-shadow: 0 0 15px #00ff00;
            transition: transform 0.3s ease-in-out;
        }
        .project-card:hover {
            transform: scale(1.1);
            box-shadow: 0 0 25px #00ff00;
        }
        .ai-section {
            margin-top: 50px;
            padding: 20px;
            border: 1px solid #00ff00;
            background: rgba(0, 255, 0, 0.1);
            box-shadow: 0 0 15px #00ff00;
        }
        #ai-response {
            font-style: italic;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Cyberpunk Tech Showcase</h1>
        <p>Welcome to my futuristic project showcase in SAP & Cybersecurity.</p>
        
        <div class="projects">
            <div class="project-card">
                <h2>Project 1</h2>
                <p>Brief description of the project.</p>
            </div>
            <div class="project-card">
                <h2>Project 2</h2>
                <p>Brief description of the project.</p>
            </div>
        </div>
        
        <div class="ai-section">
            <h2>AI Assistant</h2>
            <p>Ask the AI a question about my projects:</p>
            <input type="text" id="ai-input" placeholder="Type your question...">
            <button onclick="generateAIResponse()">Ask</button>
            <p id="ai-response"></p>
        </div>
    </div>
    
    <script>
        function generateAIResponse() {
            const input = document.getElementById("ai-input").value;
            const responseElement = document.getElementById("ai-response");
            
            if (input.toLowerCase().includes("sap")) {
                responseElement.innerText = "SAP is a powerful ERP system that helps businesses manage operations efficiently.";
            } else if (input.toLowerCase().includes("cybersecurity")) {
                responseElement.innerText = "Cybersecurity involves protecting systems and data from cyber threats using various defense mechanisms.";
            } else {
                responseElement.innerText = "I'm still learning. Ask me about SAP or cybersecurity!";
            }
        }
    </script>
</body>
</html>
