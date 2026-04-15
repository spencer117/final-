-<!DOCTYPE html>
<html>
<head>
    <title>My Personal Website</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial;
        }

        body {
            background: #f5f7fa;
            scroll-behavior: smooth;
        }

        /* NAVBAR */
        nav {
            background: #222;
            padding: 15px;
            text-align: center;
            position: sticky;
            top: 0;
        }

        nav a {
            color: white;
            margin: 15px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00adb5;
        }

        /* SECTIONS */
        section {
            padding: 50px;
            text-align: center;
        }

        h2 {
            margin-bottom: 20px;
            color: #333;
        }

        /* PROFILE */
        .profile img {
            width: 150px;
            border-radius: 50%;
            border: 4px solid #00adb5;
            transition: 0.3s;
        }

        .profile img:hover {
            transform: scale(1.1);
        }

        /* BUTTON */
        .btn {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background: #00adb5;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }

        /* TABLE */
        table {
            margin: auto;
            width: 60%;
            border-collapse: collapse;
            background: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        th {
            background: #00adb5;
            color: white;
        }

        th, td {
            padding: 12px;
            border: 1px solid #ddd;
        }

        /* FORM */
        form {
            max-width: 400px;
            margin: auto;
        }

        input, textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        input[type="submit"] {
            background: #00adb5;
            color: white;
            border: none;
            cursor: pointer;
        }

        input[type="submit"]:hover {
            background: #028a90;
        }

        /* ANIMATION */
        section {
            animation: fadeIn 1s ease-in;
        }

        @keyframes fadeIn {
            from {opacity: 0;}
            to {opacity: 1;}
        }
    </style>

</head>

<body>

<!-- NAVIGATION -->
<nav>
    <a href="#home">Home</a>
    <a href="#skills">Skills</a>
    <a href="#form">Contact</a>
</nav>

<!-- HOME / PROFILE -->
<section id="home" class="profile">
    <h2>My Profile</h2>

    <!-- CLICKABLE IMAGE -->
    <a href="https://www.google.com" target="_blank">
   <img src="img_girl.jpg" alt="boy in a jacket">



    <p>Hello! Ako si spencer barredo, student learning web development. Gusto ko maging magaling na website balang araw .</p>

    <a href="#form" class="btn">Contact Me</a>
</section>

<!-- SKILLS TABLE -->
<section id="skills">
    <h2>My Skills</h2>

    <table>
        <tr>
            <th>Skill</th>
            <th>Level</th>
        </tr>
        <tr>
            <td>HTML</td>
            <td>Intermediate</td>
        </tr>
        <tr>
            <td>CSS</td>
            <td>Beginner</td>
        </tr>
        <tr>
            <td>Design</td>
            <td>Basic</td>
        </tr>
    </table>
</section>

<!-- FORM WITH VALIDATION -->
<section id="form">
    <h2>Contact Me</h2>
<form action="/action_page.php">


<label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="barredo"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="spencer"><br><br>
   <label for="birthdate">Birth Date:</label><br>


<input type="date" id="birthdate" name="birthdate" value="2003-10-06"><br><br>
  <label for="email">Email:</label><br>
  <input type="email" name="email" value="spencerbarredo@gmail.com"><br><br>



<label for="password">Password:</label><br>
<input type="password" id="password" name="password" value="1102003"><br><br>
  


<input type="submit" value="Submit">
  
  


</form> 

<p>If you click the "Submit" button, the form-data will be sent to a page called "/action_page.php".</p>

</body>
</html>
