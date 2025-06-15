<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Society Stock Market | Society Day Live Tracker</title>
  <style>
    body {
      background-color: black;
      color: gold;
      font-family: 'Courier New', Courier, monospace;
      text-align: center;
    }
    table {
      margin: auto;
      border-collapse: collapse;
      width: 80%;
    }
    th, td {
      border: 1px solid gold;
      padding: 12px;
      background-color: #111;
    }
    th {
      background-color: #222;
    }
    .updated {
      background-color: green;
      color: white;
      transition: background-color 0.5s ease;
    }
  </style>
</head>
<body>
  <h1>Society Stock Market Live Tracker</h1>
  <table id="stockTable">
    <thead>
      <tr>
        <th>Society</th>
        <th>Total Signups</th>
        <th>Price (RM)</th>
      </tr>
    </thead>
    <tbody>
      <!-- Data will go here -->
    </tbody>
  </table>

  <script>
    const sheetUrl = "https://docs.google.com/spreadsheets/d/e/2PACX-1vS8taswu21YKZtY4egCW6S8OCeuOo0tVef54zr-3bk47s_kUwV6H2BdIjhKTG1yF9e_GkxEbNW485WM/pub?output=csv";
    let previousData = {};

    async function fetchData() {
      try {
        const response = await fetch(sheetUrl);
        const text = await response.text();
        const rows = text.trim().split("\n").map(row => row.split(","));
        const tableBody = document.querySelector("#stockTable tbody");

        tableBody.innerHTML = "";

        for (let i = 1; i < rows.length; i++) {
          if (rows[i].length < 3) continue;
          const [name, total, price] = rows[i];

          const row = document.createElement("tr");

          [name, total, price].forEach((val, index) => {
            const cell = document.createElement("td");
            cell.textContent = val;

            const key = `${name}-${index}`;
            if (previousData[key] !== undefined && previousData[key] !== val) {
              cell.classList.add("updated");
              setTimeout(() => cell.classList.remove("updated"), 5000);
            }

            previousData[key] = val;
            row.appendChild(cell);
          });

          tableBody.appendChild(row);
        }
      } catch (error) {
        console.error("❌ Failed to fetch data:", error);
      }
    }

    fetchData();
    setInterval(fetchData, 5000);
  </script>
</body>
</html>
