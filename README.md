# Ex.08 Design of Interactive Image Gallery
# Date:16/11/2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<html>
    <head>
<style>
    body{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background: radial-gradient(red,rgb(11, 11, 11));
    }
    h1{
        margin: 50;
        font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        font-size: 70px;
    }
    .main{
        display: flex;
        flex-wrap: wrap;
        border: 2px solid black;
        border-radius: 40px;
        background: radial-gradient(rgb(244, 243, 243),blue);
        width: 70%;
        height: 70%;
        justify-content: center;
        align-items: center;
        margin: auto;
    }
    .n{
        
        border-radius: 20px;
        width: 27%;
        height: 30%;
        margin: auto;
        transition: transform 0.3s ease; 
        cursor: pointer;
    }
    .n:hover{
        transform: scale(1.1);
    }

    .f{
        display: flex;
        border-radius: 40px;
        position: relative;
        top: 0%;
        bottom: 50%;
        width: 940px;
        height: 528px;
    }
    .hidden {
        display: none;
    }
</style>

    </head>
    <title>SAVEETHA WEARS</title>
    <body >
        <h1 align="center">SAVEETHA WEARS</h1>
        <div class="main">
            <img src="shirt.jpeg" alt="SHIRT" class="n" id="ni">
            <img src="pant.jpeg" alt="PANT" class="n" id="ni">
            <img src="blazzer.jpeg" alt="BLAZZER" class="n" id="ni">
            <img src="tshirt.jpeg" alt="T-SHIRT" class="n" id="ni">
            <img src="track.jpeg" alt="TRACK PANT" class="n" id="ni">
            <img src="hoodie.jpeg" alt="HOODIE" class="n" id="ni">
        </div>
        <script type="text/javascript">
            const images = document.querySelectorAll('.n');
        
            images.forEach(function(img) {
                img.addEventListener("click", function() {
                    
                    images.forEach(function(image) {
                        if (image !== img) {
                            image.classList.add('hidden');
                        }
                    });
                    
                    img.classList.add('f');
                });
        
                img.addEventListener("dblclick", function() {
                    
                    images.forEach(function(image) {
                        image.classList.remove('hidden', 'f');
                    });
                });
            });
        </script>
    </body>
</html>
```
# OUTPUT:
![Screenshot 2024-12-15 222104](https://github.com/user-attachments/assets/fccd3f37-6dda-47f9-8c9c-89914a00a7fa)
![Screenshot 2024-12-15 222911](https://github.com/user-attachments/assets/d6018bda-934b-48f2-980c-fbb5c28e6a8b)

![Screenshot 2024-12-15 222043](https://github.com/user-attachments/assets/274b2afd-a3a5-489d-9776-649c35ae014f)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
