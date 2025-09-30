<style>
  /* Base Styles */
  .overview-container {
    font-family: 'Montserrat', sans-serif;
    color: #333;
    line-height: 1.6;
  }
  .hero {
    padding: 40px;
    background: linear-gradient(135deg, #1d2671, #c33764);
    color: white;
    text-align: center;
  }
  .hero img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    border: 5px solid white;
  }
  .hero h1 {
    font-size: 3rem;
    margin: 20px 0 10px;
  }
  .hero p {
    font-size: 1.5rem;
  }
  .hero .buttons {
    margin-top: 20px;
  }
  .hero a, .hero button {
    margin: 0 10px;
    padding: 8px 15px;
    background: rgba(255,255,255,0.2);
    border-radius: 5px;
    color: white;
    font-weight: bold;
    text-decoration: none;
    border: none;
    cursor: pointer;
  }
  .about, .projects, .skills, .connect, .footer {
    padding: 40px;
    text-align: center;
  }
  .projects {
    background: #f5f5f5;
  }
  .project-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    margin-top: 30px;
  }
  .project-card {
    background: #fff;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    text-align: center;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  }
  .project-card i {
    font-size: 2rem;
    color: #c33764;
  }
  .skills .skill-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
    margin-top: 20px;
  }
  .skill {
    background: #fff;
    padding: 10px 20px;
    border-radius: 20px;
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 1.1rem;
  }
  .skill i {
    font-size: 2rem;
    color: #1d2671;
  }
  .connect a {
    color: white;
    margin: 0 10px;
    font-size: 2rem;
  }
  .footer {
    background: #333;
    color: white;
    padding: 20px 0;
  }
</style>

<div class="overview-container">
  <!-- Hero Section -->
  <div class="hero">
    <!-- Update 'profile-pic.jpg' with your actual profile image URL or relative path -->
    <img src="profile-pic.jpg" alt="Rourke V Profile">
    <h1>Rourke V</h1>
    <p>Software Developer & Designer</p>
    <div class="buttons">
      <a href="Rourke_Veller_CV.pdf" download>
        <i class="fas fa-download"></i> Download CV
      </a>
      <a href="https://github.com/RourkeV">
        <i class="fab fa-github"></i> GitHub
      </a>
    </div>
  </div>

  <!-- About Me Section -->
  <div class="about">
    <h2>About Me</h2>
    <p>
      I blend minimalistic design with state-of-the-art software development to create engaging digital experiences.
      My resume—crafted in a sleek black-and-white style using Canva—details my professional journey as both a developer and a designer.
      Browse my featured projects below and feel free to connect!
    </p>
  </div>

  <!-- Featured Projects Section -->
  <div class="projects">
    <h2>Featured Projects</h2>
    <div class="project-cards">
      <div class="project-card">
        <i class="fas fa-laptop-code"></i>
        <h3>Portfolio Website</h3>
        <p>A modern overview site showcasing my work.</p>
        <a href="https://github.com/RourkeV/portfolio-website" target="_blank" style="color: #1d2671; font-weight: bold;">View Repo</a>
      </div>
      <div class="project-card">
        <i class="fas fa-project-diagram"></i>
        <h3>rourkev</h3>
        <p>A curated collection of innovative projects.</p>
        <a href="https://github.com/RourkeV/rourkev" target="_blank" style="color: #1d2671; font-weight: bold;">View Repo</a>
      </div>
      <div class="project-card">
        <i class="fas fa-car"></i>
        <h3>LPR Solver</h3>
        <p>Collaborative project on license plate recognition.</p>
        <a href="https://github.com/GideonVermeulen/LPR_Solver" target="_blank" style="color: #1d2671; font-weight: bold;">View Repo</a>
      </div>
      <div class="project-card">
        <i class="fas fa-cogs"></i>
        <h3>PRG282 Project</h3>
        <p>A hands-on project developed during PRG282 coursework.</p>
        <a href="https://github.com/RourkeV/PRG282-Project" target="_blank" style="color: #1d2671; font-weight: bold;">View Repo</a>
      </div>
      <div class="project-card">
        <i class="fas fa-lightbulb"></i>
        <h3>M2-PRG381</h3>
        <p>An engaging project from the PRG381 module.</p>
        <a href="https://github.com/FreeYungHammy/M2-PRG381" target="_blank" style="color: #1d2671; font-weight: bold;">View Repo</a>
      </div>
    </div>
  </div>

  <!-- Skills & Tools Section -->
  <div class="skills">
    <h2>Skills & Tools</h2>
    <div class="skill-list">
      <div class="skill">
        <i class="fab fa-js-square"></i>
        <span>JavaScript</span>
      </div>
      <div class="skill">
        <i class="fab fa-python"></i>
        <span>Python</span>
      </div>
      <div class="skill">
        <i class="fas fa-code"></i>
        <span>C#</span>
      </div>
      <div class="skill">
        <i class="fab fa-java"></i>
        <span>Java</span>
      </div>
      <div class="skill">
        <i class="fab fa-react"></i>
        <span>React</span>
      </div>
      <div class="skill">
        <i class="fas fa-server"></i>
        <span>Node.js</span>
      </div>
      <div class="skill">
        <i class="fas fa-cloud"></i>
        <span>.NET</span>
      </div>
      <div class="skill">
        <i class="fas fa-pen-fancy"></i>
        <span>UX/UI Design</span>
      </div>
    </div>
  </div>

  <!-- Connect Section -->
  <div class="connect" style="background: #1d2671; color: white;">
    <h2>Connect with Me</h2>
    <p>
      <a href="mailto:your-email@example.com">
        <i class="fas fa-envelope"></i>
      </a>
      <a href="https://github.com/RourkeV">
        <i class="fab fa-github"></i>
      </a>
      <a href="https://www.linkedin.com/in/your-profile">
        <i class="fab fa-linkedin"></i>
      </a>
    </p>
    <p>Feel free to reach out for collaborations or just to say hi!</p>
  </div>

  <!-- Footer -->
  <div class="footer">
    <p>&copy; 2025 Rourke V. All rights reserved.</p>
  </div>
</div>