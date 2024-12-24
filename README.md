# Ex.08 Design of Interactive Image Gallery
## Date:
24.12.24
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
<html>
    <title>My Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 0;
            background-size: cover;
            background-image: url('home2.jpg');
            padding: 20px;
            min-height: 100vh;
            position: relative;
        }

        h1 {
            margin-top: 20px;
            color: rgb(227, 225, 225);
            font-size: xx-large;
            font-weight: bold;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            max-width: 800px;
            width: 100%;
            margin-top: 20px;
        }

        .photo {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            cursor: pointer;
        }

        .photo img {
            width: 150px;
            height: auto;
            border-radius: 8px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .photo img:hover {
            transform: scale(1.2);
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5);
        }

        .photo p {
            margin-top: 5px;
            font-size: 14px;
            color: #333;
        }

        footer {
            position: absolute;
            bottom: 0;
            width: 100%;
            text-align: center;
            background-color: rgba(0, 0, 0, 0.7);
            color: #fff;
            padding: 10px 0;
            font-size: 14px;
        }
    </style>

    <body>
        <h1>My IMAGE GALLERY</h1>
        <div class="gallery">
            <div class="photo" onclick="openImage('p.jpg')">
                <img src="p.jpg" alt="Paris">
                <p>Paris</p>
            </div>
            <div class="photo" onclick="openImage('n.jpg')">
                <img src="n.jpg" alt="Northern_lights">
                <p>Northern Lights</p>
            </div>
            <div class="photo" onclick="openImage('b.jpg')">
                <img src="p.jpg" alt="Birds">
                <p>Birds</p>
            </div>
            <div class="photo" onclick="openImage('c.jpg')">
                <img src="c.jpg" alt="Car">
                <p>Car</p>
            </div>
            <div class="photo" onclick="openImage('m.jpg')">
                <img src="m.jpg" alt="Mountain">
                <p>Mountain</p>
            </div>
            <div class="photo" onclick="openImage('be.jpg')">
                <img src="be.jpg" alt="Beach">
                <p>Beach</p>
            </div>
            <div class="photo" onclick="openImage('cc.jpg')">
                <img src="cc.jpg" alt="Concert">
                <p>Concert</p>
            </div>
        </div>

        <footer>
            &copy; 2024 Designed and Developed by Madhu Shrie J.
        </footer>

        <script>
            function openImage(src) {
                const newWindow = window.open("", "_blank");
                newWindow.document.write(`
                    <html>
                        <head><title>Image Preview</title></head>
                        <body style="margin:0;display:flex;align-items:center;justify-content:center;height:100vh;background-color:#000;">
                            <img src="${src}" style="max-width:100%;max-height:100%;">
                        </body>
                    </html>
                `);
            }
        </script>
    </body>
</html>
```
## OUTPUT:
![alt text](<Screenshot (49).png>)
![alt text](<Screenshot (50).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
