# My name is Shriman Aditya

I am a CSE graduate and a web developer for GitHub.

![Programming nerd](https://i.imgur.com/YxLZOjO.jpg)

Number of unique visitors: **0**

Most frequently used languages:
- JavaScript [5]
- HTML [3]
- CSS [2]
- Python [4]

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
