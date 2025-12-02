<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tejas Govind Pokalwar</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Segoe UI',system-ui,sans-serif}
body{background:#0f172a;color:#e2e8f0;min-height:100vh;padding:20px}
.container{max-width:1000px;margin:0 auto;padding:20px}
.header{text-align:center;padding:40px 0}
h1{font-size:2.8rem;margin-bottom:15px;background:linear-gradient(90deg,#60a5fa,#34d399,#fbbf24,#f472b6);background-clip:text;-webkit-background-clip:text;color:transparent;animation:fadeInDown 1s ease,colorShift 8s infinite alternate}
@keyframes fadeInDown{from{opacity:0;transform:translateY(-30px)}to{opacity:1;transform:translateY(0)}}
@keyframes colorShift{0%{background-position:0% 50%}100%{background-position:100% 50%}}
.wave-emoji{animation:wave 2s infinite;transform-origin:70% 70%}
@keyframes wave{0%{transform:rotate(0deg)}10%{transform:rotate(14deg)}20%{transform:rotate(-8deg)}30%{transform:rotate(14deg)}40%{transform:rotate(-4deg)}50%{transform:rotate(10deg)}60%{transform:rotate(0deg)}100%{transform:rotate(0deg)}}
.subtitle{font-size:1.3rem;font-style:italic;margin-bottom:30px;color:#94a3b8;animation:fadeInDown 1.2s ease 0.2s both}
hr{border:none;height:3px;background:linear-gradient(90deg,transparent,#60a5fa,#34d399,transparent);margin:30px 0;animation:lineExpand 1.5s ease}
@keyframes lineExpand{from{width:0;margin-left:50%}to{width:100%;margin-left:0}}
.section{background:rgba(30,41,59,0.7);border-radius:12px;padding:25px;margin-bottom:25px;box-shadow:0 10px 30px rgba(0,0,0,0.3);border-left:5px solid#60a5fa;animation:slideInRight 0.8s ease}
.section:hover{transform:translateY(-5px);box-shadow:0 15px 35px rgba(0,0,0,0.4);transition:all 0.3s}
@keyframes slideInRight{from{opacity:0;transform:translateX(30px)}to{opacity:1;transform:translateX(0)}}
h2{font-size:1.8rem;margin-bottom:20px;color:#34d399;display:flex;align-items:center}
h2::before{content:"";display:inline-block;width:10px;height:10px;background-color:#f472b6;border-radius:50%;margin-right:10px;animation:pulse 2s infinite}
@keyframes pulse{0%,100%{transform:scale(1);opacity:1}50%{transform:scale(1.3);opacity:0.7}}
ul{list-style-type:none}
li{padding:8px 0;padding-left:25px;position:relative}
li::before{content:"▹";position:absolute;left:0;color:#fbbf24;animation:bounce 1s infinite alternate}
@keyframes bounce{from{transform:translateX(0)}to{transform:translateX(5px)}}
.badges{display:flex;flex-wrap:wrap;gap:10px;margin-top:15px}
.badge{display:inline-block;padding:8px 16px;border-radius:20px;font-weight:bold;font-size:0.9rem;animation:badgeGlow 3s infinite alternate}
@keyframes badgeGlow{0%{box-shadow:0 0 5px currentColor}100%{box-shadow:0 0 15px currentColor}}
.leetcode{background:#FFA116;color:#000}
.codechef{background:#5B4638;color:#fff}
.codeforces{background:#3B5998;color:#fff}
.tech-stack{display:flex;flex-wrap:wrap;gap:10px;margin-top:15px}
.tech-item{padding:6px 12px;background:rgba(96,165,250,0.2);border-radius:8px;border:1px solid rgba(96,165,250,0.5);animation:float 3s ease-in-out infinite}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-5px)}}
.quote{text-align:center;font-style:italic;padding:25px;margin-top:30px;border-radius:12px;background:rgba(248,113,113,0.1);border-left:5px solid#f87171;border-right:5px solid#f87171;animation:quoteFade 2s ease,borderPulse 4s infinite}
@keyframes quoteFade{from{opacity:0}to{opacity:1}}
@keyframes borderPulse{0%,100%{border-color:#f87171}50%{border-color:#34d399}}
.connect{text-align:center;margin-top:40px;animation:fadeInUp 1s ease}
@keyframes fadeInUp{from{opacity:0;transform:translateY(30px)}to{opacity:1;transform:translateY(0)}}
.social-links{display:flex;justify-content:center;gap:20px;margin-top:20px}
.social-btn{display:inline-block;padding:12px 25px;border-radius:30px;text-decoration:none;font-weight:bold;animation:socialPulse 2s infinite}
@keyframes socialPulse{0%,100%{transform:scale(1)}50%{transform:scale(1.05)}}
.github{background:#000;color:#fff}
.linkedin{background:#0A66C2;color:#fff}
li:nth-child(1){animation:fadeInList 0.5s ease 0.1s both}
li:nth-child(2){animation:fadeInList 0.5s ease 0.2s both}
li:nth-child(3){animation:fadeInList 0.5s ease 0.3s both}
@keyframes fadeInList{to{opacity:1}from{opacity:0}}
@media(max-width:768px){h1{font-size:2.2rem}.section{padding:20px}.social-links{flex-direction:column;align-items:center}}
</style>
</head>
<body>
<div class="container">
<header class="header">
<h1><span class="wave-emoji">👋</span> Hi, I'm Tejas Govind Pokalwar</h1>
<p class="subtitle">Web Developer • Data Analyst • Machine Learning Enthusiast • Competitive Programmer</p>
</header>
<hr>
<section class="section">
<h2>🧠 Competitive Programming</h2>
<ul>
<li><strong>LeetCode Knight Badge</strong> — 2000+ rating & 800+ problems solved</li>
<li><strong>CodeChef 3★ (Max Rating: 1670)</strong></li>
<li><strong>Codeforces Pupil (Max Rating: 1376)</strong></li>
</ul>
<div class="badges">
<div class="badge leetcode">LeetCode Knight</div>
<div class="badge codechef">CodeChef 3★</div>
<div class="badge codeforces">Codeforces Pupil</div>
</div>
</section>
<section class="section">
<h2>🎓 Academic Achievements</h2>
<ul>
<li><strong>10.0 SGPA in both first-year semesters</strong></li>
<li><strong>Overall CGPA: 9.84</strong></li>
<li><strong>Strong foundation in mathematics, algorithms, and core CS concepts</strong></li>
</ul>
</section>
<section class="section">
<h2>🚀 About Me</h2>
<p>I'm a focused developer passionate about building real products, analyzing data, and exploring machine learning.</p>
<p>I enjoy solving challenging problems, contributing to scalable systems, and continuously improving my technical depth.</p>
</section>
<section class="section">
<h2>💻 Web Development</h2>
<div class="tech-stack">
<div class="tech-item">HTML</div>
<div class="tech-item">CSS</div>
<div class="tech-item">JavaScript</div>
<div class="tech-item">React.js</div>
<div class="tech-item">Next.js</div>
<div class="tech-item">Node.js</div>
<div class="tech-item">Express</div>
<div class="tech-item">MongoDB</div>
<div class="tech-item">MySQL</div>
<div class="tech-item">REST APIs</div>
<div class="tech-item">Authentication</div>
<div class="tech-item">Deployment</div>
</div>
<p style="margin-top:15px"><strong>Full-stack MERN/Next.js applications</strong></p>
</section>
<section class="section">
<h2>📊 Data Analysis & Machine Learning</h2>
<div class="tech-stack">
<div class="tech-item">Python</div>
<div class="tech-item">NumPy</div>
<div class="tech-item">Pandas</div>
<div class="tech-item">Matplotlib</div>
<div class="tech-item">Seaborn</div>
<div class="tech-item">Scikit-learn</div>
</div>
<ul style="margin-top:15px">
<li>Data cleaning, preprocessing, exploratory analysis</li>
<li>Building and evaluating simple ML models</li>
</ul>
</section>
<section class="connect">
<h2>📬 Connect With Me</h2>
<div class="social-links">
<a href="https://github.com/Tejas134200" class="social-btn github">GitHub</a>
<a href="https://www.linkedin.com/in/tejas-pokalwar-049a58297/" class="social-btn linkedin">LinkedIn</a>
</div>
</section>
<div class="quote">
<p>⭐ "The more you learn, the more you realize how much more there is to explore."</p>
</div>
</div>
</body>
</html>
