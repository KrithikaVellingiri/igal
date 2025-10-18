# Ex.08 Design of Interactive Image Gallery
## Date:09.10.2025

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

index.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Krithika V 25017985 - Image Gallery</title>


  <link rel="stylesheet" href="style.css">
</head>

<body>
  <h1>Krithika V 25017985</h1>

  <div class="gallery">
    <div class="gallery-item"><img src="b.jpeg" alt="Image 1"></div>
    <div class="gallery-item"><img src="che.jpg" alt="Image 2"></div>
    <div class="gallery-item"><img src="r.jpeg" alt="Image 3"></div>
    <div class="gallery-item"><img src="s.jpeg" alt="Image 4"></div>
    <div class="gallery-item"><img src="v.jpeg" alt="Image 5"></div>
  </div>

  <footer>© 2025 Image Gallery</footer>


  <script src="script.js"></script>
</body>
</html>

style.css

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: red;
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  margin-top: 30px;
  color: white;
  font-size: 28px;
  text-align: center;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 15px;
  width: 80%;
  max-width: 1000px;
  margin: 30px auto;
}

.gallery-item {
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease;
}

.gallery-item img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.gallery-item:hover img {
  transform: scale(1.1);
}

footer {
  margin: 30px;
  font-size: 14px;
  color: #555;
}

sty.js


console.log("Script loaded successfully!");

window.addEventListener("load", () => {
  const galleryItems = document.querySelectorAll(".gallery-item");
  galleryItems.forEach((item, index) => {
    item.style.opacity = "0";
    item.style.transform = "translateY(20px)";
    setTimeout(() => {
      item.style.transition = "all 0.5s ease";
      item.style.opacity = "1";
      item.style.transform = "translateY(0)";
    }, 150 * index);
  });
});
```
## OUTPUT:
![alt text](<Screenshot (836).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
