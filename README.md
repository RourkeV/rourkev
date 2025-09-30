<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rourke Veller | Software Engineering Student</title>
    <style>
        :root {
            --primary: #2d5a7a;
            --secondary: #4a8cbf;
            --accent: #ff6b35;
            --light: #f8f9fa;
            --dark: #343a40;
            --gray: #6c757d;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 60px 0;
            text-align: center;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid white;
            margin: 0 auto 20px;
            background-color: #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .tagline {
            font-size: 1.2rem;
            margin-bottom: 20px;
            opacity: 0.9;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        section {
            padding: 60px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--primary);
            position: relative;
        }
        
        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 3px;
            background-color: var(--accent);
            margin: 10px auto;
        }
        
        .about-content {
            display: flex;
            flex-direction: column;
            gap: 20px;
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .skill-category {
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .skill-category h3 {
            color: var(--primary);
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid #eee;
        }
        
        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill-tag {
            background-color: var(--light);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: var(--dark);
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
        }
        
        .project-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
        }
        
        .project-img {
            height: 180px;
            background-color: #eee;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--gray);
        }
        
        .project-content {
            padding: 20px;
        }
        
        .project-title {
            color: var(--primary);
            margin-bottom: 10px;
        }
        
        .project-description {
            color: var(--gray);
            margin-bottom: 15px;
            font-size: 0.95rem;
        }
        
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 15px;
        }
        
        .tech-tag {
            background-color: var(--secondary);
            color: white;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
        }
        
        .btn {
            display: inline-block;
            padding: 8px 16px;
            background-color: var(--primary);
            color: white;
            text-decoration: none;
            border-radius: 4px;
            font-size: 0.9rem;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: var(--secondary);
        }
        
        .experience-item {
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            margin-bottom: 20px;
        }
        
        .experience-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }
        
        .experience-title {
            color: var(--primary);
            font-weight: 600;
        }
        
        .experience-date {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        .experience-company {
            color: var(--secondary);
            margin-bottom: 10px;
        }
        
        .experience-description {
            color: var(--dark);
        }
        
        footer {
            background-color: var(--dark);
            color: white;
            padding: 40px 0;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        
        .social-link {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .social-link:hover {
            color: var(--accent);
        }
        
        @media (max-width: 768px) {
            .skills-container, .projects-grid {
                grid-template-columns: 1fr;
            }
            
            .experience-header {
                flex-direction: column;
                gap: 5px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="profile-img">RV</div>
            <h1>Rourke Veller</h1>
            <p class="tagline">Software Engineering Student | Full-Stack Developer | Entrepreneur</p>
            <div class="contact-info">
                <div class="contact-item">
                    <span>📧</span>
                    <span>rourke@nitida.co.za</span>
                </div>
                <div class="contact-item">
                    <span>📱</span>
                    <span>+27 82 800 5235</span>
                </div>
                <div class="contact-item">
                    <span>📍</span>
                    <span>Stellenbosch, South Africa</span>
                </div>
            </div>
        </div>
    </header>

    <section id="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="about-content">
                <p>Sociable, solutions-oriented, and driven Software Engineering student currently in my third year at Belgium Campus ITversity, with a keen interest for problem-solving, innovation, and teamwork.</p>
                <p>I offer a unique mix of technical proficiency, business initiative, and leadership skills. I excel in collaborative environments and take initiative when new opportunities arise.</p>
                <p>I bring not just a strong academic foundation in software engineering but also real-world entrepreneurial experience, having successfully established and operated a café on campus.</p>
                <p>I am now seeking a dynamic and challenging internship for my 4th-year industry placement, where I can learn from industry professionals and contribute meaningfully to their business while growing as a developer.</p>
            </div>
        </div>
    </section>

    <section id="skills">
        <div class="container">
            <h2 class="section-title">Technical Skills</h2>
            <div class="skills-container">
                <div class="skill-category">
                    <h3>Programming Languages</h3>
                    <div class="skills-list">
                        <span class="skill-tag">Java</span>
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">C#</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">SQL</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Web Technologies</h3>
                    <div class="skills-list">
                        <span class="skill-tag">HTML5</span>
                        <span class="skill-tag">CSS</span>
                        <span class="skill-tag">Node.js</span>
                        <span class="skill-tag">Express.js</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Databases</h3>
                    <div class="skills-list">
                        <span class="skill-tag">PostgreSQL</span>
                        <span class="skill-tag">MySQL</span>
                        <span class="skill-tag">MongoDB</span>
                        <span class="skill-tag">Apache Derby</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Tools & Methodologies</h3>
                    <div class="skills-list">
                        <span class="skill-tag">Git</span>
                        <span class="skill-tag">GitHub</span>
                        <span class="skill-tag">Visual Studio</span>
                        <span class="skill-tag">VS Code</span>
                        <span class="skill-tag">IntelliJ IDEA</span>
                        <span class="skill-tag">Postman</span>
                        <span class="skill-tag">Docker</span>
                        <span class="skill-tag">OOP</span>
                        <span class="skill-tag">MVC</span>
                        <span class="skill-tag">REST APIs</span>
                        <span class="skill-tag">Agile (Scrum)</span>
                        <span class="skill-tag">Clean Code</span>
                        <span class="skill-tag">Unit Testing</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="projects">
        <div class="container">
            <h2 class="section-title">Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-img">Project Image</div>
                    <div class="project-content">
                        <h3 class="project-title">Student Information System</h3>
                        <p class="project-description">Led a team in designing and developing a student record management system in C# with Apache Derby for secure data storage and CRUD functionalities.</p>
                        <div class="project-tech">
                            <span class="tech-tag">C#</span>
                            <span class="tech-tag">Apache Derby</span>
                            <span class="tech-tag">SQL</span>
                        </div>
                        <a href="#" class="btn">View on GitHub</a>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-img">Project Image</div>
                    <div class="project-content">
                        <h3 class="project-title">Dating Application</h3>
                        <p class="project-description">Designed and developed a functional dating app with user authentication, profile creation, matching, and messaging features.</p>
                        <div class="project-tech">
                            <span class="tech-tag">C#</span>
                            <span class="tech-tag">Visual Studio</span>
                            <span class="tech-tag">Git</span>
                        </div>
                        <a href="#" class="btn">View on GitHub</a>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-img">Project Image</div>
                    <div class="project-content">
                        <h3 class="project-title">E-commerce Website</h3>
                        <p class="project-description">Full-stack e-commerce platform developed as part of academic coursework with product listings, cart functionality, and user accounts.</p>
                        <div class="project-tech">
                            <span class="tech-tag">JavaScript</span>
                            <span class="tech-tag">HTML/CSS</span>
                            <span class="tech-tag">Node.js</span>
                            <span class="tech-tag">MySQL</span>
                        </div>
                        <a href="#" class="btn">View on GitHub</a>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-img">Project Image</div>
                    <div class="project-content">
                        <h3 class="project-title">Mobile Expense Tracker</h3>
                        <p class="project-description">Mobile application for tracking personal expenses with categorization, reporting, and budget management features.</p>
                        <div class="project-tech">
                            <span class="tech-tag">Java</span>
                            <span class="tech-tag">Android</span>
                            <span class="tech-tag">SQLite</span>
                        </div>
                        <a href="#" class="btn">View on GitHub</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="experience">
        <div class="container">
            <h2 class="section-title">Experience</h2>
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="experience-title">Founder & Operator</h3>
                    <span class="experience-date">2023 – 2025</span>
                </div>
                <p class="experience-company">Campus Café, Belgium Campus</p>
                <p class="experience-description">
                    Identified a gap in campus services and launched a profitable café/tuckshop. Managed business operations including procurement, customer service, finances, inventory, and team supervision. Hired and supervised fellow students, fostering teamwork in a fast-paced environment. Applied entrepreneurial thinking and leadership daily while balancing academics.
                </p>
            </div>
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="experience-title">Pizza Delivery</h3>
                    <span class="experience-date">2021 – 2022</span>
                </div>
                <p class="experience-company">Pete's Pizza</p>
                <p class="experience-description">
                    Delivered orders promptly and accurately while maintaining high customer satisfaction. Handled cash and card transactions, managed receipts, and ensured secure delivery. Communicated effectively with customers and team members to resolve issues and coordinate deliveries. Demonstrated reliability, accountability, and professionalism.
                </p>
            </div>
        </div>
    </section>

    <section id="education">
        <div class="container">
            <h2 class="section-title">Education</h2>
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="experience-title">BSc in Computing (Software Engineering)</h3>
                    <span class="experience-date">2023 – Present</span>
                </div>
                <p class="experience-company">Belgium Campus ITversity, Stellenbosch, SA</p>
                <p class="experience-description">
                    Specialized in full-stack development, databases, and systems analysis. Key Modules: Software Design, Web Technologies, OOP, Databases, Mobile Dev, Algorithms.
                </p>
            </div>
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="experience-title">Software Engineering Bootcamp</h3>
                    <span class="experience-date">2022</span>
                </div>
                <p class="experience-company">HyperionDev (Online)</p>
                <p class="experience-description">
                    Intensive year-long course covering front-end, back-end, and full-stack software development, Git, Clean code and debugging. Built real-world applications and completed coding challenges.
                </p>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="footer-content">
                <p>Interested in working together? I'm always open to discussing new opportunities.</p>
                <div class="social-links">
                    <a href="https://github.com/RourkeV" class="social-link">GitHub</a>
                    <a href="mailto:rourke@nitida.co.za" class="social-link">Email</a>
                    <a href="#" class="social-link">LinkedIn</a>
                </div>
                <p>&copy; 2025 Rourke Veller. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>