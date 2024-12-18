# Ex.08 Design of Interactive Image Gallery
## Date:
18.12.24
## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            margin: 0; 
            background-image: url('home2.jpg'); 
            background-size: cover; 
            background-repeat: no-repeat; 
            background-attachment: fixed; 
        }
        header { 
            background: rgba(105, 171, 93, 0.7); 
            color: white; 
            padding: 10px; 
            text-align: center; 
        }
        nav a { 
            color: white; 
            margin: 0 15px; 
            text-decoration: none; 
        }
        nav a:hover { 
            text-decoration: underline; 
        }
        main { 
            text-align: center; 
            padding: 20px; 
            background: rgba(104, 163, 98, 0.8); 
            margin: 50px auto;
            max-width: 600px;
            border-radius: 10px;
        }
        footer { 
            background: rgba(104, 147, 92, 0.7); 
            color: white; 
            text-align: center; 
            padding: 10px; 
            position: relative; 
            bottom: 0; 
            width: 100%; 
        }
        footer p { 
            margin: 5px 0; 
        }
        footer a { 
            color: lightblue; 
            text-decoration: none; 
        }
        footer a:hover { 
            text-decoration: underline; 
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contactus.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1>Welcome to My Photo Gallery</h1>
        <p>Experience the world through my eyes.</p>
    </main>
    <footer>
        <p>&copy; 2024 Designed and Developed by MADHU SHRIE J</p>
            </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            background-color: beige;
        }
        header {
            background: #4e9754;
            color: rgb(105, 190, 100);
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: rgb(246, 248, 246);
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            flex: 1; 
            padding: 20px;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            padding: 20px;
        }
        .photo {
            background: rgb(108, 180, 120);
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            width: 250px;
            text-align: center;
        }
        .photo img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .photo-title {
            font-size: 18px;
            font-weight: bold;
            margin: 10px 0;
        }
        .photo-description {
            font-size: 14px;
            color: #555;
            margin: 0 10px 10px;
        }
        footer {
            background: #60a563;
            color: white;
            text-align: center;
            padding: 10px;
            width: 100%;
        }
        footer a {
            color: rgb(102, 189, 98);
            text-decoration: none;
            margin: 0 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contactus.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1 style="text-align: center; margin: 20px 0;">PHOTO GALLARY</h1>
        <div class="gallery">
                <div class="photo">
                <img src="n.jpg" alt="n">
                <p>NORTHERN LIGHTS</p>
                </div>
                <div class="photo">
                <img src="b.jpg" alt="b">
                <p>BIRDS</p>
                </div>
                <div class="photo">
                <img src="be.jpg" alt="be">
                <p>BEACH</p>
                </div>
                <div class="photo">
                <img src="m.jpg" alt="m">
                <p>MOUNTAIN</p>
                </div>
                <div class="photo">
                <img src="cc.jpg" alt="cc">
                <p>CONCERT</p>
                </div>
                <div class="photo">
                <img src="c.jpg" alt="c">
                <p>CAR</p>
                </div>
                <div class="photo">
                <img src="p.jpg" alt="p">
                <p>PARIS</p>
                </div>

                        </div>
    </main>
    <footer>
       <p> &copy; 2024 Designed and Developed by MADHU SHRIE J</p>
    </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            background-color: beige;
        }
        header {
            background: #4fa25e;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            flex: 1; 
            padding: 20px;
            text-align: center;
        }
        main .content {
            max-width: 600px;
            margin: 0 auto;
            text-align: left;
        }
        footer {
            background: #569f53;
            color: white;
            text-align: center;
            padding: 10px;
            width: 100%;
        }
        footer a {
            color: rgb(236, 239, 240);
            text-decoration: none;
            margin: 0 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contactus.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1>About Us</h1>
        <div class="content">
            <p style="font-size: 24px;"> <b>Welcome to My Photo Gallery</b></p> 
            <p style="font-size: 20px;">This collection is a reflection of my journey through the lens, capturing moments that inspire, challenge, and move me. Each image tells a story — whether it's a fleeting moment in nature, a candid portrait, or an abstract view of the world. My goal is to transport you through visual storytelling, evoking emotions and sparking curiosity.</p>
            <p style="font-size: 20px;">Thank you for visiting and experiencing the world through my eyes.</p>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Designed and Developed by MADHU SHRIE J</p>
    </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            background-color: beige;
        }
        header {
            background: #4b994b;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            flex: 1; 
            padding: 20px;
            text-align: center;
        }
        main form {
            max-width: 500px;
            margin: 0 auto;
            text-align: left;
        }
        form label {
            display: block;
            margin-top: 10px;
            font-weight: bold;
        }
        form input, form textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 14px;
        }
        form button {
            margin-top: 15px;
            padding: 10px 20px;
            background: #faf4f4;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        form button:hover {
            background: #555;
        }
        footer {
            background: #68c35a;
            color: white;
            text-align: center;
            padding: 10px;
            width: 100%;
        }
        footer a {
            color: rgb(231, 236, 238);
            text-decoration: none;
            margin: 0 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contactus.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1>Contact Us</h1>
        <section class="contact me">
        <h2>keep in touch </h2>
        <p style="font-size: 20px;"><strong>Website Handeled By:</strong> MADHU SHRIE J</p>
        <p style="font-size: 20px;"><strong>Phone:</strong> 9443419387</p>
        <p style="font-size: 20px;"><strong>Email:</strong> imagegallery@gmail.com</p>
    </section>

            </main>
    <footer>
        <p>&copy; 2024  Designed and Developed by MADHU SHRIE J</p>  
 </footer>
</body>
</html>
```
## OUTPUT:
![alt text](<Screenshot (44).png>)
![alt text](<Screenshot (45).png>)
![alt text](<Screenshot (46).png>)
![alt text](<Screenshot (47).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
