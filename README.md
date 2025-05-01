<!DOCTYPE html>  <html lang="en">  
<head>  
  <meta charset="UTF-8" />  
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>  
  <title>Chinthakula Charan Goud - Portfolio</title>  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
  <style>  
    body {  
      margin: 0;  
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;  
      background-color: #0f0f0f;  
      color: #fff;  
      overflow-x: hidden;  
    }  .dark-mode {  
  background-color: #fff;  
  color: #000;  
}  

header {  
  background: #1a1a1a;  
  padding: 40px 20px 20px;  
  text-align: center;  
  position: relative;  
  overflow: hidden;  
}  

.blinking {  
  animation: blink 1.5s linear infinite;  
  color: #00ffe1;  
  font-size: 2.2em;  
  font-weight: bold;  
}  

@keyframes blink {  
  0%, 100% { opacity: 1; }  
  50% { opacity: 0.3; }  
}  

.typewriter {  
  display: inline-block;  
  font-size: 2.5em;  
  color: #ff00ff;  
  font-weight: bold;  
  white-space: nowrap;  
  overflow: hidden;  
  border-right: 4px solid #ff00ff;  
  animation: typing 3s steps(20) 1s forwards, blinkCaret 0.75s step-end infinite;  
}  

@keyframes typing {  
  from {  
    width: 0;  
  }  
  to {  
    width: 100%;  
  }  
}  

@keyframes blinkCaret {  
  50% {  
    border-color: transparent;  
  }  
}  

nav {  
  text-align: center;  
  margin-top: 10px;  
}  

nav a {  
  margin: 0 15px;  
  text-decoration: none;  
  color: #00ffe1;  
  transition: color 0.3s, transform 0.3s;  
}  

nav a:hover {  
  color: #00cccc;  
  transform: scale(1.1);  
}  

section {  
  padding: 40px 20px;  
  text-align: center;  
  animation: fadeIn 1s ease forwards;  
  opacity: 0;  
}  

.visible {  
  opacity: 1 !important;  
}  

.info-card {  
  background: #1f1f1f;  
  margin: 20px auto;  
  padding: 20px;  
  max-width: 700px;  
  border-radius: 10px;  
  box-shadow: 0 0 15px rgba(0,255,225,0.1);  
  animation: slideUp 0.8s ease-in-out;  
}  

@keyframes fadeIn {  
  from { opacity: 0; transform: translateY(20px); }  
  to { opacity: 1; transform: translateY(0); }  
}  

@keyframes slideUp {  
  from { opacity: 0; transform: translateY(50px); }  
  to { opacity: 1; transform: translateY(0); }  
}  

.short-boxes {  
  display: flex;  
  flex-wrap: wrap;  
  justify-content: center;  
  gap: 15px;  
  margin-top: 20px;  
}  

.short-box {  
  background: #2a2a2a;  
  padding: 15px 20px;  
  border-radius: 8px;  
  font-size: 0.95em;  
  color: #00ffe1;  
  box-shadow: 0 0 8px rgba(0,255,225,0.2);  
  transition: transform 0.3s ease;  
}  

.short-box:hover {  
  transform: scale(1.05);  
}  

table {  
  width: 100%;  
  margin-top: 20px;  
  border-collapse: collapse;  
  color: #fff;  
}  

table, th, td {  
  border: 1px solid #00ffe1;  
}  

th, td {  
  padding: 10px;  
  text-align: left;  
}  

th {  
  background-color: #333;  
}  

td {  
  background-color: #1f1f1f;  
}  

footer {  
  background: #121212;  
  padding: 20px;  
  text-align: center;  
  color: #777;  
}  

.toggle-switch {  
  position: absolute;  
  top: 10px;  
  right: 20px;  
  display: flex;  
  align-items: center;  
  cursor: pointer;  
}  

.switch {  
  width: 50px;  
  height: 25px;  
  background: #444;  
  border-radius: 50px;  
  position: relative;  
  transition: background 0.3s;  
}  

.switch::after {  
  content: "";  
  width: 21px;  
  height: 21px;  
  background: #fff;  
  position: absolute;  
  top: 2px;  
  left: 2px;  
  border-radius: 50%;  
  transition: left 0.3s;  
}  

.dark-mode .switch {  
  background: #00ffe1;  
}  

.dark-mode .switch::after {  
  left: 27px;  
}  

.skills-icons i {  
  margin: 0 10px;  
  font-size: 24px;  
  color: #00ffe1;  
  animation: iconAnim 0.5s ease-in-out forwards;  
  opacity: 0;  
  transform: scale(0.6);  
}  

.skills-icons i:nth-child(1) { animation-delay: 0.2s; }  
.skills-icons i:nth-child(2) { animation-delay: 0.4s; }  
.skills-icons i:nth-child(3) { animation-delay: 0.6s; }  
.skills-icons i:nth-child(4) { animation-delay: 0.8s; }  

@keyframes iconAnim {  
  to {  
    opacity: 1;  
    transform: scale(1);  
  }  
}  

.btn {  
  display: inline-block;  
  margin-top: 15px;  
  padding: 10px 20px;  
  background-color: #00ffe1;  
  color: #000;  
  text-decoration: none;  
  border-radius: 5px;  
  transition: 0.3s ease;  
}  

.btn:hover {  
  background-color: #00cccc;  
  transform: scale(1.05);  
}  

form input, form textarea {  
  width: 90%;  
  padding: 10px;  
  margin: 10px 0;  
  border-radius: 5px;  
  border: none;  
}  

.parallax {  
  background: url('https://via.placeholder.com/1920x1080') center center/cover no-repeat;  
  min-height: 100vh;  
  position: relative;  
  z-index: -1;  
  transform: translateZ(0);  
}  

.parallax-content {  
  position: relative;  
  z-index: 1;  
}

  </style>  
</head>  
<body>  <header>  
  <div class="toggle-switch" onclick="toggleTheme()">  
    <div class="switch"></div>  
  </div>  
  <div class="blinking">Chinthakula Charan Goud</div>  
  <div class="typewriter">Portfolio</div>  
</header>  <nav>  
  <a href="#about">About</a>  
  <a href="#education">Education</a>  
  <a href="#skills">Skills</a>  
  <a href="#interests">Interests</a>  
  <a href="#contact">Contact</a>  
</nav>  <section id="about" class="parallax">  
  <div class="parallax-content">  
    <div class="info-card">  
      <h2>About Me</h2>  
      <p>I am Chinthakula Charan Goud, a passionate and curious student who is exploring various domains in the tech world. I have completed certifications like PGDCA and Tally Prime ERP, and I'm familiar with Microsoft Office tools including Excel, PowerPoint, and Word (2007). Though I’m still building my technical skillset, I am focused, disciplined, and committed to continuous learning. I aim to grow into a successful professional in the IT industry.</p>  
      <a class="btn" href="charan-resume.pdf" download>Download CV</a>  
    </div>  
  </div>  
</section>  <section id="education">  
  <div class="info-card">  
    <h2>Education</h2>  
    <table>  
      <tr><th>Qualification</th><th>Duration</th></tr>  
      <tr><td>SSC</td><td>2022 - 2023</td></tr>  
      <tr><td>Intermediate</td><td>2023 - 2025</td></tr>  
    </table>  
  </div>  
</section>  <section id="skills">  
  <div class="info-card">  
    <h2>Skills</h2>  
    <div class="skills-icons">  
      <i class="fas fa-laptop-code"></i>  
      <i class="fas fa-database"></i>  
      <i class="fas fa-file-excel"></i>  
      <i class="fas fa-file-powerpoint"></i>  
    </div>  
    <table>  
      <tr><th>Skill</th><th>Proficiency</th></tr>  
      <tr><td>PGDCA</td><td>Intermediate</td></tr>  
      <tr><td>Tally Prime ERP</td><td>Intermediate</td></tr>  
      <tr><td>MS Word 2007</td><td>Advanced</td></tr>  
      <tr><td>MS Excel</td><td>Advanced</td></tr>  
      <tr><td>MS PowerPoint</td><td>Intermediate</td></tr>  
    </table>  
  </div>  
</section>  <section id="interests">  
  <div class="info-card">  
    <h2>Career Interests</h2>  
    <div class="short-boxes">  
      <div class="short-box">Web Development</div>  
      <div class="short-box">Cybersecurity</div>  
      <div class="short-box">Data Science</div>  
      <div class="short-box">Data Analyst</div>  
    </div>  
  </div>  
</section>  <section id="contact">  
  <div class="info-card">  
    <h2>Contact Information</h2>  
    <p><strong>Email:</strong> charangoudchintakula@gmail.com</p>  
    <p><strong>Phone:</strong> 9398607743</p>  
    <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/charangoud" target="_blank" class="btn">LinkedIn Profile</a></p>  
    <p><strong>GitHub:</strong> <a href="https://github.com/charangoud" target="_blank" class="btn">GitHub Profile</a></p>  
  </div>  
</section>  <footer>  
  <p>&copy; 2025 Chinthakula Charan Goud. All rights reserved.</p>  
</footer>  <script>  
  function toggleTheme() {  
    document.body.classList.toggle('dark-mode');  
  }  
</script>  </body>  
</html>  
