<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tejas Govind Pokalwar - Animated Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            color: #f0f0f0;
            min-height: 100vh;
            padding: 20px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header Animations */
        .header {
            text-align: center;
            padding: 40px 0;
            position: relative;
        }
        
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 15px;
            background: linear-gradient(90deg, #ff7e5f, #feb47b, #86a8e7, #91eae4);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: fadeInDown 1s ease-out, colorShift 8s infinite alternate;
            background-size: 300% 100%;
        }
        
        @keyframes colorShift {
            0% { background-position: 0% 50%; }
            100% { background-position: 100% 50%; }
        }
        
        .wave-emoji {
            display: inline-block;
            animation: wave 2s infinite;
            transform-origin: 70% 70%;
        }
        
        @keyframes wave {
            0% { transform: rotate(0deg); }
            10% { transform: rotate(14deg); }
            20% { transform: rotate(-8deg); }
            30% { transform: rotate(14deg); }
            40% { transform: rotate(-4deg); }
            50% { transform: rotate(10deg); }
            60% { transform: rotate(0deg); }
            100% { transform: rotate(0deg); }
        }
        
        .subtitle {
            font-size: 1.3rem;
            font-style: italic;
            margin-bottom: 30px;
            color: #b8c1ec;
            animation: fadeInDown 1.2s ease-out 0.2s both;
        }
        
        hr {
            border: none;
            height: 3px;
            background: linear-gradient(90deg, transparent, #86a8e7, #91eae4, transparent);
            margin: 30px 0;
            animation: lineExpand 1.5s ease-out;
        }
        
        @keyframes lineExpand {
            from { width: 0; margin-left: 50%; }
            to { width: 100%; margin-left: 0; }
        }
        
        /* Section Animations */
        .section {
            background: rgba(30, 30, 46, 0.7);
            border-radius: 15px;
            padding: 25px;
            margin-bottom: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            border-left: 5px solid #86a8e7;
            animation: slideInRight 0.8s ease-out;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.4);
        }
        
        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        h2 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: #91eae4;
            display: flex;
            align-items: center;
        }
        
        h2::before {
            content: "";
            display: inline-block;
            width: 10px;
            height: 10px;
            background-color: #ff7e5f;
            border-radius: 50%;
            margin-right: 10px;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.3); opacity: 0.7; }
        }
        
        /* List Animations */
        ul {
            list-style-type: none;
        }
        
        li {
            padding: 8px 0;
            padding-left: 25px;
            position: relative;
            animation: fadeInList 0.5s ease-out forwards;
            opacity: 0;
        }
        
        @keyframes fadeInList {
            to { opacity: 1; }
        }
        
        li::before {
            content: "▹";
            position: absolute;
            left: 0;
            color: #feb47b;
            animation: bounce 1s infinite alternate;
        }
        
        @keyframes bounce {
            from { transform: translateX(0); }
            to { transform: translateX(5px); }
        }
        
        /* Badge Animations */
        .badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        
        .badge {
            display: inline-block;
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: bold;
            font-size: 0.9rem;
            animation: badgeGlow 3s infinite alternate;
        }
        
        @keyframes badgeGlow {
            0% { box-shadow: 0 0 5px currentColor; }
            100% { box-shadow: 0 0 15px currentColor; }
        }
        
        .leetcode { background: #FFA116; color: black; }
        .codechef { background: #5B4638; color: white; }
        .codeforces { background: #3B5998; color: white; }
        
        /* Tech Stack Animations */
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        
        .tech-item {
            padding: 6px 12px;
            background: rgba(134, 168, 231, 0.2);
            border-radius: 8px;
            border: 1px solid rgba(134, 168, 231, 0.5);
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }
        
        /* Quote Animation */
        .quote {
            text-align: center;
            font-style: italic;
            padding: 25px;
            margin-top: 30px;
            border-radius: 15px;
            background: rgba(255, 126, 95, 0.1);
            border-left: 5px solid #ff7e5f;
            border-right: 5px solid #ff7e5f;
            animation: quoteFade 2s ease-out, borderPulse 4s infinite;
            position: relative;
            overflow: hidden;
        }
        
        .quote::before {
            content: "❝";
            position: absolute;
            top: 10px;
            left: 15px;
            font-size: 2rem;
            color: rgba(255, 126, 95, 0.3);
        }
        
        .quote::after {
            content: "❞";
            position: absolute;
            bottom: 10px;
            right: 15px;
            font-size: 2rem;
            color: rgba(255, 126, 95, 0.3);
        }
        
        @keyframes quoteFade {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes borderPulse {
            0%, 100% { border-color: #ff7e5f; }
            50% { border-color: #91eae4; }
        }
        
        /* Connect Section */
        .connect {
            text-align: center;
            margin-top: 40px;
            animation: fadeInUp 1s ease-out;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-btn {
            display: inline-block;
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
            animation: socialPulse 2s infinite;
        }
        
        @keyframes socialPulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        .github { background: #000; color: white; }
        .linkedin { background: #0A66C2; color: white; }
        
        /* Stagger animations for list items */
        li:nth-child(1) { animation-delay: 0.1s; }
        li:nth-child(2) { animation-delay: 0.2s; }
        li:nth-child(3) { animation-delay: 0.3s; }
        li:nth-child(4) { animation-delay: 0.4s; }
        li:nth-child(5) { animation-delay: 0.5s; }
        
        /* Responsive adjustments */
        @media (max-width: 768px) {
            h1 { font-size: 2.2rem; }
            .section { padding: 20px; }
            .social-links { flex-direction: column; align-items: center; }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <h1><span class="wave-emoji">👋</span> Hi, I'm Tejas Govind Pokalwar</h1>
            <p class="subtitle">Web Developer • Data Analyst • Machine Learning Enthusiast • Competitive Programmer</p>
        </header>
        
        <hr>
        
        <section class="section" style="animation-delay: 0.1s">
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
        
        <section class="section" style="animation-delay: 0.2s">
            <h2>🎓 Academic Achievements</h2>
            <ul>
                <li><strong>10.0 SGPA in both first-year semesters</strong></li>
                <li><strong>Overall CGPA: 9.84</strong></li>
                <li><strong>Strong foundation in mathematics, algorithms, and core CS concepts</strong></li>
            </ul>
        </section>
        
        <section class="section" style="animation-delay: 0.3s">
            <h2>🚀 About Me</h2>
            <p>I'm a focused developer passionate about building real products, analyzing data, and exploring machine learning.</p>
            <p>I enjoy solving challenging problems, contributing to scalable systems, and continuously improving my technical depth.</p>
        </section>
        
        <section class="section" style="animation-delay: 0.4s">
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
            <p style="margin-top: 15px;"><strong>Full-stack MERN/Next.js applications</strong></p>
        </section>
        
        <section class="section" style="animation-delay: 0.5s">
            <h2>📊 Data Analysis & Machine Learning</h2>
            <div class="tech-stack">
                <div class="tech-item">Python</div>
                <div class="tech-item">NumPy</div>
                <div class="tech-item">Pandas</div>
                <div class="tech-item">Matplotlib</div>
                <div class="tech-item">Seaborn</div>
                <div class="tech-item">Scikit-learn</div>
            </div>
            <ul style="margin-top: 15px;">
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

    <script>
        // Simple script to add scroll animations without external libraries
        document.addEventListener('DOMContentLoaded', function() {
            // Add staggered animation to sections on scroll
            const sections = document.querySelectorAll('.section');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.animationPlayState = 'running';
                        observer.unobserve(entry.target);
                    }
                });
            }, { threshold: 0.1 });
            
            sections.forEach(section => {
                section.style.animationPlayState = 'paused';
                observer.observe(section);
            });
            
            // Add hover effect to social buttons
            const socialBtns = document.querySelectorAll('.social-btn');
            socialBtns.forEach(btn => {
                btn.addEventListener('mouseenter', function() {
                    this.style.transform = 'scale(1.1)';
                });
                btn.addEventListener('mouseleave', function() {
                    this.style.transform = 'scale(1)';
                });
            });
            
            // Add a subtle background animation
            let hue = 0;
            function updateBackground() {
                hue = (hue + 0.2) % 360;
                document.body.style.background = `linear-gradient(135deg, hsl(${hue}, 70%, 15%), hsl(${(hue + 30) % 360}, 70%, 25%), hsl(${(hue + 60) % 360}, 70%, 15%))`;
                requestAnimationFrame(updateBackground);
            }
            
            // Start the background animation
            updateBackground();
        });
    </script>
</body>
</html>
