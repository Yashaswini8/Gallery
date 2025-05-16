# Ex.08 Design of Interactive Image Gallery
## Name: Yashaswini.S
## Register Number:212224220123
# Date:16.05.2025
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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ART GALLERY</title>
    <style>
        body {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-image: url("imagegallery.jpg");
            background-size: cover;  
            background-position: center;
            background-attachment: fixed;   
            background-repeat: no-repeat;
        }

        h1 {
            margin-top: 20px;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 350px;
            height: 250px;
            border: 6px solid #000000;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid rgb(1, 1, 1);
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1><u>ART GALLERY</u></h1>
    <div class="gallery">
        <img src="eiffel.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="tajmahal.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="roman.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="boating.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="mountains.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="opera house.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="bridge.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="bali.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="city.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="waterfalls.jpg" alt="Image 5" onclick="openModal(this)">
    </div>

    <!-- Modal for displaying larger image -->
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <footer>
      &copy; 2024 designed by Yashaswini . All Rights Reserved.
    </footer>

    <script>
        // Function to open the modal and display the clicked image
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>
```
# OUTPUT:

![Screenshot 2025-05-13 190426](https://github.com/user-attachments/assets/d06b2a08-85a6-45e2-8980-12b730566247)

![Screenshot 2025-05-13 190457](https://github.com/user-attachments/assets/a5a4ad3c-0e0c-49b1-834c-8b0725b93d7b)

![Screenshot 2025-05-13 194221](https://github.com/user-attachments/assets/e6e5074e-d2de-40cd-bb7a-1e04652ebde5)

![Screenshot 2025-05-13 194428](https://github.com/user-attachments/assets/89a296ea-433c-4b1b-ab33-0723c948b3bf)

![Screenshot 2025-05-13 194428](https://github.com/user-attachments/assets/ec4a16b8-1632-452a-832e-938827add781)



# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
