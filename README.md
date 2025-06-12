<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Pleez Pleez Mac and Cheese</title>
  <style>
    body {
      margin: 0;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: #ffeb3b;
      background-image: radial-gradient(circle at 20% 30%, #fbc02d 10%, transparent 11%),
                        radial-gradient(circle at 80% 70%, #fbc02d 8%, transparent 9%),
                        radial-gradient(circle at 50% 50%, #fbc02d 12%, transparent 13%);
      background-size: 200px 200px;
      background-repeat: repeat;
      text-align: center;
    }

    header {
      padding: 2rem;
      font-size: 3rem;
      color: #fff;
      background-color: #f57f17;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    }

    button {
      margin: 2rem auto;
      padding: 1rem 2rem;
      font-size: 1.2rem;
      border: none;
      background-color: #ff9800;
      color: #fff;
      cursor: pointer;
      border-radius: 10px;
      box-shadow: 2px 4px 8px rgba(0,0,0,0.2);
      transition: background 0.3s;
    }

    button:hover {
      background-color: #fb8c00;
    }

    #menuImage {
      display: none;
      max-width: 90%;
      margin: 2rem auto;
      border-radius: 15px;
      box-shadow: 0 4px 16px rgba(0,0,0,0.4);
    }
  </style>
</head>
<body>

  <header>Pleez Pleez Mac and Cheese</header>

  <button onclick="toggleMenu()">Show Menu</button>

  <img id="menuImage" src="menu.png" alt="Pleez Pleez Menu">

  <script>
    const menu = document.getElementById('menuImage');
    const button = document.querySelector('button');

    function toggleMenu() {
      if (menu.style.display === 'none' || menu.style.display === '') {
        menu.style.display = 'block';
        button.textContent = 'Hide Menu';
      } else {
        menu.style.display = 'none';
        button.textContent = 'Show Menu';
      }
    }
  </script>

</body>
</html>
