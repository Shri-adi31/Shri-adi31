<!DOCTYPE html>
<html>
<head>
  <title>Introduction</title>
  <style>
    body {
      background-color: lightblue;
      text-align: center;
    }
    h1 {
      color: darkblue;
      font-size: 3em;
      font-weight: bold;
      margin: 20px 0;
    }
    p {
      color: darkgreen;
      font-size: 2em;
      margin: 20px 0;
    }
    img {
      height: 300px;
      border-radius: 50%;
    }
    ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
    }
    li {
      display: inline-block;
      margin: 0 10px;
      font-size: 1.5em;
      color: darkred;
    }
  </style>
</head>
<body>
  <h1>My name is Shriman Aditya</h1>
  <p>I am a CSE graduate and a web developer for GitHub.</p>
  <img src="https://i.imgur.com/YxLZOjO.jpg" alt="Programming nerd">
  <p>Number of unique visitors: <span id="visitor-count">0</span></p>
  <p>Most frequently used languages:</p>
  <ul>
    <li>JavaScript</li>
    <li>HTML</li>
    <li>CSS</li>
    <li>Python</li>
  </ul>
  <script>
    console.log("Hello! My name is Shriman Aditya and I am a CSE graduate and a web developer for GitHub.");
    var visitorCount = 0;
    if (localStorage.getItem("visitorCount") == null) {
      localStorage.setItem("visitorCount", 0);
    } else {
      visitorCount = parseInt(localStorage.getItem("visitorCount"));
      visitorCount++;
      localStorage.setItem("visitorCount", visitorCount);
    }
    document.getElementById("visitor-count").innerHTML = visitorCount;
  </script>
</body>
</html>
