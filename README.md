<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Barza - Hear Their Cries</title>
  <style>
    body {
      background-color: black;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    .video-container {
      position: relative;
      text-align: center;
    }

    video {
      width: 100%;
      height: auto;
      object-fit: cover;
    }

    .overlay-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: orange;
      font-size: 2rem;
      font-weight: bold;
      animation: fadeInOut 3s infinite;
    }

    @keyframes fadeInOut {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.5; }
    }

    .links {
      text-align: center;
      margin: 20px 0;
    }

    .link-button {
      display: inline-block;
      margin: 10px;
      padding: 10px 20px;
      background-color: orange;
      color: black;
      text-decoration: none;
      font-weight: bold;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    .link-button:hover {
      background-color: darkorange;
    }

    .awareness {
      margin: 20px;
      text-align: center;
      font-size: 1.2rem;
      color: orange;
    }
  </style>
</head>
<body>
  <div class="video-container">
    <video autoplay loop controls>
      <source src="path-to-your-video.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <div class="overlay-text">Hear Their Cries</div>
  </div>
  
  <div class="links">
    <a href="https://matwprojectusa.org/appeals/limbs-of-hope" class="link-button">Donate</a>
    <a href="https://www.aljazeera.com/tag/gaza/" class="link-button">Live Updates</a>
    <a href="https://www.aljazeera.com/program/newsfeed/2024/10/7/the-names-of-those-killed-in-israels-genocide-in-gaza" class="link-button">Victims' Names</a>
  </div>

  <div class="awareness">
    You can help for free by sharing this website and raising awareness.
  </div>
</body>
</html>
