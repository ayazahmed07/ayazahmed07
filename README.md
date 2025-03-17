<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Ayaz Ahmed - GitHub Profile</title>
  <!-- Bootstrap CSS for modern styling -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" />
  <!-- Custom CSS -->
  <style>
    body {
      background-color: #f5f5f5;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    .profile-header {
      background: #fff;
      padding: 2rem;
      margin-bottom: 2rem;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      text-align: center;
    }
    .profile-header img {
      border-radius: 50%;
      width: 150px;
      border: 4px solid #007bff;
    }
    .profile-header h1 {
      margin-top: 1rem;
      font-size: 2.5rem;
      color: #333;
    }
    .profile-header p {
      font-size: 1.1rem;
      color: #555;
    }
    .pinned-projects h2,
    .chart-container h2 {
      margin-bottom: 1rem;
      color: #007bff;
    }
    .card {
      margin-bottom: 1rem;
    }
    .chart-container {
      background: #fff;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Profile Header -->
    <div class="profile-header">
      <img src="https://github.com/ayazahmed07.png" alt="Ayaz Ahmed" />
      <h1>Ayaz Ahmed</h1>
      <p>
        Hello! I’m Ayaz Ahmed. Currently learning TypeScript programming at the Governor Sindh Initiative of Artificial Intelligence.
      </p>
      <a href="https://github.com/ayazahmed07" target="_blank" class="btn btn-primary mt-3">
        Visit GitHub
      </a>
    </div>

    <!-- Pinned Projects Section -->
    <div class="pinned-projects">
      <h2>Pinned Projects</h2>
      <div class="row">
        <!-- ATM Project -->
        <div class="col-md-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title">ATM Project</h5>
              <p class="card-text">A project simulating ATM functionalities using JavaScript.</p>
              <a href="https://github.com/ayazahmed07/ATM" target="_blank" class="btn btn-outline-primary">View Project</a>
            </div>
          </div>
        </div>
        <!-- Currency Converter -->
        <div class="col-md-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title">CurConverter</h5>
              <p class="card-text">Currency converter built with TypeScript, Inquirer, and Node.js.</p>
              <a href="https://github.com/ayazahmed07/curconverter" target="_blank" class="btn btn-outline-primary">View Project</a>
            </div>
          </div>
        </div>
        <!-- Simple Calculator -->
        <div class="col-md-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title">Simple Calculator</h5>
              <p class="card-text">A simple calculator created using TypeScript, Node.js, and Inquirer.</p>
              <a href="https://github.com/ayazahmed07/simple-calculator" target="_blank" class="btn btn-outline-primary">View Project</a>
            </div>
          </div>
        </div>
        <!-- Todo App -->
        <div class="col-md-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title">Todo App</h5>
              <p class="card-text">A task management app developed using JavaScript.</p>
              <a href="https://github.com/ayazahmed07/todo" target="_blank" class="btn btn-outline-primary">View Project</a>
            </div>
          </div>
        </div>
        <!-- TypeScript Assignment -->
        <div class="col-md-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title">TypeScript Getting Started Assignment</h5>
              <p class="card-text">An introductory assignment project for learning TypeScript.</p>
              <a href="https://github.com/ayazahmed07/typescript-getting-started-Assignment" target="_blank" class="btn btn-outline-primary">View Project</a>
            </div>
          </div>
        </div>
        <!-- Word Counter -->
        <div class="col-md-4">
          <div class="card">
            <div class="card-body">
              <h5 class="card-title">Word Counter</h5>
              <p class="card-text">A project to count words using JavaScript.</p>
              <a href="https://github.com/ayazahmed07/wordcounter" target="_blank" class="btn btn-outline-primary">View Project</a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Graphical Representation Section -->
    <div class="chart-container">
      <h2>Programming Languages Breakdown</h2>
      <canvas id="languageChart" width="400" height="400"></canvas>
    </div>
  </div>

  <!-- Bootstrap Bundle with Popper -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
  <!-- Chart.js Library -->
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script>
    // Sample data for language usage based on your pinned projects.
    const data = {
      labels: ['JavaScript', 'TypeScript'],
      datasets: [{
        data: [5, 1], // Adjust these values based on your actual project stats.
        backgroundColor: [
          'rgba(255, 206, 86, 0.7)',
          'rgba(54, 162, 235, 0.7)'
        ],
        borderColor: [
          'rgba(255, 206, 86, 1)',
          'rgba(54, 162, 235, 1)'
        ],
        borderWidth: 1
      }]
    };

    const config = {
      type: 'pie',
      data: data,
      options: {
        responsive: true,
        plugins: {
          legend: {
            position: 'top'
          },
          title: {
            display: true,
            text: 'Language Usage in Pinned Projects'
          }
        }
      }
    };

    // Render the chart
    const languageChart = new Chart(
      document.getElementById('languageChart'),
      config
    );
  </script>
</body>
</html>
