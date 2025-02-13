<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Edit Option for GitHub README Code</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
    }
    #codeDisplay {
      background-color: #f5f5f5;
      padding: 10px;
      border: 1px solid #ccc;
      white-space: pre-wrap;
      font-family: Consolas, monospace;
    }
    #codeArea {
      width: 100%;
      height: 400px;
      font-family: Consolas, monospace;
      display: none;
    }
    button {
      margin-bottom: 10px;
      padding: 5px 10px;
      font-size: 16px;
    }
  </style>
</head>
<body>

<button id="toggleButton" onclick="toggleEdit()">Edit</button>

<!-- Updated README code with Skills, Projects and Real Time Girl Animation -->
<pre id="codeDisplay">
&lt;h1 align="center"&gt;Hi, I'm Monica Jayakumar &lt;img src="https://media.giphy.com/media/l0MYt5jPR6QX5pnqM/giphy.gif" width="35"&gt;&lt;/h1&gt;

&lt;p align="center"&gt;
  &lt;a href="https://github.com/Monica2403"&gt;&lt;img src="https://img.shields.io/badge/GitHub-181717?style=plastic&amp;logo=github&amp;logoColor=white" alt="GitHub"&gt;&lt;/a&gt;
  &lt;a href="mailto:monicaajayakumar@gmail.com"&gt;&lt;img src="https://img.shields.io/badge/Gmail-EA4335?style=plastic&amp;logo=gmail&amp;logoColor=white" alt="Email"&gt;&lt;/a&gt;
  &lt;a href="https://linkedin.com/in/monicajayakumar"&gt;&lt;img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=plastic&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn"&gt;&lt;/a&gt;
&lt;/p&gt;

&lt;p align="center"&gt;
  &lt;img src="https://komarev.com/ghpvc/?username=Monica2403&amp;label=Profile%20views&amp;color=0047AB&amp;style=plastic" alt="Profile views"&gt;
&lt;/p&gt;

&lt;hr&gt;

&lt;h2 id="about-me"&gt;About Me&lt;/h2&gt;
&lt;p&gt;
  I am a highly analytical professional with a strong focus on leveraging data to drive strategic decision-making. Passionate about using cutting-edge tools and techniques, I excel in data mining, visualization, and implementing machine learning solutions to solve complex problems.
&lt;/p&gt;

&lt;h2 id="skills"&gt;Skills&lt;/h2&gt;
&lt;p&gt;
  &lt;strong&gt;Programming &amp; Data Analysis:&lt;/strong&gt; Python, R Programming, SQL&lt;br&gt;
  &lt;strong&gt;Data Visualization &amp; BI:&lt;/strong&gt; Power BI, Tableau&lt;br&gt;
  &lt;strong&gt;Cloud &amp; Machine Learning:&lt;/strong&gt; AWS, Azure-ML, Deep Learning&lt;br&gt;
  &lt;strong&gt;Other Tools:&lt;/strong&gt; Microsoft Power Platform, SAP, Model Driven Apps, JIRA, Confluence, DevOps, Visio, Miro, MS PowerPoint, MS Excel, MS Word, NLP
&lt;/p&gt;

&lt;h2 id="projects"&gt;Highlight Ground Breaking Projects:&lt;/h2&gt;
&lt;h3&gt;Nebula AI&lt;/h3&gt;
&lt;p&gt;&lt;strong&gt;Link:&lt;/strong&gt; &lt;a href="https://nebulaspace.netlify.app/" target="_blank"&gt;https://nebulaspace.netlify.app/&lt;/a&gt;&lt;/p&gt;
&lt;p&gt;Nebula AI is an autonomous space mission control system designed to optimize satellite operations through cutting-edge artificial intelligence. It integrates advanced AI agents that proactively detect anomalies, dynamically allocate resources, and make real-time decisions to ensure mission success. By leveraging real-time telemetry data and predictive analytics, Nebula AI enhances system reliability, reduces operational risks, and minimizes human intervention. The system features real-time dashboards, simulation modules, and task scheduling agents to support complex missions like Saturn Orbit Insertion and Titan Flybys. Its adaptable architecture supports multi-satellite coordination, making it a future-ready solution for space exploration and commercial satellite management.&lt;/p&gt;
&lt;p&gt;Currently exploring AI Agents and developing models related to autonomous decision-making and real-time system optimization.&lt;/p&gt;

&lt;h2 id="connect-with-me"&gt;Connect with Me&lt;/h2&gt;
&lt;p&gt;
  &lt;a href="mailto:monicaajayakumar@gmail.com"&gt;&lt;img src="https://img.shields.io/badge/Gmail-EA4335?style=plastic&amp;logo=gmail&amp;logoColor=white" alt="Email"&gt;&lt;/a&gt;
  &lt;a href="https://github.com/Monica2403"&gt;&lt;img src="https://img.shields.io/badge/GitHub-181717?style=plastic&amp;logo=github&amp;logoColor=white" alt="GitHub"&gt;&lt;/a&gt;
  &lt;a href="https://linkedin.com/in/monicajayakumar"&gt;&lt;img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=plastic&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn"&gt;&lt;/a&gt;
&lt;/p&gt;

&lt;p align="center"&gt;&lt;i&gt;Location: Cambridge, United Kingdom&lt;/i&gt;&lt;/p&gt;
</pre>

<textarea id="codeArea"></textarea>

<script>
  function toggleEdit() {
    var codeDisplay = document.getElementById('codeDisplay');
    var codeArea = document.getElementById('codeArea');
    var toggleButton = document.getElementById('toggleButton');
    
    if (codeArea.style.display === 'none' || codeArea.style.display === '') {
      // Switch to edit mode: copy current code to the textarea
      codeArea.value = codeDisplay.textContent;
      codeDisplay.style.display = 'none';
      codeArea.style.display = 'block';
      toggleButton.textContent = 'Save';
    } else {
      // Save changes: copy text from textarea back to the display
      codeDisplay.textContent = codeArea.value;
      codeDisplay.style.display = 'block';
      codeArea.style.display = 'none';
      toggleButton.textContent = 'Edit';
    }
  }
</script>

</body>
</html>
