<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Profile</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .loader {
            border: 16px solid #f3f3f3;
            border-top: 16px solid #00D9FF;
            border-radius: 50%;
            width: 60px;
            height: 60px;
            animation: spin 2s linear infinite;
        }
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        .hidden {
            display: none;
        }
        .content {
            display: none;
        }
    </style>
</head>
<body>
    <div class="loader"></div>
    <div class="content">
        <h1>My Profile</h1>
        <h2>Name: Hanzlazahid007</h2>
        <h3>Role: Software Developer</h3>
        <h4>Tech Stack: HTML, CSS, JavaScript, React, Node.js</h4>
        <h5>Projects:
            <ul>
                <li>Project 1</li>
                <li>Project 2</li>
                <li>Project 3</li>
            </ul>
        </h5>
        <h5>GitHub Stats:</h5>
        <ul>
            <li>Stars: 100</li>
            <li>Forks: 20</li>
            <li>Contributors: 5</li>
        </ul>
    </div>
    <script>
        setTimeout(function() {
            document.querySelector('.loader').classList.add('hidden');
            document.querySelector('.content').style.display = 'block';
        }, 5000);
    </script>
</body>
</html>
