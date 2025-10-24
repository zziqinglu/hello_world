<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Your Name | Academic Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 40px auto;
      max-width: 800px;
      line-height: 1.6;
      color: #222;
    }
    h1, h2 {
      border-bottom: 2px solid #ccc;
      padding-bottom: 4px;
    }
    a {
      color: #0366d6;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .section {
      margin-top: 30px;
    }
  </style>
</head>

<body>
  <h1>Your Name</h1>
  <p>Department of Computer Science, University Name</p>
  <p>
    Email: <a href="mailto:your.email@university.edu">your.email@university.edu</a> |
    <a href="https://github.com/yourusername">GitHub</a> |
    <a href="https://scholar.google.com">Google Scholar</a>
  </p>

  <div class="section">
    <h2>About</h2>
    <p>
      I am a researcher interested in reinforcement learning, optimization, and decision-making under uncertainty.
      I am currently a Ph.D. candidate at University Name, advised by Prof. Advisor.
    </p>
  </div>

  <div class="section">
    <h2>Research</h2>
    <ul>
      <li>Reinforcement learning with function approximation</li>
      <li>Safe and robust decision making</li>
      <li>Hierarchical and configurable MDPs</li>
    </ul>
  </div>

  <div class="section">
    <h2>Publications</h2>
    <ul>
      <li>
        <strong>Title of Paper</strong>,
        Conference on Machine Learning (ICML), 2025.
        <a href="#">[PDF]</a> <a href="#">[Code]</a>
      </li>
      <li>
        <strong>Another Paper Title</strong>,
        Journal of Artificial Intelligence Research (JAIR), 2024.
        <a href="#">[PDF]</a>
      </li>
    </ul>
  </div>

  <div class="section">
    <h2>Teaching</h2>
    <ul>
      <li>CS101: Introduction to Machine Learning (Spring 2025)</li>
      <li>CS201: Reinforcement Learning (Fall 2024)</li>
    </ul>
  </div>

  <div class="section">
    <h2>Contact</h2>
    <p>
      Office: Room 123, Science Building, University Name<br>
      Email: <a href="mailto:your.email@university.edu">your.email@university.edu</a>
    </p>
  </div>

  <footer style="margin-top: 40px; border-top: 1px solid #ccc; padding-top: 10px; font-size: 0.9em; color: #555;">
    © <span id="year"></span> Your Name — Hosted on GitHub Pages
  </footer>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
