<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>DP Portfolio</title>
  <style>
    body{
        font-family: Times New Roman, Arial;
        text-align: center;
    }

  </style>
</head>
<body>
<h1>Dave Pierre</h1>
<p><a href="mailto:davepierred@yahoo.com">davepierred@yahoo.com</a></p>

<a href="cartoon.html">View Masterpiece</a>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Cartoon</title>
    <style>
    body {
        font-family: Times New Roman
        text-align: center;
        background-color: blue;
    }
    canvas {
        border: 5px solid purple;
        margin: 15px auto;
        background-color: #add8e6;
    }
    a {
        display: block;
        margin-top: 20px;
        text-decoration: none;
        color: black; /* Set link color to black */
        text-decoration: none; /* Remove underline */
        }
</style>
</head>
<body>
<h1>Cartoon 1of1 </h1>

<canvas id="myCanvas" width="600" height="400"></canvas>

<script>
var caption = "Cartoon Mania";
var canvas = document.getElementById('myCanvas');
var cantoon= canvas.getContext('2d');

// Draw caption text
cantoon.fillStyle = 'white';
cantoon.font = '28px Times New Roman';
cantoon.fillText(caption, 40, 65);

// Draw sun
cantoon.beginPath();
cantoon.arc(550, 110, 30, 0, Math.PI * 2);
cantoon.fillStyle = 'yellow';
cantoon.fill();

// Draw mountains
cantoon.fillStyle = 'grey';
cantoon.beginPath();
cantoon.moveTo(0, 250);
cantoon.lineTo(100, 90);
cantoon.lineTo(300, 250);
cantoon.lineTo(450, 150);
cantoon.lineTo(600, 250);
cantoon.fill();

// Draw ground
cantoon.fillStyle = '#8B4513';
cantoon.fillRect(0, 250, canvas.width, canvas.height - 250);


// house 1
cantoon.fillStyle = 'purple';
cantoon.fillRect(100, 180, 100, 70);

// Draw windows
cantoon.fillStyle = 'white';
cantoon.fillRect(110, 195, 30, 30);
cantoon.fillRect(160, 195, 30, 30);
// Draw door
cantoon.fillStyle = 'black'; // brown
cantoon.fillRect(140, 230, 20, 20);
// house 2
cantoon.fillStyle = 'blue'; // House color
cantoon.fillRect(250, 160, 90, 90); // Main body
cantoon.fillStyle = 'white'; // Window color
cantoon.fillRect(260, 165, 30, 30); // Window 1
cantoon.fillRect(300, 165, 30, 30); // Window 2
cantoon.fillStyle = 'brown'; // Door color
cantoon.fillRect(280, 210, 30, 40); // Door
// Draw grass
cantoon.fillStyle = 'green';
for (let i = 0; i < canvas.width; i += 20) {
    cantoon.fillRect(i, 255, 20, 80);
}
// draw fence
cantoon.fillStyle = 'black';
for (let i = 0; i < canvas.width; i += 20) {
    cantoon.fillRect(i, 315, 10, 80);
}
</script>
<a href="canvass.html">Back to Portfolio</a>


</body>
</html>
