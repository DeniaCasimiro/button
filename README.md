# button

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Menu Button</title>
  <style>
    .menu-container {
      position: relative;
      display: inline-block;
    }

    .menu-btn {
      background: white;
      color: black;
      border: 1px solid black;
      border-radius: 50%;
      padding: 30px 55px;
      cursor: pointer;
    }

    .menu-tabs {
      display: none;
      position: absolute;
      top: 100%;
      left: 50%;
      transform: translateX(-50%);
      background: white;
      border: 1px solid black;
      border-radius: 10px;
      overflow: hidden;
    }

    .menu-tabs div {
      padding: 8px 20px;
      cursor: pointer;
    }

    .menu-tabs div:hover {
      background: #f0f0f0;
    }

    .menu-container:hover .menu-tabs {
      display: block;
      animation: slideDown 0.3s ease;
    }

    @keyframes slideDown {
      from { opacity: 0; transform: translate(-50%, -10px); }
      to { opacity: 1; transform: translate(-50%, 0); }
    }
  </style>
</head>
<body>
  <div class="menu-container">
    <button class="menu-btn">Menu</button>
    <div class="menu-tabs">
      <div>Name 1</div>
      <div>Name 2</div>
      <div>Name 3</div>
    </div>
  </div>
</body>
</html>
