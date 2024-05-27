<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Air Flash Staff Portal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            text-align: center;
            padding: 20px;
            border: 2px solid #333;
            border-radius: 10px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            overflow-y: auto;
            max-height: 90vh;
            width: 80%;
        }
        input[type="password"], button {
            padding: 10px;
            font-size: 16px;
            margin-top: 10px;
        }
        button {
            cursor: pointer;
        }
        .content {
            display: none;
            margin-top: 20px;
            text-align: left;
        }
        .content p, .content ul {
            margin: 0 0 10px;
            line-height: 1.6;
        }
        .button-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .button-container button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
        }
        .document {
            display: none;
        }
    </style>
    <script>
        function showPasswordInput(documentType) {
            document.getElementById("password-section").style.display = "block";
            document.getElementById("password").dataset.documentType = documentType;
        }

        function checkPassword() {
            const password = document.getElementById("password").value;
            const documentType = document.getElementById("password").dataset.documentType;
            let correctPassword = "";

            if (documentType === "firstOfficer") {
                correctPassword = "FlashFirstOfficer53";
            } else if (documentType === "cabinCrew") {
                correctPassword = "CabinCrewOnTop5";
            } else if (documentType === "groundOperations") {
                correctPassword = "LoveFuelingPlanes1";
            }

            if (password === correctPassword) {
                document.getElementById("password-section").style.display = "none";
                document.getElementById(documentType).style.display = "block";
            } else {
                alert("Incorrect password. Please try again.");
            }
        }

        function redirectToGoogle() {
            window.location.href = "https://google.com";
        }
    </script>
</head>
<body>
    <div class="container" id="main">
        <h1>Welcome to Air Flash Staff Portal</h1>
        <p>Select a guide to access:</p>
        <div class="button-container">
            <button onclick="showPasswordInput('firstOfficer')">First Officer Guide</button>
            <button onclick="showPasswordInput('cabinCrew')">Cabin Crew Guide</button>
            <button onclick="showPasswordInput('groundOperations')">Ground Operations Guide</button>
        </div>
    </div>
    
    <div class="container" id="password-section" style="display:none;">
        <h2>Enter Password</h2>
        <input type="password" id="password" placeholder="Enter Password">
        <button onclick="checkPassword()">Submit</button>
    </div>
    
    <div class="container document" id="firstOfficer">
        <h2>First Officer Guide</h2>
        <p>Welcome!</p>
        <p>Welcome to Air Flash, where we fly, but fly faster. We are a low-cost, British Ro-Aviation airline founded in the middle of March 2024 by aviatorflash, bringing such an exciting era to ro-aviation, with constant giveaways, development, flights and many classes to choose at such a low price! Daily, at Air Flash, we thrive to make a safe community. Thanks to our amazing members of staff, and members of the server, this is truly possible. We operate from Liverpool John Lennon Airport, which is the airport where we are located.</p>
        <p>You have chosen to be a part of our First Officer Team, where we will teach you how to become a truly professional and amazing Pilot, who will one day climb up the ranks to become a Captain.</p>
        <p>Get Started:</p>
        <p>At AirFlash, our main aircraft which we use is the Airbus A320. The manufacturer of the plane (In Roblox) is AeroWare, which is one of the most popular developers for aircrafts within the Ro-Aviation Community. It is a pretty simple system, however very realistic, with all features which are needed, eg. Lights, Spoilers, Flaps etc. ( <a href="https://ibb.co/Svfp9vN">Check to see how it looks like</a> ).</p>
        <p>What to do:</p>
        <p>You may not always remember in what order to do things, therefore we have created a guide. We encourage staff to use it during flights, as there is no room for mess ups! Read the guide below.</p>
        <ul>
            <li><strong>Pre-Flight:</strong></li>
            <li>Activate Battery: ON</li>
            <li>Switch on Navigation Lights: ON (Always active when Battery is on)</li>
            <li>Illuminate Logo Lights: ON (Only between 17:00 - 09:00 in-game time)</li>
            <li>Power up Auxiliary Power Unit (APU): ON (Only if GPU is not connected)</li>
            <li>Turn on Dome Light: ON</li>
            <li><strong>Pre-Taxi:</strong></li>
            <li>Activate Beacon Lights: ON (Once the final ground vehicle is detached)</li>
            <li><strong>Engine Start:</strong></li>
            <li>Start Engine 1: START (Once pushback is halfway complete)</li>
            <li>Start Engine 2: START (After Engine 1 is fully started)</li>
            <li>Deactivate Auxiliary Power Unit (APU): OFF (During Engine 2 start-up)</li>
            <li><strong>Taxiing:</strong></li>
            <li>Turn on Taxi Lights: ON</li>
            <li>Set Flaps: 1+F (Initial takeoff configuration)</li>
            <li>Turn off Dome Light: OFF</li>
            <li>Perform Spoilers Check: UP then DOWN (Ensure functionality)</li>
            <li><strong>Pre-Runway:</strong></li>
            <li>Turn off Taxi Lights: OFF (At the holding point)</li>
           
            <li>Switch on Strobe Lights: ON (Before entering the active runway)</li>
            <li>Switch off Logo Lights: OFF (Before entering the active runway)</li>
            <li>Adjust Flaps: 2 (Only for Airbus A321-200 and A321neo, set takeoff flaps)</li>
            <li>Turn on Landing Lights: ON (Once lined up on the runway)</li>
            <li>Arm Spoilers: ARM (Once lined up on the runway)</li>
            <li><strong>Takeoff Sequence:</strong></li>
            <li>Retract Landing Gear: RETRACTED (At approximately 100 ft)</li>
            <li>Set Flaps to Zero: 0 (At approximately 1000 ft or as directed by the captain)</li>
            <li>Turn off Landing Lights: OFF (At approximately 1000 ft)</li>
            <li><strong>In-Flight (Cruise):</strong></li>
            <li>Enable Cruise Setting: ON (As commanded by the captain, usually between 4,000 to 6,000 feet)</li>
            <li><strong>Descent Preparation:</strong></li>
            <li>Set Flaps: 1 (As directed by the captain)</li>
            <li>Set Flaps: 2 (As directed by the captain)</li>
            <li>Turn on Landing Lights: ON (As directed by the captain)</li>
            <li>Set Flaps: 3 (As directed by the captain)</li>
            <li>Lower Landing Gear: DOWN (As directed by the captain)</li>
            <li>Set Flaps: 4 (As directed by the captain)</li>
            <li><strong>Landing:</strong></li>
            <li>Deploy Spoilers: UP (Upon touchdown)</li>
            <li><strong>Post-Landing:</strong></li>
            <li>Retract Spoilers: DOWN (Once off the runway)</li>
            <li>Set Flaps to Zero: 0 (Once off the runway)</li>
            <li>Turn off Landing Lights: OFF (After turning off the runway)</li>
            <li>Turn off Strobe Lights: OFF (Once fully off the runway)</li>
            <li>Turn on Taxi Lights: ON (Once fully off the runway)</li>
        </ul>
    </div>
    
    <div class="container document" id="cabinCrew">
        <h2>Cabin Crew Guide</h2>
        <p>Welcome To The Air Flash Cabin Crew Team!</p>
        <p>Welcome to Air Flash, where we fly, but fly faster. We are a low-cost, British Ro-Aviation airline founded in the middle of March 2024 by aviatorflash, bringing an exciting new era to Ro-Aviation with constant giveaways, development, flights, and many classes to choose from at such low prices! Daily, at Air Flash, we thrive to create a safe and welcoming community. Thanks to our amazing members of staff and the vibrant members of our server, this is truly possible. We operate from Liverpool John Lennon Airport, which serves as our home base.</p>
        <p>You have chosen to be a part of our Cabin Crew team, where we will teach you how to unleash your full potential and professionalism, and watch you climb the ranks up to a Cabin Crew Supervisor, or more Internal Roles! There really is no guide to being a Cabin Crew member, but there are some things we expect of you!</p>
        <ol>
            <li><strong>Professionalism:</strong> Always maintain a professional attitude. You are the face of Air Flash, and your behavior should reflect the high standards we uphold.</li>
            <li><strong>Customer Service:</strong> Provide excellent customer service. Our passengers' experience is paramount, and your role is crucial in ensuring they have a pleasant flight.</li>
            <li><strong>Safety First:</strong> Prioritize safety at all times. Familiarize yourself with all safety procedures and protocols to ensure the well-being of our passengers and crew.</li>
            <li><strong>Teamwork:</strong> Work well with your colleagues. A cohesive team ensures smooth operations and a positive environment for everyone.</li>
            <li><strong>Flexibility:</strong> Be adaptable to changing schedules and scenarios. Aviation is dynamic, and flexibility is key to handling unexpected situations.</li>
            <li><strong>Communication:</strong> Communicate effectively with passengers and team members. Clear and concise communication helps in providing better service and addressing any issues promptly.</li>
            <li><strong>Presentation:</strong> Maintain a neat and presentable appearance. Adhering to our uniform standards and grooming guidelines is essential in portraying a professional image.</li>
            <li><strong>Training:</strong> Engage actively in all training sessions. Continuous learning and improvement are vital for your growth and the overall success of Air Flash.</li>
        </ol>
        <p>We are thrilled to have you on board and look forward to seeing you excel in your role. Remember, the sky is not the limit at Air Flash – it's just the beginning. Let's make every flight a memorable one for our passengers.</p>
        <p>Welcome aboard, and let’s fly faster together!</p>
        <p>Warm regards,</p>
        <p>The Air Flash Management Team</p>
        <button onclick="redirectToGoogle()">Done Reading</button
        </div>

        <div class="container document" id="groundOperations">
            <h2>Ground Operations Guide</h2>
            <p>Welcome To The Air Flash Ground Crew Team!</p>
            <p>Welcome to Air Flash, where we fly, but fly faster. We are a low-cost, British Ro-Aviation airline founded in the middle of March 2024 by aviatorflash, bringing an exciting new era to ro-aviation with constant giveaways, development, flights, and many classes to choose from at such low prices! Daily, at Air Flash, we thrive to create a safe and welcoming community. Thanks to our amazing members of staff and the vibrant members of our server, this is truly possible. We operate from Liverpool John Lennon Airport, which serves as our home base.</p>
            <p>You have chosen to be a part of our Ground Crew team, a crucial role that ensures the smooth operation of our flights and the satisfaction of our passengers. Here are some instructions and expectations to help you excel in your role:</p>
            <ol>
                <li><strong>Aircraft Preparation:</strong> Before each flight, ensure that the aircraft is properly prepared. This includes refueling, performing pre-flight checks, and verifying that all necessary supplies are on board.</li>
                <li><strong>Passenger Assistance:</strong> Assist passengers with boarding and deplaning. Provide directions, answer questions, and help with any special needs to ensure a smooth and pleasant experience.</li>
                <li><strong>Baggage Handling:</strong> Manage the loading and unloading of baggage. Ensure that all luggage is handled with care and properly stowed to prevent damage and facilitate easy retrieval.</li>
                <li><strong>Safety Procedures:</strong> Adhere to all safety protocols at all times. This includes wearing the appropriate safety gear and being aware of your surroundings to prevent accidents.</li>
                <li><strong>Communication:</strong> Maintain clear and constant communication with the flight crew and other ground staff. Use provided communication tools to coordinate activities and ensure everyone is on the same page.</li>
                <li><strong>Customer Service:</strong> Provide excellent customer service. Greet passengers with a friendly attitude and assist them with any issues or concerns they might have while on the ground.</li>
                <li><strong>Time Management:</strong> Be punctual and manage your time efficiently. Ensure that all ground operations are completed promptly to avoid any delays in flight schedules.</li>
                <li><strong>Training and Development:</strong> Engage actively in all training sessions provided by Air Flash. Stay updated with the latest procedures and protocols to ensure the highest level of efficiency and safety.</li>
            </ol>
            <p>We are thrilled to have you on board and look forward to seeing you excel in your role. Remember, the ground crew is the backbone of our operations, and your efforts are vital in making each flight a success.</p>
            <p>Welcome aboard, and let’s work together to make Air Flash the best</p>
        </div>
        
        </body>
        </html>
            
