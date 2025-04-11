<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Image Carousel</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f7f7f7;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .carousel-container {
      background: white;
      border: 1px solid #ccc;
      border-radius: 10px;
      overflow: hidden;
      width: 90%;
      max-width: 500px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      text-align: center;
      position: relative;
    }

    .carousel-image {
      width: 100%;
      display: none;
    }

    .carousel-image.active {
      display: block;
    }

    .carousel-heading {
      font-size: 1.5rem;
      margin: 1rem 0;
    }

    .arrow {
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      font-size: 2rem;
      color: #333;
      background-color: rgba(255,255,255,0.7);
      border: none;
      cursor: pointer;
      padding: 0.5rem 1rem;
      z-index: 1;
    }

    .arrow:hover {
      background-color: rgba(200,200,200,0.8);
    }

    .arrow.left {
      left: 0;
    }

    .arrow.right {
      right: 0;
    }
  </style>
</head>
<body>
  <div class="carousel-container">
    <button class="arrow left" onclick="prevSlide()">❮</button>
    <div class="carousel-heading" id="carousel-heading">Home</div>
    <img class="carousel-image active" src="https://github.com/user-attachments/assets/42aaefe3-520f-4875-8d39-d2a41af3488a" alt="Home">
    <img class="carousel-image" src="https://github.com/user-attachments/assets/d0183cc7-eebc-4017-a499-e299bea7f89c" alt="Login">
    <img class="carousel-image" src="https://github.com/user-attachments/assets/d49f9a8a-49eb-4442-bc75-4abda64699ca" alt="Sign Up">
    <img class="carousel-image" src="https://github.com/user-attachments/assets/11c7f5e3-1555-4ff9-992f-3a1840c6aaca" alt="Verification">
    <button class="arrow right" onclick="nextSlide()">❯</button>
  </div>

  <script>
    const headings = ["Home", "Login", "Sign Up", "Verification"];
    let currentIndex = 0;
    const images = document.querySelectorAll(".carousel-image");
    const heading = document.getElementById("carousel-heading");

    function showSlide(index) {
      images.forEach((img, i) => {
        img.classList.toggle("active", i === index);
      });
      heading.textContent = headings[index];
    }

    function prevSlide() {
      currentIndex = (currentIndex - 1 + images.length) % images.length;
      showSlide(currentIndex);
    }

    function nextSlide() {
      currentIndex = (currentIndex + 1) % images.length;
      showSlide(currentIndex);
    }
  </script>
</body>
</html>
