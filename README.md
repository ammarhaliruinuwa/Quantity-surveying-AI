<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AI-Powered Quantity Surveyor Workflow</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f7fc;
      color: #333;
    }

    header {
      background: #007bff;
      color: white;
      padding: 1rem 2rem;
      text-align: center;
    }

    .container {
      max-width: 1200px;
      margin: 2rem auto;
      padding: 0 1rem;
    }

    h1, h2, h3 {
      color: #2c3e50;
    }

    .section {
      background: white;
      border-radius: 8px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      padding: 1.5rem;
      margin-bottom: 1.5rem;
    }

    .feature {
      display: flex;
      align-items: center;
      margin-bottom: 1rem;
    }

    .feature img {
      width: 60px;
      height: 60px;
      margin-right: 1rem;
    }

    footer {
      text-align: center;
      padding: 1rem 0;
      background: #2c3e50;
      color: white;
      position: relative;
      bottom: 0;
      width: 100%;
    }

    button {
      background: #007bff;
      color: white;
      border: none;
      padding: 0.75rem 1.5rem;
      border-radius: 4px;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s ease;
    }

    button:hover {
      background: #0056b3;
    }

    .data-insights {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
    }

    .insight-card {
      background: #ffffff;
      border-radius: 8px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      padding: 1rem;
      text-align: center;
    }

    .insight-card h3 {
      margin: 0.5rem 0;
    }

    .insight-card p {
      font-size: 1rem;
      color: #666;
    }

    /* Modal Styles */
    .modal {
      display: none;
      position: fixed;
      z-index: 1;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(0, 0, 0, 0.5);
    }

    .modal-content {
      background-color: #fefefe;
      margin: 15% auto;
      padding: 20px;
      border: 1px solid #888;
      width: 80%;
      max-width: 600px;
      border-radius: 8px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    }

    .close {
      color: #aaa;
      float: right;
      font-size: 28px;
      font-weight: bold;
    }

    .close:hover,
    .close:focus {
      color: black;
      text-decoration: none;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <header>
    <h1>AI-Powered Quantity Surveyor Workflow</h1>
    <p>Streamline your tasks, gain data-driven insights, and enhance collaboration.</p>
  </header>

  <div class="container">
    <div class="section">
      <h2>Key Features</h2>
      <div class="feature">
        <img src="https://via.placeholder.com/60x60?text=Automation" alt="Automation Icon">
        <div>
          <h3>Task Automation</h3>
          <p>Automate repetitive tasks such as material takeoff, cost estimation, and report generation using advanced AI algorithms.</p>
        </div>
      </div>
      <div class="feature">
        <img src="https://via.placeholder.com/60x60?text=Insights" alt="Insights Icon">
        <div>
          <h3>Data-Driven Insights</h3>
          <p>Access real-time analytics and predictive insights to make informed decisions about project costs and timelines.</p>
        </div>
      </div>
      <div class="feature">
        <img src="https://via.placeholder.com/60x60?text=Collaboration" alt="Collaboration Icon">
        <div>
          <h3>Enhanced Collaboration</h3>
          <p>Collaborate seamlessly with team members through integrated communication tools and shared project dashboards.</p>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Data Insights</h2>
      <div class="data-insights">
        <div class="insight-card">
          <h3>Project Costs</h3>
          <p>$500,000</p>
        </div>
        <div class="insight-card">
          <h3>Material Usage</h3>
          <p>200 tons of steel</p>
        </div>
        <div class="insight-card">
          <h3>Time Estimation</h3>
          <p>12 months</p>
        </div>
        <div class="insight-card">
          <h3>Resource Allocation</h3>
          <p>50 workers</p>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>Get Started</h2>
      <button id="startButton">Start Now</button>
    </div>
  </div>

  <!-- Modal -->
  <div id="myModal" class="modal">
    <div class="modal-content">
      <span class="close">&times;</span>
      <h2>Welcome to the AI-Powered Quantity Surveyor Workflow</h2>
      <p>This platform is designed to streamline your workflow by automating tasks, providing data-driven insights, and enhancing collaboration.</p>
      <button onclick="closeModal()">Close</button>
    </div>
  </div>

  <footer>
    <p>&copy; 2023 AI-Powered Quantity Surveyor Workflow. All rights reserved.</p>
  </footer>

  <script>
    // Get modal element
    var modal = document.getElementById("myModal");

    // Get the button that opens the modal
    var startButton = document.getElementById("startButton");

    // Get the <span> element that closes the modal
    var span = document.getElementsByClassName("close")[0];

    // When the user clicks the button, open the modal 
    startButton.onclick = function() {
      modal.style.display = "block";
    }

    // When the user clicks on <span> (x), close the modal
    span.onclick = function() {
      closeModal();
    }

    // When the user clicks anywhere outside of the modal, close it
    window.onclick = function(event) {
      if (event.target == modal) {
        closeModal();
      }
    }

    // Function to close the modal
    function closeModal() {
      modal.style.display = "none";
    }
  </script>
</body>
</html>
