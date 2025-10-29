Step 1:
Create a folder — example: admin-dashboard.

Step 2:
Inside the folder, create a new file named index.html.

Step 3:
Open index.html in any text editor (like VS Code or Notepad).

Step 4:
Type the basic HTML structure:

<!DOCTYPE html>
<html>
<head>
  <title>Admin Dashboard</title>
</head>
<body>
</body>
</html>

Step 5:
Add a heading inside the <body> tag:

<h1>Admin Dashboard</h1>

Step 6:
Create a space for the chart:

<canvas id="myChart"></canvas>

Step 7:
Add the Chart.js library (a tool for making charts) before the end of </body>:

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

Step 8:
Add a simple chart script:

<script>
const ctx = document.getElementById('myChart');
new Chart(ctx, {
  type: 'bar',
  data: {
    labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May'],
    datasets: [{
      label: 'Sales ($)',
      data: [1200, 1900, 3000, 2500, 3200],
      backgroundColor: 'skyblue'
    }]
  }
});
</script>

Step 9:
Add a little style for a clean look:

<style>
body {
  text-align: center;
  font-family: Arial;
  background-color: #f0f0f0;
}
canvas {
  width: 80%;
  max-width: 600px;
  margin-top: 20px;
}
</style>

Step 10

Save the file and double-click it —
 Your simple Admin Dashboard with a chart will open in the browser!
