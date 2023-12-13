<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Car Color Selector</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
    }

    .car-options {
      display: flex;
      gap: 10px;
      align-items: center;
      justify-content: center;
    }

    .car-option {
      cursor: pointer;
      position: relative;
    }

    .car-icon {
      width: 50px;
      height: 50px;
      border-radius: 50%;
    }

    .car-name {
      position: absolute;
      bottom: -20px;
      left: 50%;
      transform: translateX(-50%);
    }

    #car-image {
      width: 300px;
      height: 200px;
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <h1>ASSERT YOUR STYLE</h1>
  <h2>從七種頂級車色中選擇適合您的顏色</h2>

  <div class="car-options">
    <div class="car-option" onclick="changeOption('Black')">
      <img src="Black_car_image.jpg" alt="Black Car" class="car-icon">
      <span class="car-name">Black</span>
    </div>
    <div class="car-option" onclick="changeOption('White')">
      <img src="White_car_image.jpg" alt="White Car" class="car-icon">
      <span class="car-name">White</span>
    </div>
    <div class="car-option" onclick="changeOption('Gray')">
      <img src="Gray_car_image.jpg" alt="Gray Car" class="car-icon">
      <span class="car-name">Gray</span>
    </div>
    <div class="car-option" onclick="changeOption('Silver')">
      <img src="Silver_car_image.jpg" alt="Silver Car" class="car-icon">
      <span class="car-name">Silver</span>
    </div>
    <div class="car-option" onclick="changeOption('Red')">
      <img src="Red_car_image.jpg" alt="Red Car" class="car-icon">
      <span class="car-name">Red</span>
    </div>
    <div class="car-option" onclick="changeOption('Blue')">
      <img src="Blue_car_image.jpg" alt="Blue Car" class="car-icon">
      <span class="car-name">Blue</span>
    </div>
    <div class="car-option" onclick="changeOption('Orange')">
      <img src="Orange_car_image.jpg" alt="Orange Car" class="car-icon">
      <span class="car-name">Orange</span>
    </div>
    <!-- Add more options as needed -->
  </div>

  <div id="car-image">
    <img src="Black_car_image.jpg" alt="Default Car" style="width: 100%; height: 100%; object-fit: cover;">
  </div>

  <script>
    function changeOption(option) {
      var carImage = document.getElementById('car-image');
      carImage.innerHTML = `<img src="${option}_car_image.jpg" alt="${option} Car" style="width: 100%; height: 100%; object-fit: cover;">`;
    }
  </script>

</body>
</html>
