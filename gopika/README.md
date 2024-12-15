Ex.07 Restaurant Website
Date:
AIM:
To develop a static Restaurant website to display the food items and services provided by them.

DESIGN STEPS:
Step 1:
Requirement collection.

Step 2:
Creating the layout using HTML and CSS.

Step 3:
Updating the sample content.

Step 4:
Choose the appropriate style and color scheme.

Step 5:
Validate the layout in various browsers.

Step 6:
Validate the HTML code.

Step 7:
Publish the website in the given URL.

PROGRAM:
```
rest.html

<!DOCTYPE html>
<html lang="en"?>
    <head>
        <title>TASTY DINE</title>
        <link rel="icon" href="logo.jpg">
    </head>
    <style>
        body{
            background-image: url(back1.webp);
            background-size: cover;
            background-position: center;
        }
        .nav-list{
            position: absolute;
            top: 30px;
            left: 80%;
            transform:  translatex(10%);
        }
        .nav-list a{
            display: inline blocks;
            margin: 0 10px;
            font-family:MS Sans Serif;
            text-decoration: none;
            font-size: 18px;
            font-weight: bold;
            color: white;
        }
        .nav-list a:hover{
            color: rgb(235, 9, 149);
        }
    </style>
        <div class="nav-list">
        
        <a href="rest.html">Home</a>
        <a href="contact.html">contact</a>
        <a href="order.html">menu</a>
        <a href="admin.html">Administration</a>

        </div>
    <body style="color: white;">
        <center>
        <img src="logo.jpg" style="height: 150px;">
        </center>
        <center>
            <h1 style="color: green; font-size: 50px;">TASTE DINE</h1>
    <table> 
        <center>
        <tr>
            <td><img src="burger.jpg" style="width: 300px; height: 250px;"></td>
            <td><img src="Dosai.jpg" style="width:300px; height: 250px;"></td>
            <td><img src="puri.jpg" style="width:300px; height: 250px;"></td>
            <td><img src="parotta.jpg" style="width:300px; height: 250px;"></td>
            <td><img src="panipuri.webp" style="width:300px; height: 250px;"></td>
        </tr>
        </center>
        <tr>
            <td><h3 style="color:rgb(235, 9, 149);"><center>BURGER</center></h3></td>
            <td><h3 style="color:rgb(235, 9, 149);"><center>DOSAI </center></h3></td>
            <td><h3 style="color: rgb(235, 9, 149);"><center>PURI</center></h3></td>
            <td><h3 style="color: rgb(235, 9, 149)"><center>PAROTTA</center></h3></td>
            <td><h3 style="color:rgb(235, 9, 149)"><center>PANIPURI</center></h3></td>
        </tr>
    </table>
    <h2>OUR specialities:   
    </h2>
        <p style="font-family: 'Times New Roman',Times, serif";><center>
            Speciality restaurants offer a fine dining experience wherein guests can enjoy their meals cooked to perfection by master chef's in a live kitchen. The authentic décor and warm and personalized service is an experience to cherish.
        People don't just go to restaurants for the food; they go for the experience. Talk about the overall experience your restaurant offers, from the service to the atmosphere. For example: "Our friendly staff and warm, inviting atmosphere make every meal feel like a special occasion."        
        </p> 
        <hr>
        <tr>
            <td><h4 style="font-size: larger;"><center>THE BEST PLACE TO EXPERIENCE THE REAL TASTE!</center></h4></td>
        </tr>
    </body>        
</html>

contact.html

<html>
    <head>
        <title> CONTACT </title>
    </head>
    <style>
        
        body{
        
            background-image: url(back1.webp);
            background-size: cover;
            background-position: center;
        }
        body{
            display: inline blocks;
            padding-left: 500px;
            font-family:MS Sans Serif;
            text-decoration: none;
            font-size: 23px;
            font-weight: bolder;
            color: rgb(217, 231, 239);
            position:absolute;
            top: 200px;
        }
    </style>

        
        <a href="rest.html">HOME</a>
        <a href="contact.html">CONTACT</a>
        <a href="order.html">MENU</a>
        <a href="admin.html">ADMINISTRATION</a>


    <center>
        <section id="contact">  
            <h1 style="color:#0ffbff">contact<h1>
            <h4  style="color:#00f2ff">+91 6987230465<br> | tastydine@gmail.com</h4>
            <P  style="color:#0479ff">Address: no.39 T Nagnar, chennai. <br>
                <br> contact us to place the order<br>
            <hr> THE PLACE WHERE YOU FIND THE REAL TASTE
            </P>
         </section> 
    </center>
    </body>
</html>


admin.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ADMIN</title>

    <style>
        body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            color: #070c31;
            background-color: #f63a3a;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #a7cb27;
            color: rgb(136, 69, 199);
            padding: 15px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(1, 33, 15, 0.1);
        }

        header h1 {
            font-size: 1.8rem;
            font-family: 'Playfair Display', serif;
        }

        header nav a {
            text-decoration: none;
            color: rgb(30, 134, 225);
            font-weight: 500;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1rem;
        }

        header nav a:hover {
            color: #8b2a83;
        }

        .admin-container {
            padding: 40px 20px;
            background: #1daac6;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 2.5rem;
            color: #674f31;
            margin-bottom: 20px;
            font-family: 'Playfair Display', serif;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .admin-item {
            background: rgb(180, 185, 153);
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(159, 154, 149, 0.1);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease;
            text-align: left;
        }

        .admin-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }

        .admin-item:hover {
            transform: scale(1.05);
        }

        .admin-details {
            padding: 15px;
        }

        .admin-details h3 {
            font-size: 1.4rem;
            color: #2c3e50;
            margin-bottom: 8px;
        }

        .admin-details p {
            font-size: 1rem;
            color: #555;
            margin-bottom: 10px;
        }

        footer {
            background: #978b5a;
            color: rgb(123, 154, 169);
            text-align: center;
            padding: 15px 0;
        }

        footer a {
            color: #dba419;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ecf0f1;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }

            header nav a {
                font-size: 0.9rem;
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>    

<header>
        <h1>TASTY DINE</h1>
        <nav>
            <a href="rest.html">Home</a>
            <a href="order.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="admin-container">
        <h1> OUR SUPPORTER'S</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="chef 1.jpg" alt="CEO">
                <div class="admin-details">
                    <h3>Trisha</h3>
                    <p>CEO </p>
                </div>
            </div>

            <div class="admin-item">
                <img src="chef 2.jpg" alt="Manager">
                <div class="admin-details">
                    <h3>Vijay</h3>
                    <p>Manager</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="chef 3.jpg" alt="Master Chef">
                <div class="admin-details">
                    <h3>Sivakarthikeyan</h3>
                    <p>Master Chef </p>
                </div>
            </div>

            <div class="admin-item">
                <img src="chef 4.jpg" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Agarwal</h3>
                    <p>Assistant Managing Director</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="chef 5.jpg" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Samantha </h3>
                    <p>Assistant Managing Director </p>
                </div>
            </div>

        </div>
    </div>

    <footer>
        <p>&copy; 2024 TASTY DINE. All rights reserved. | <a href="rest.html">Back to Home</a></p>
    </footer>

</body>
</html>





```
OUTPUT:
![alt text](<Screenshot (33).png>)
![alt text](<Screenshot (34).png>)
![alt text](<Screenshot (35).png>)
![alt text](<Screenshot (36).png>)



RESULT:
The program for designing software company website using HTML and CSS is completed successfully.