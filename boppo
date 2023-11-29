<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Resizable Button</title>
  <style>
    #resizableButton {
      font-size: 16px;
      padding: 10px;
      transition: all 0.3s;
    }
  </style>
</head>
<body>

<button id="resizableButton" onclick="increaseSize()">Click me!</button>

<script>
  let clickCount = 0;

  function increaseSize() {
    clickCount++;
    const button = document.getElementById('resizableButton');
    const newSize = 16 + clickCount * 2; // You can adjust the rate of increase here
    button.style.fontSize = newSize + 'px';
    button.style.padding = (10 + clickCount) + 'px'; // Adjust padding as well for visual effect
  }
</script>

</body>
</html>
