<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My GitHub Portfolio</title>
</head>
<body>
  <h1>My Portfolio</h1>
  
  <!-- Project 1 -->
  <div style="position: relative; width: 200px; height: 200px; background-color: black; display: inline-block; margin: 10px;">
    <a href="https://github.com/your-username/project1" target="_blank">
      <img src="project1-image.jpg" alt="Project 1" 
           style="width: 100%; height: 100%; position: absolute; top: 0; left: 0; opacity: 0; transition: opacity 0.5s;">
    </a>
  </div>
  
  <!-- Project 2 -->
  <div style="position: relative; width: 200px; height: 200px; background-color: black; display: inline-block; margin: 10px;">
    <a href="https://github.com/your-username/project2" target="_blank">
      <img src="project2-image.jpg" alt="Project 2" 
           style="width: 100%; height: 100%; position: absolute; top: 0; left: 0; opacity: 0; transition: opacity 0.5s;">
    </a>
  </div>

  <!-- Add more projects as needed -->

  <script>
    // JavaScript to reveal image on hover
    document.querySelectorAll('div').forEach(div => {
      div.addEventListener('mouseover', () => {
        div.querySelector('img').style.opacity = '1';
      });
      div.addEventListener('mouseout', () => {
        div.querySelector('img').style.opacity = '0';
      });
    });
  </script>
</body>
</html>
