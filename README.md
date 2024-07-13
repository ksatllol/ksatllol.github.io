<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>jetBlue Roblox</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #E0F7FA;
            color: #01579B;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            min-height: 100vh;
            box-sizing: border-box;
        }
        header {
            background-color: #0288D1;
            width: 100%;
            padding: 10px 20px;
            text-align: center;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        header img {
            width: 150px;
            border-radius: 10px;
        }
        .nav-buttons {
            display: flex;
            gap: 20px;
        }
        .btn {
            background-color: #039BE5;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        .btn:hover {
            background-color: #0277BD;
        }
        .content {
            text-align: center;
            margin: 20px;
            width: 100%;
            box-sizing: border-box;
            padding-top: 60px; /* Adjusted padding for header space */
        }
        .page {
            display: none;
        }
        .page.active {
            display: block;
        }
        footer {
            background-color: #f1f3f4;
            padding: 10px;
            text-align: center;
            width: 100%;
            font-size: 12px;
            color: #757575;
            margin-top: auto;
        }
    </style>
</head>
<body>
    <header>
        <img src="https://cdn.discordapp.com/attachments/1261374917509910572/1261713458349740042/XTo9lYW.png?ex=6693f5b9&is=6692a439&hm=b7f38925b0dfa0bbee300e193a1634db611835f296b88b04c5e509faeb476973" alt="JetBlue Logo">
        <div class="nav-buttons">
            <div class="btn" onclick="showPage('home')">Home</div>
            <div class="btn" onclick="showPage('timetable')">Flight Timetable</div>
            <div class="btn" onclick="showPage('information')">Information</div>
            <div class="btn" onclick="location.href='https://discord.gg/WVUp84TRKp'">Discord Server</div>
            <div class="btn" onclick="location.href='https://roblox.com'">Roblox Group</div>
        </div>
    </header>
    <div id="home" class="page active">
        <div class="content">
            <h1>Welcome to jetBlue Roblox!</h1>
            <p>Join our amazing community and experience the best of virtual aviation with jetBlue on Roblox.</p>
            <p>Add more information about jetBlue Roblox here...</p>
        </div>
    </div>
    <div id="timetable" class="page">
        <div class="content">
            <h1>Flight Timetable</h1>
            <p>Sorry! There are no scheduled flights as of now.</p>
        </div>
    </div>
    <div id="information" class="page">
        <div class="content">
            <h1>Information</h1>
            <p>jetBlue is going through a much needed renovation due to new management put in place. Sorry for any inconvenience that could have been caused by this.</p>
        </div>
    </div>
    <footer>
        jetBlue Roblox is in no way affiliated with the real jetBlue Airlines. We are simply a fan page.
    </footer>

    <script>
        function showPage(pageId) {
            const pages = document.querySelectorAll('.page');
            pages.forEach(page => {
                if (page.id === pageId) {
                    page.classList.add('active');
                } else {
                    page.classList.remove('active');
                }
            });
        }
    </script>
</body>
</html>
