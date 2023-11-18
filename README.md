# webpro2
webpro2
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Image Gallery</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f4f4f4;
    }

    .gallery {
      max-width: 600px;
      text-align: center;
    }

    .thumbnails img {
      width: 100px;
      height: 75px;
      margin: 5px;
      cursor: pointer;
    }

    .main-image {
      max-width: 100%;
      border: 2px solid #333;
    }
  </style>
</head>
<body>

<div class="gallery">
  <div class="thumbnails">
    <img src="image1.jpg" onclick="showImage('image1.jpg')" alt="Image 1">
    <img src="image2.jpg" onclick="showImage('image2.jpg')" alt="Image 2">
    <img src="image3.jpg" onclick="showImage('image3.jpg')" alt="Image 3">
    <!-- Add more images as needed -->
  </div>

  <img class="main-image" src="image1.jpg" alt="Main Image">

  <script>
    function showImage(imageUrl) {
      document.querySelector('.main-image').src = imageUrl;
    }
  </script>
</div>

</body>
</html>
