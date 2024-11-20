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

    .sound-button {
      position: absolute;
      top: 90%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: orange;
      color: black;
      border: none;
      padding: 10px 20px;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      border-radius: 5px;
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
    <video id="video" autoplay loop muted>
      <source src="assets/videos/copy_BE49A0DC-82B3-4D83-8028-F6AED2B252F3.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <div class="overlay-text">Hear Their Cries</div>
    <button id="soundButton" class="sound-button">Enable Sound</button>
  </div>
  
  <div class="links">
    <a href="https://matwprojectusa.org/appeals/limbs-of-hope" class="link-button">Donate</a>
    <a href="https://www.aljazeera.com/tag/gaza/" class="link-button">Live Updates</a>
    <a href="https://www.aljazeera.com/program/newsfeed/2024/10/7/the-names-of-those-killed-in-israels-genocide-in-gaza" class="link-button">Victims' Names</a>
  </div>

  <div class="awareness">
    You can help for free by sharing this website and raising awareness.
  </div>
  <script>
    const video = document.getElementById('video');
    const soundButton = document.getElementById('soundButton');

    soundButton.addEventListener('click', () => {
      video.muted = false;
      video.play(); // Ensures video continues playing
      soundButton.style.display = 'none'; // Hide the button after enabling sound
    });
  </script>
</body>
</html>
