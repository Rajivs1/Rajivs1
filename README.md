<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub README</title>
    <style>
        @keyframes floatEffect {
            0% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
            100% { transform: translateY(0); }
        }
        body {
            font-family: Arial, sans-serif;
            transition: background-color 0.3s, color 0.3s;
        }
        .floating {
            display: inline-block;
            animation: floatEffect 2s ease-in-out infinite;
            font-size: 26px;
            font-weight: bold;
        }
        .dark-mode {
            background-color: #121212;
            color: #ffffff;
        }
        .light-mode {
            background-color: #ffffff;
            color: #000000;
        }
        .toggle-btn {
            margin: 20px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        .dark-btn {
            background-color: #ffffff;
            color: #121212;
        }
        .light-btn {
            background-color: #121212;
            color: #ffffff;
        }
    </style>
</head>
<body class="light-mode">
    <button class="toggle-btn light-btn" onclick="toggleTheme()">Switch to Dark Mode</button>
    <h1 class="floating">Hi there 👋, I'm <b>Rajiv Ranjan!</b></h1>
    
    <h2>👨‍💻 About Me</h2>
    <ul>
        <li>🔭 I’m currently working on <b>My new Project</b> and <b>StudyNotion</b>.</li>
        <li>🌱 I’m learning <b>Data Structures, Algorithms, and Backend Development</b>.</li>
        <li>💬 Ask me about <b>HTML, CSS, JavaScript, MERN Stack, C, C++, Python, and Cricket</b>.</li>
        <li>🎓 Final Year B.Tech in CSE.</li>
    </ul>
    
    <h2>⚡ Technologies</h2>
    <table border="1">
        <tr>
            <th>Programming Languages</th>
            <th>Frontend</th>
            <th>Backend</th>
            <th>Database</th>
            <th>Other</th>
        </tr>
        <tr>
            <td>C, C++, Python, Java</td>
            <td>HTML, CSS, Tailwind CSS, Bootstrap, JavaScript</td>
            <td>Node.js, Express.js</td>
            <td>MongoDB, SQL</td>
            <td>Git, GitHub</td>
        </tr>
    </table>
    
    <h2>📫 How to Reach Me</h2>
    <ul>
        <li><a href="https://www.linkedin.com/in/rajiv-ranjan1" target="_blank">LinkedIn</a></li>
        <li><a href="mailto:rajeev04632@gmail.com">Email</a></li>
        <li><a href="https://github.com/Rajivs1" target="_blank">GitHub</a></li>
        <li><a href="https://wa.me/8521982915" target="_blank">WhatsApp</a></li>
    </ul>
    
    <script>
        function toggleTheme() {
            const body = document.body;
            const button = document.querySelector(".toggle-btn");
            
            if (body.classList.contains("light-mode")) {
                body.classList.replace("light-mode", "dark-mode");
                button.textContent = "Switch to Light Mode";
                button.classList.replace("light-btn", "dark-btn");
            } else {
                body.classList.replace("dark-mode", "light-mode");
                button.textContent = "Switch to Dark Mode";
                button.classList.replace("dark-btn", "light-btn");
            }
        }
    </script>
</body>
</html>
