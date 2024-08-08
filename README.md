# Mini-RGPV-portal-
This web page is basically for study purpose and it is a simple landing page 📃📃
<!DOCTYPE html>
<html lang="en">

<head>
	<meta charset="UTF-8">
	<meta name="viewport" content=
"width=device-width, initial-scale=1.0">
      
	<style>
        /* style.css */

body {
	font-family:
'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	margin: 0;
	padding: 0;
	background-color: #0a939a;
}

#APRSY{
	display: flex;
	flex-direction: column;
	min-height: 100vh;
}

header {
	background-color: #0108017a;
	color: rgb(66, 169, 87);
	text-align: center;
	padding: 1em;
}

nav {
	background-color: #ce111b;
}

nav ul {
	list-style-type: none;
	margin: 0;
	padding: 0;
	display: flex;
	justify-content: center;
}

nav li {
	margin: 0;
}

nav a {
	text-decoration: none;
	color: #240b95;
	padding: 1em;
	display: block;
	transition: background-color 0.3s ease;
}

nav a:hover {
	background-color: #aa1313;
}

main {
	flex: 1;
	padding: 1em;
}

#content {
	max-width: 1000px;
	margin: 0 auto;
	background-color: #bed10b;
	padding: 20px;
	border-radius: 8px;
	box-shadow:
0 0 10px rgba(0, 0, 0, 0.1);
}

#content h2 {
	color: #ca0e0e;
}

#content img {
	width: 400px;
	height: auto;
	margin: 0 auto;
	display: block;
	border-radius: 10px;
	box-shadow: 
2px 2px 5px rgba(6, 74, 171, 0.877);
	border: 3px solid #2F8D46;
}

form {
	max-width: 400px;
	margin: 20px auto;
	padding: 20px;
	background-color: #0a46a0;
	border-radius: 8px;
	box-shadow: 
0 0 10px rgba(117, 12, 33, 0.884);
}

form label {
	display: block;
	margin-bottom: 8px;
}

form input,
form textarea {
	width: 100%;
	padding: 8px;
	margin-bottom: 16px;
	box-sizing: border-box;
	border: 1px solid #dadee0;
	border-radius: 4px;
}

form button {
	background-color: #b60f20;
	color: #220ed1;
	padding: 10px;
	border: none;
	border-radius: 4px;
	cursor: pointer;
	transition: 
background-color 0.3s ease;
}

form button:hover {
	background-color: #4410be;
}

    </style>
	<title>YOGESH MALVIYA</title>
</head>

<body>

    
	<div id="app">
		<header>

			<h1>
				<i>Developed by A.P.R.S.Y</i>
			</h1>
			<h1>R G P V PORTAL

            </h1>

			</h1>
            
		</header>
		<nav>
			<ul>
				<li>
					<a href="#" onclick=
					"changeContent('home')">
						Home
					</a>
				</li>
				<li>
					<a href="#" onclick=
					"changeContent('about')">
						About
					</a>
				</li>
				<li>
					<a href="#" onclick=
					"changeContent('contact')">
						Contact
					</a>
				</li>
			</ul>
		</nav>
		<main>
			<div id="content">

				<img src=
"">
				<h2>Welcome to A.P.R.S.Y WEBSITE</h2>
				<p>
					<B>This is the main portal of RGPV diploma
                    this web page is redirect to the main RGPV diploma</B>
                
			
				</p>
				<p>
					<I>Visit the RGPV Diploma portal</I>
					<a href="https://www.rgpvdiploma.in/" target="_blank">
						CLICK
					</a>.
				</p>
			</div>
		</main>
	</div>
	<script src="script.js"></script>
    <script> 
        function changeContent(page) {
	var contentDiv = document.getElementById('content');

	switch (page) {
		case 'home':
			contentDiv.innerHTML = `
				<img src=
"">
				<h2>
					Welcome to the Home Page!
				</h2>
				<p>
					This is the main page OF RGPV Diploma.
                <p>
                    Student login
                    <a href="https://www.rgpvdiploma.in/StudentLife/StudentLogin.aspx"target="_blank">
                          click</a></p>
                <p> 
                    Institute login
                    <a href="https://www.rgpvdiploma.in/Institutions/Institutionslogin.aspx"target="_blank">
                          click</a></p>
                 <p>Employee login
                    <a href="https://www.rgpvdiploma.in/Admin/EmployerLogin.aspx"target="_blank">
                         click</a></p>             

				</p>
				<p>
					<b>Explore the different sections using
					the navigation menu.</b>
				</p>
			`;
			break;
		case 'about':
			contentDiv.innerHTML = `
				<h2>About Us</h2>
				<p>
					This is the about page content. Learn more 
					about our purpose and team.
				</p>
				<p>
					This web page created by the C.S.E Branch student
				</p>
			`;
			break;
		case 'contact':
			contentDiv.innerHTML = 
				`<h2>Contact Us</h2> 
				<p>
					The user can face any problem to contect us!
				</p> 
				<form> 
				<label for="name">Name:</label> 
				<input type="text" id="name" name="name" 
						placeholder="Your Name" required>
				<label for="email">Email:</label> 
				<input type="email" id="email" name="email" 
						placeholder="Your Email" required>
				<label for="message">Message:</label> 
				<textarea id="message" name="message" 
							placeholder="Your Message" 
							rows="4" required>
					</textarea>
				<button type="submit">Send Message</button> 
				</form>`;
			break;

		default:
			contentDiv.innerHTML = '<h2>Page not found!</h2>';
	}
}

    </script>
</body>

</html>
