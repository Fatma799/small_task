<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Space Adventure - Explore the Universe!</title>

  <style>
    
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }


    body {
      margin-top: 300px;
      font-family: 'Arial', sans-serif;
      background-color: #1e1e2f; 
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      height: 100vh;
      text-align: center;
      overflow-x: hidden;
    }


    .space-container {
      background-color: #2e2e45;
      border-radius: 15px;
      padding: 30px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      width: 90%;
      max-width: 1000px;
      border: 3px solid #ffcc00; 
      animation: slideIn 1s ease-out;
    }

    header {
      margin-bottom: 20px;
    }

    h1 {
      color: #ffcc00; 
      font-size: 2.5rem;
      animation: fadeIn 1.5s ease-out;
    }

    p {
      font-size: 1.2rem;
      color: #dcdcdc;
      animation: fadeIn 2s ease-out;
    }

    .planets {
      display: flex;
      justify-content: space-around;
      margin-top: 20px;
      flex-wrap: wrap; 
    }

    .planet {
      background-color: #3e3e5c;
      padding: 15px;
      border-radius: 10px;
      width: 150px;
      text-align: center;
      transition: transform 0.3s ease-in-out;
      animation: planetFadeIn 2s ease-in-out;
      margin: 10px;
    }

    .planet video {
      width: 100%;
      height: auto;
      border-radius: 10px;
      margin-bottom: 10px;
    }

    .planet:hover {
      transform: scale(1.1);
      background-color: #ff6347;
    }

    h3 {
      color: #ffcc00;
      font-size: 1.5rem;
    }

    .fun-facts {
      margin-top: 30px;
      background-color: #3e3e5c;
      padding: 20px;
      border-radius: 10px;
      animation: fadeIn 2s ease-out;
    }

    ul {
      list-style-type: none;
      font-size: 1.2rem;
      color: #dcdcdc;
      padding-left: 0;
    }

    .explore-more {
      margin-top: 30px;
    }

    .explore-more .btn {
      background-color: #ffcc00;
      padding: 12px 25px;
      font-size: 1.3rem;
      color: #333;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
      display: inline-block;
    }

    .explore-more .btn:hover {
      background-color: #ff6347;
    }

    footer button {
      background-color: #ff6347;
      color: white;
      border: none;
      padding: 12px 25px;
      font-size: 1.2rem;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 20px;
      transition: background-color 0.3s;
    }

    footer button:hover {
      background-color: #ff4500;
    }

    .logo {
      margin-top: 40px;
      padding: 10px;
    }

    .logo img {
      width: 150px;
      height: auto;
      animation: logoAnimation 2s ease-out;
    }

    @keyframes fadeIn {
      0% {
        opacity: 0;
        transform: translateY(-20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes slideIn {
      0% {
        opacity: 0;
        transform: translateX(-100%);
      }
      100% {
        opacity: 1;
        transform: translateX(0);
      }
    }

    @keyframes planetFadeIn {
      0% {
        opacity: 0;
        transform: scale(0.8);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }

    @keyframes logoAnimation {
      0% {
        opacity: 0;
        transform: scale(0.5);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }

    @keyframes fadeInUp {
      0% {
        opacity: 0;
        transform: translateY(20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body>
  <div class="space-container">
    <header>
      <h1>Welcome to the Space Adventure!</h1>
      <p>Let's explore the stars, planets, and galaxies together!</p>
    </header>

    <section class="planets">
      <h2>Meet the Planets</h2>
      <div class="planet" id="mercury">
        <h3>Mercury</h3>
        <video class="planet" controls>
          <source src="0_Planet_Mercury_3840x2160.mp4">
        </video>
        <p>Mercury is the closest planet to the Sun!</p>
      </div>
      <div class="planet" id="venus">
        <h3>Venus</h3>
        <video class="planet" controls>
          <source src="0_Planet_Saturn_3840x2160.mp4">
        </video>
        <p>Venus is known for its thick clouds and extreme temperatures!</p>
      </div>
      <div class="planet" id="earth">
        <h3>Earth</h3>
        <video class="planet" controls>
          <source src="0_Earth_Planet_3840x2160.mp4">
        </video>
        <p>Earth is the only planet known to support life!</p>
      </div>
      <div class="planet" id="mars">
        <h3>Mars</h3>
        <video class="planet" controls>
          <source src="0_Mars_Planet_3840x2160.mp4">
        </video>
        <p>Mars is also called the Red Planet because of its color!</p>
      </div>
    </section>

    <section class="fun-facts">
      <h2>Fun Space Facts</h2>
      <ul>
        <li>The Sun is 99.86% of the mass in our solar system!</li>
        <li>There are more stars in the universe than grains of sand on all the Earth’s beaches!</li>
        <li>One day on Venus is longer than one year on Venus!</li>
      </ul>
    </section>

    <section class="explore-more">
      <h2>Want to Learn More?</h2>
      <a href="https://www.nasa.gov" target="_blank" class="btn">Visit NASA's Website</a>
    </section>

    <section class="space-exploration">
      <h2>Space Exploration</h2>
      <p>Explore the infinite wonders of the universe, and unlock the secrets of black holes, nebulae, and distant galaxies. Join the mission to discover more!</p>
    </section>

    <div class="logo">
      <img src="WhatsApp Image 2025-01-24 at 20.49.54_75196b71.jpg" alt="Logo"> 
    </div>

    <footer>
      <button class="btn">Launch Your Rocket!</button>
      <button class="btn">Visit the Moon</button>
    </footer>
  </div>
</body>
</html>
