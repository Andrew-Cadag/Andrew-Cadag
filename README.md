<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ronald Andrew D. Cadag's Portfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <script src="https://kit.fontawesome.com/your-fontawesome-kit.js" crossorigin="anonymous"></script> <style>
        /* CSS Variables for Easy Theme Customization */
        :root {
            --bg-color: #0D1117;
            --primary-text: #CDD6F4;
            --secondary-text: #A6ADC8;
            --border-color: #30363D;
            --card-bg: #161B22;
            --accent-gradient: linear-gradient(90deg, #00F6FF, #7289DA, #00F6FF);
            --font-main: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
        }

        /* General Body Styling */
        body {
            background-color: var(--bg-color);
            color: var(--primary-text);
            font-family: var(--font-main);
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 2rem;
        }

        /* Main Container */
        .container {
            max-width: 900px;
            width: 100%;
            background-color: var(--bg-color);
            border: 1px solid var(--border-color);
            border-radius: 15px;
            padding: 2.5rem;
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        }

        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 3rem;
        }

        .name {
            font-size: clamp(2.5rem, 5vw, 4rem); /* Responsive font size */
            font-weight: 900;
            letter-spacing: -2.5px;
            background: var(--accent-gradient);
            background-size: 200% 200%;
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradient-animation 4s ease infinite;
            margin: 0;
            line-height: 1.2;
        }

        @keyframes gradient-animation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .title {
            font-size: clamp(1.1rem, 2vw, 1.25rem);
            font-weight: 500;
            color: var(--secondary-text);
            margin-top: 0.5rem;
            margin-bottom: 1.5rem;
        }
        
        /* Social Links */
        .socials {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
        }

        .socials a {
            color: var(--secondary-text);
            font-size: 1.5rem;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        .socials a:hover {
            color: #7289DA;
            transform: scale(1.1);
        }

        /* Section Styling */
        .section {
            margin-bottom: 2.5rem;
        }

        .section-title {
            font-size: 1.75rem;
            font-weight: 700;
            color: var(--primary-text);
            margin-bottom: 1.5rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid var(--border-color);
        }
        
        /* About Me Section */
        .about-me p {
            font-size: 1.1rem;
            line-height: 1.6;
            color: var(--secondary-text);
        }

        /* Tech Stack Section */
        .tech-stack-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 1.5rem;
        }
        
        .tech-category {
            background-color: var(--card-bg);
            padding: 1.5rem;
            border-radius: 10px;
            border: 1px solid var(--border-color);
        }

        .tech-category h4 {
            font-size: 1.1rem;
            font-weight: 500;
            margin-top: 0;
            margin-bottom: 1rem;
            color: var(--primary-text);
        }

        .tech-category ul {
            list-style: none;
            padding: 0;
            margin: 0;
            color: var(--secondary-text);
        }
        
        /* Project Cards */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .project-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 10px;
            padding: 1.5rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 20px rgba(0, 246, 255, 0.1);
        }

        .project-card h3 {
            font-size: 1.25rem;
            margin-top: 0;
            margin-bottom: 0.75rem;
            color: #7289DA;
        }

        .project-card p {
            font-size: 1rem;
            color: var(--secondary-text);
            line-height: 1.5;
            margin-bottom: 1rem;
        }
        
        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tag {
            background-color: #30363D;
            color: var(--primary-text);
            padding: 0.25rem 0.75rem;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        /* GitHub Stats Section */
        .github-stats {
            text-align: center;
        }
        
        .github-stats img {
            max-width: 100%;
            margin: 0.5rem;
        }

    </style>
</head>
<body>

    <div class="container">
        <header class="header">
            <h1 class="name">RONALD ANDREW D. CADAG</h1>
            <p class="title">IT Student @ Mapua University | Aspiring Software Engineer</p>
            <div class="socials">
                <a href="#" target="_blank" title="GitHub"><i class="fab fa-github"></i></a>
                <a href="#" target="_blank" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
                <a href="#" target="_blank" title="Personal Website"><i class="fas fa-globe"></i></a>
            </div>
        </header>

        <section class="section about-me">
            <h2 class="section-title">About Me</h2>
            <p>
                A passionate and driven Information Technology student, building upon a foundational year in Computer Engineering. My focus is on the intersection of robust engineering and human-centered design to create intuitive, data-informed digital systems. I am actively seeking opportunities to apply my academic knowledge and project experience to solve real-world challenges.
            </p>
        </section>

        <section class="section">
            <h2 class="section-title">My Tech Stack 🛠️</h2>
            <div class="tech-stack-grid">
                <div class="tech-category">
                    <h4>Languages</h4>
                    <ul>
                        <li>C++</li>
                        <li>Java</li>
                        <li>Python</li>
                        <li>HTML/CSS</li>
                        <li>JavaScript</li>
                    </ul>
                </div>
                <div class="tech-category">
                    <h4>Databases & Platforms</h4>
                    <ul>
                        <li>MySQL</li>
                        <li>Firebase</li>
                        <li>Git & GitHub</li>
                        <li>Linux/Unix Shell</li>
                    </ul>
                </div>
                <div class="tech-category">
                    <h4>Design & Frameworks</h4>
                    <ul>
                        <li>Figma</li>
                        <li>React (Learning)</li>
                        <li>Node.js (Learning)</li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="section">
            <h2 class="section-title">Featured Projects & Research 💼</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>A Comparative Study of KDA in Valorant</h3>
                    <p>Quantitative analysis modeling the impact of in-game metrics (KDA, ADR) on match outcomes, identifying key indicators of player success.</p>
                    <div class="project-tags">
                        <span class="tag">Data Analysis</span>
                        <span class="tag">User Behavior</span>
                        <span class="tag">Statistics</span>
                    </div>
                </div>
                <div class="project-card">
                    <h3>[Concept] Command-Line Database App</h3>
                    <p>Conceptual design of a C++ CLI application for student record management, applying principles from Information Management and Data Structures.</p>
                    <div class="project-tags">
                        <span class="tag">C++</span>
                        <span class="tag">Data Structures</span>
                        <span class="tag">CLI</span>
                        <span class="tag">System Design</span>
                    </div>
                </div>
            </div>
        </section>

        <section class="section">
            <h2 class="section-title">GitHub Statistics 📊</h2>
            <div class="github-stats">
                <img src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=transparent&text_color=cdd6f4&icon_color=7289da" alt="GitHub Stats">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=transparent&text_color=cdd6f4&icon_color=7289da" alt="Top Languages">
            </div>
        </section>

    </div>

</body>
</html>
