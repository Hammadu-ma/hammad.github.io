<!DOCTYPE html>
<htm
l lang="en">
<head background="GardenWallpaper_flawed.jpg">
    <link rel="icon" type="image/png" href="chrome://branding/content/icon32.png">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HAMMAD TECHNOLOGIES</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/js/all.min.js" defer></script>
   <style>
 :root {
            --primary-bg: #1e1e2f; /* Dark modern background */
            --secondary-bg: #28293e; /* Secondary card background */
            --accent-color: #f0f414; /* Futuristic cyan */
            --text-color: #e0e6ed; /* Soft light text */
            --button-bg: #4fd1c5; /* Bright teal for buttons */
            
            
            
            --primary-bg: #1e1e2f; /* Dark modern background */
            --secondary-bg: #28293e; /* Secondary card background */
            --accent-color: #13d0bd; /* Futuristic cyan */
            --text-color: #e0e6ed; /* Soft light text */
            --button-bg: #11f0e5; /* Bright teal for buttons */
            --button-hover: #07752d; /* Hover state for buttons */
            --border-color: #2a2b42; /* Subtle border */
        }

        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            background-color: var(--primary-bg);
            color: var(--text-color);
            line-height: 1.6;
            overflow-x: hidden;
        }

        header {
            background-image: url('bo.jpg');
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        header h1 {
            font-size: 1.8rem;
            color: var(--accent-color);
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            gap: 1rem;
        }

        nav a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: bold;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease, color 0.3s ease;
        }

        nav a:hover {
            background-color: var(--accent-color);
            color: var(--primary-bg);
        }

        .page {
            display: none;
            padding: 2rem;
            animation: fadeIn 0.5s ease;
        }

        .active {
            display: block;
        }

        .repair-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
        }

        .repair-option {
            background-color: var(--secondary-bg);
            padding: 1.5rem;
            border-radius: 10px;
            text-align: center;
            cursor: pointer;
            transition: transform 0.3s ease, background-color 0.3s ease;
        }

        .repair-option:hover {
            transform: translateY(-5px);
            background-color: var(--accent-color);
            color: var(--primary-bg);
        }

        .form-container {
            max-width: 400px;
            margin: 0 auto;
            background-color: var(--secondary-bg);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }

        .form-container input,
        .form-container button {
            width: 100%;
            margin: 1rem 0;
            padding: 0.7rem;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
        }

        .form-container input {
            background-color: var(--primary-bg);
            color: var(--text-color);
            border: 1px solid var(--border-color);
        }

        .form-container button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }

        .form-container button:hover {
            background-color: var(--button-hover);
        }

        .appearance-toggle {
            position: fixed;
            bottom: 20px;
            left: 20px;
            z-index: 1000;
        }

        .appearance-toggle button {
            background-color: var(--accent-color);
            color: var(--primary-bg);
            padding: 0.7rem 1.5rem;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
            transition: background-color 0.3s ease;
        }

        .appearance-toggle button:hover {
            background-color: var(--button-hover);
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
            
        /* Chat Page */
        .chat-box {
            background-color: var(--secondary-bg);
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.5);
        }

        .chat-messages {
            max-height: 300px;
            overflow-y: auto;
            padding: 10rem;
            background-image: url('body.jpg');
            border: 1px solid var(--border-color);
            border-radius: 5px;
			size: width,50px hight,10px;
        }

        .chat-message {
            padding: 0.5rem;
            border-radius: 10px;
            background-image: url('body.jpg');
            color: var(--text-color);
            margin: 0.5rem 0;
            position: relative;
        }

        .chat-message .status {
            position: absolute;
            bottom: 5px;
            right: 10px;
            font-size: 0.8rem;
            color: var(--accent-color);
        }

        .chat-input {
            display: flex;
            gap: 0.5rem;
            margin-top: 1rem;
        }

        .chat-input input {
            flex: 1;
            padding: 0.7rem;
            border-radius: 5px;
            border: 1px solid var(--border-color);
            background-color: var(--secondary-bg);
            color: var(--text-color);
        }

        .chat-input button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            padding: 0.7rem 1.5rem;
            font-size: 1rem;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .chat-input button:hover {
            background-color: var(--button-hover);
        }

        /* Fade In Animation */
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
            
            
  --primary-bg: #1e1e2f; /* Dark modern background */
            --secondary-bg: #28293e; /* Secondary card background */
            --accent-color: #14e4f4; /* Futuristic cyan */
            --text-color: #e0e6ed; /* Soft light text */
            --button-bg: #4fd1c5; /* Bright teal for buttons */
            --button-hover: #3cb1a7; /* Hover state for buttons */
            --border-color: #2a2b42; /* Subtle border */
            --golden-bg: #d4af37; /* Golden color for payment page */
            --orange-box: #ff8c00; /* Orange for bank details */
            --white-color: #ffffff; /* White for text */
        }

        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            background-color: var(--primary-bg);
            color: var(--text-color);
            line-height: 1.6;
        }

        header {
            background-color: var(--secondary-bg);
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        header h1 {
            font-size: 1.8rem;
            color: var(--accent-color);
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            gap: 1rem;
        }

        nav a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: bold;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease, color 0.3s ease;
        }

        nav a:hover {
            background-color: var(--accent-color);
            color: var(--primary-bg);
        }

        .page {
            display: none;
            padding: 2rem;
            animation: fadeIn 0.5s ease;
        }

        .active {
            display: block;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            padding: 2rem;
        }

        .product-card {
            background-color: var(--secondary-bg);
            padding: 1.5rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 6px 15px rgba(6, 225, 233, 0.5);
            transition: transform 0.3s ease;
        }

        .product-card:hover {
            transform: translateY(-10px);
        }

        .product-card img {
            max-width: 40%;
            border-radius: 10px;
			-ms-flex-item-align: right;
        }

        .product-card button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            border: none;
            padding: 0.7rem 1.5rem;
            font-weight: bold;
            font-size: 1rem;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 1rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .product-card button:hover {
          background-color: var(--button-hover);
          box-shadow: 0 6px 15px rgba(149, 236, 0, 0.5);
        }

        /* Payment Page */
        .payment-box {
            background-color: var(--golden-bg);
            padding: 2rem;
            text-align: center;
            border-radius: 10px;
        }

        .payment-box button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            border: none;
            padding: 1rem;
            font-size: 1.2rem;
            font-weight: bold;
            border-radius: 10px;
            margin: 1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .payment-box button:hover {
            background-color: var(--button-hover);
        }

        .bank-details {
            background-color: var(--orange-box);
            color: var(--white-color);
            padding: 1rem;
            margin-top: 1rem;
            font-size: 1.2rem;
            font-weight: bold;
            border-radius: 10px;
        }  
 /* Pay Page */
        .pay-box button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            border: none;
            padding: 1rem;
            font-size: 2rem;
            font-weight: bold;
            border-radius: 10px;
            margin: 1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
		 .pay-box button:hover {
            background-color: var(--button-hover);
        }
		
		   .file-input {
            display: flex;
            gap: 0.5rem;
            margin-top: 1rem;
        }

        .file-input input {
            flex: 1;
            padding: 0.7rem;
            border-radius: 5px;
            border: 1px solid var(--border-color);
            background-color: var(--secondary-bg);
            color: var(--text-color);
        }
		
		.file-input button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            padding: 1rem 1.7rem;
            font-size: 1rem;
            border: block;
            border-radius: 8px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
		 .file-input button:hover {
            background-color: var(--button-hover);
        }

        .Location Page {
            display: flex;
            gap: 0.5rem;
            margin-top: 1rem;
        }

        .ipaddress {
            flex: 1;
            padding: 0.7rem;
            border-radius: 5px;
            border: 1px solid var(--border-color);
            background-color: var(--secondary-bg);
            color: var(--text-color);
        }
		
		.ipaddress button {
            background-color: var(--button-bg);
            color: var(--primary-bg);
            padding: 1rem 1.7rem;
            font-size: 1rem;
            border: block;
            border-radius: 8px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
		 .ipaddress button:hover {
            background-color: var(--button-hover);
        }
    
    </style>
</head>
<body>
    <header>
        <h1>HAMMAD TECHNOLOGIES</h1>
        <nav>
            <ul>
                <li><a id="homeLink" href="#"><i class="fas fa-home"></i>Home</a></li>
                <li><a id="chatLink" href="#"><i class="fas fa-comments"></i>Message</a></li>
                <li><a id="accountLink" href="#"><i class="fas fa-user"></i>Account </a></li>
                <li><a id="repairLink" href="#"><i class="fas fa-tools"></i>repair</a></li>
                <li><a id="aboutLink" href="#"><i class="fas fa-info-circle"></i></a></li>
            </ul>
        </nav>
                </header>
    <!-- Home Page -->
    <div class="page active" id="homePage">
        <h2>Welcome to Hammad Technologies</h2>
        <p>Your one-stop destination for cutting-edge</>
  <div class="product-card">
                <img src="\image\caro.png" alt="Smartphone">
                <h3>Smartphone</h3>
                <p>$699</p>
                <button onclick="switchPage('paymentPage')">Buy Now</button>
				<button onclick="switchPage('chatpage')">contact</button>
				
				<div>
				<img src="\hammad\fl.jpg" alt="flash product">
                <h3>flash product</h3>
                <p>$30,000</p>
                <button onclick="switchPage('paymentPage')">Buy Now</button>
				<button onclick="switchPage('chatPage')">contact</button>
				

				</div>
				
				<div>
				<img src="\Users\Hp\Pictures\Pictures\caro.jpg" alt="Smartphone">
                <h3>Smartphone</h3>
                <p>$30,000</p>
                <button onclick="switchPage('paymentPage')">Buy Now</button>
				<button onclick="switchPage('chatPage')">contact</button>
				
				</div>
				
            </div>

        </div>
    </div>
	
   <!-- payment Page -->
    <div class="page" id="paymentPage">
        <div class="payment-box">
            <h2>Select Payment Method</h2>
            <button onclick="switchPage('reportpage')">Bank</button>
            <button>Credit Card</button>
            <div id="bankDetails" class="bank-details" style="display: none;">
                Account: 100544233185
            </div>
        </div>
    </div>

<!-- reort Page -->
 <div class="page" id="reportpage">
    <div class="report-box">
            <h2>account number 1000544233185</h2>
<p> <a href="#" onclick="switchPage('payPage')" style="color: var(--accent-color);">pay</a></p>
</div>
</div>
<!-- pay Page -->
    <div class="page" id="payPage">
         <div class="pay-box">
		<h2>SEND YOUR RECIEPT</h2>
		  <div class="chat-input">
                <input type="file" id="file-input" placeholder="insert reciept..." style="color: var(--accent-color);">
        <button class="send" onclick="alert('you will be responded soon')">Send</button>
        <button class="cancel" onclick="switchPage('homePage')">Cancel</button>
   </div>
  </div>
   </div>
<!-- chat Page -->
    <div class="page" id="chatPage">
        <div class="chat-box">
            <h2>Chat with Us</h2>
            <div class="chat-messages" id="chatMessages"></div>
            <div class="chat-input">
                <input type="text" id="chatInput" placeholder="Type a message...">
                <button onclick="sendMessage()">Send</button>
            </div>
        </div>
    </div>
<!-- golden page -->
<div class="page" id="goldenpage">
<h2  background="dark.jpg"><strong> wel come to our subscription</strong> </h2> 
<div class="form-container" background="dark.jpg">
<input type="name" placeholder="firstname">
<input type="name" placeholder="lasttname">
<input type="name" placeholder="middlename">
<input type="name" placeholder="region">
<input type="name" placeholder="woreda">
<input type="name" placeholder="zone">
<input type="name" placeholder="kebele">
<button onclick="switchPage('profilePage')">submit</button>
</div>
<img  src="\image\caro.png" alt="Smartphone" >
 </div>
    <!-- Account Page -->
    <div class="page" id="accountPage">
        <div class="form-container">
            <h2>Login</h2>
            <input type="phonenumber" placeholder="enter your phone number">
            <input type="password" placeholder="Enter your password">
          <button onclick="switchPage('goldenpage')">login</button>
            <p style="text-align: center;">Don't have an account? <a href="#" onclick="switchPage('signupPage')" style="color: var(--accent-color);">Sign Up</a></p>
        </div>
    </div>

    <!-- Sign-Up Page -->
    <div class="page" id="signupPage">
        <div class="form-container">
            <h2>Sign Up</h2>
            <input type="text" placeholder="Full Name">
            <input type="email" placeholder="Email Address">
            <input type="password" placeholder="Create Password">
            <button onclick="switchPage('goldenpage')">Sign Up</button>
        </div>
    </div>
   <!-- chat Page -->
   <div class="page" id="chatPage">
        <div class="chat-box">
            <h2>Chat with Us</h2>
            <div class="chat-messages" id="chatMessages"></div>
            <div class="chat-input">
                <input type="text" id="chatInput" placeholder="Type a message...">
                <button onclick="sendMessage()">Send</button>
            </div>
        </div>
    </div>

    <!-- Repair Page -->
    <div class="page" id="repairPage">
        <h2>Select Repair Option</h2>
        <div class="repair-grid">
            <div class="repair-option" onclick="switchPage('locationPage')">Dish Repair</div>
            <div class="repair-option" onclick="switchPage('locationPage')">TV Repair</div>
            <div class="repair-option" onclick="switchPage('locationPage')">Fridge Repair</div>
            <div class="repair-option" onclick="switchPage('locationPage')">Other Appliances</div>
		    <div class="repair-option" onclick="switchPage('homePage')">hammad</div>
        </div>
    </div>

    <!-- About Page -->
    <div class="page" id="aboutPage">
        <h2>About Us</h2>
        <p>At Hammad Technologies, we provide top-notch solutions to power your world.</p>
    </div>


<!-- Location Page -->
    <div class="page" id="locationPage">
        <h2>Send Your Location</h2>
        <input type="ipaddress" id="ipaddress" placeholder="Enter your location">
        <button class="send-location" onclick="alert('locationsent')">Send</button>
        <button class="cancel" onclick="switchPage('repairPage')">Cancel</button>
    </div>



    <!-- Appearance Settings -->
    <div class="appearance-toggle">
        <button onclick="toggleTheme()">Toggle</button>
    </div>
<!-- profile page -->
    <class class="page" id="profilePage">
        <div class="form-container">
            <h2>my profile </h2>
            <input type="file" placeholder="put your picture">
          <button onclick="switchPage('homePage')">home</button>
            <p style="text-align: center;">check your information? <a href="#" onclick="switchPage('goldenpage')" style="color: var(--accent-color);">check info</a></p>
        </div>
    </class>

    <script>
        const pages = document.querySelectorAll('.page');
        document.getElementById('homeLink').onclick = () => switchPage('homePage');
        document.getElementById('accountLink').onclick = () => switchPage('accountPage');
        document.getElementById('chatLink').onclick = () => switchPage('chatPage');
        document.getElementById('repairLink').onclick = () => switchPage('repairPage');
        document.getElementById('aboutLink').onclick = () => switchPage('aboutPage');
        
        function switchPage(id) {
            pages.forEach(page => page.classList.remove('active'));
            document.getElementById(id).classList.add('active');
        }

        let isDark = true;
        function toggleTheme() {
            if (isDark) {

     const showBankDetails = () => {
            document.getElementById('bankDetails').style.display = 'block';
        };
                document.documentElement.style.setProperty('--primary-bg', '#ffffff');
                document.documentElement.style.setProperty('--text-color', '#000000');
                document.documentElement.style.setProperty('--secondary-bg', '#f4f4f4');
                isDark = false;
            } else {
                document.documentElement.style.setProperty('--primary-bg', '#1e1e2f');
                document.documentElement.style.setProperty('--secondary-bg', '#28293e');
                document.documentElement.style.setProperty('--text-color', '#e0e6ed');
                isDark = true;
            }
        }
        const goldenPage = () => {
            SubmitEvent="saveData"
            if (submit) 
        {const imputData = SVGComponentTransferFunctionElement

        }
        }

          const sendMessage = () => {
            const input = document.getElementById('chatInput');
            const message = input.value.trim();
            if (message) {
                const chatMessages = document.getElementById('chatMessages');
                const msg = document.createElement('div');
                msg.className = 'chat-message';
                msg.textContent = message;
                const status = document.createElement('span');
                status.className = 'status';
                status.textContent = '✓';
                msg.appendChild(status);
                chatMessages.appendChild(msg);
                input.value = '';
                chatMessages.scrollTop = chatMessages.scrollHeight;
            }
        };

    </script>
</body>
</html>
