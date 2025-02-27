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

    form {
      display: flex;
      flex-direction: column;
      max-width: 400px;
      margin: 0 auto;
    }

    label {
      margin-bottom: 0.5rem;
      font-weight: bold;
    }

    input[type="number"], input[type="text"] {
      padding: 0.5rem;
      margin-bottom: 1rem;
      border: 1px solid #ccc;
      border-radius: 4px;
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

    footer {
      text-align: center;
      padding: 1rem 0;
      background: #2c3e50;
      color: white;
      position: relative;
      bottom: 0;
      width: 100%;
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
      <h2>Project Cost Estimator</h2>
      <form id="projectForm">
        <label for="area">Project Area (sqm):</label>
        <input type="number" id="area" name="area" required>

        <label for="materials">Materials Used:</label>
        <input type="text" id="materials" name="materials" placeholder="e.g., Steel, Concrete" required>

        <button type="submit">Estimate Costs</button>
      </form>
    </div>

    <div class="section">
      <h2>Data Insights</h2>
      <div class="data-insights" id="insights">
        <!-- Dynamic insights will be inserted here -->
      </div>
    </div>
  </div>

  <footer>
    <p>&copy; 2023 AI-Powered Quantity Surveyor Workflow. All rights reserved.</p>
  </footer>

  <script>
    // Simulate AI-driven cost estimation
    document.getElementById('projectForm').addEventListener('submit', function(event) {
      event.preventDefault();

      // Get user input
      const area = parseFloat(document.getElementById('area').value);
      const materials = document.getElementById('materials').value;

      // Simulate AI calculation (basic example)
      const baseCostPerSqm = 150; // Example cost per square meter
      const materialCostFactor = materials.includes('Steel') ? 1.2 : 1.0; // Adjust cost based on materials
      const totalCost = area * baseCostPerSqm * materialCostFactor;

      // Display results dynamically
      const insightsSection = document.getElementById('insights');
      insightsSection.innerHTML = ''; // Clear previous insights

      // Create insight cards
      const createCard = (title, value) => {
        const card = document.createElement('div');
        card.className = 'insight-card';
        card.innerHTML = `
          <h3>${title}</h3>
          <p>${value}</p>
        `;
        insightsSection.appendChild(card);
      };

      createCard('Project Area', `${area} sqm`);
      createCard('Materials', materials);
      createCard('Estimated Cost', `$${totalCost.toFixed(2)}`);
      createCard('Time Estimation', `${Math.ceil(area / 100)} months`); // Example time estimation
    });
  </script>
</body>
</html>
