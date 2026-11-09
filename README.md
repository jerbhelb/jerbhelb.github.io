# jerbhelb.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Your Name | Portfolio</title>
  <style>
    /* Global Styles */
    :root {
      --bg-color: #0d1117;
      --card-bg: #161b22;
      --border-color: #30363d;
      --text-main: #c9d1d9;
      --text-muted: #8b949e;
      --accent: #58a6ff;
      --accent-hover: #1f6feb;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      background-color: var(--bg-color);
      color: var(--text-main);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Header & Navigation */
    header {
      position: sticky;
      top: 0;
      background-color: rgba(13, 17, 23, 0.9);
      backdrop-filter: blur(8px);
      border-bottom: 1px solid var(--border-color);
      z-index: 100;
    }

    nav {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
    }

    nav .logo {
      font-size: 1.2rem;
      font-weight: bold;
      color: #fff;
    }

    nav ul {
      display: flex;
      list-style: none;
      gap: 1.5rem;
    }

    /* Container */
    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    section {
      margin-bottom: 4rem;
    }

    h2 {
      font-size: 1.8rem;
      margin-bottom: 1.5rem;
      border-bottom: 1px solid var(--border-color);
      padding-bottom: 0.5rem;
      color: #fff;
    }

    /* Hero Section */
    .hero {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      gap: 1rem;
      padding: 4rem 0 2rem;
    }

    .hero h1 {
      font-size: 3rem;
      color: #fff;
    }

    .hero p {
      font-size: 1.25rem;
      color: var(--text-muted);
      max-width: 600px;
    }

    .btn {
      display: inline-block;
      background-color: var(--accent);
      color: #fff;
      padding: 0.75rem 1.5rem;
      border-radius: 6px;
      font-weight: 600;
      margin-top: 1rem;
    }

    .btn:hover {
      background-color: var(--accent-hover);
      text-decoration: none;
    }

    /* Projects Grid */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background-color: var(--card-bg);
      border: 1px solid var(--border-color);
      border-radius: 8px;
      padding: 1.5rem;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .card h3 {
      color: #fff;
      margin-bottom: 0.5rem;
    }

    .card p {
      color: var(--text-muted);
      font-size: 0.95rem;
      margin-bottom: 1rem;
    }

    .card .tags {
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
      margin-bottom: 1rem;
    }

    .tag {
      background-color: rgba(88, 166, 255, 0.1);
      color: var(--accent);
      padding: 0.2rem 0.6rem;
      border-radius: 12px;
      font-size: 0.8rem;
    }

    /* Skills List */
    .skills-list {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
    }

    .skill-item {
      background-color: var(--card-bg);
      border: 1px solid var(--border-color);
      padding: 0.5rem 1rem;
      border-radius: 6px;
      font-size: 0.95rem;
    }

    /* Contact & Footer */
    footer {
      border-top: 1px solid var(--border-color);
      padding: 2rem 0;
      text-align: center;
      color: var(--text-muted);
      font-size: 0.9rem;
    }

    .social-links {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin-bottom: 1rem;
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <header>
    <nav>
      <div class="logo">Jane Doe</div>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <!-- Hero Section -->
    <section class="hero">
      <h1>Hi, I'm Jane Doe 👋</h1>
      <p>A passionate Full-Stack Developer specializing in building scalable web applications and open-source software.</p>
      <a href="#projects" class="btn">View My Work</a>
    </section>

    <!-- About Section -->
    <section id="about">
      <h2>About Me</h2>
      <p>
        I have over 3 years of experience writing clean, maintainable code. My primary focus is on modern JavaScript frameworks, backend APIs, and cloud infrastructure. When I'm not coding, I enjoy contributing to open-source projects and writing technical blog posts.
      </p>
    </section>

    <!-- Projects Section -->
    <section id="projects">
      <h2>Featured Projects</h2>
      <div class="grid">
        
        <!-- Project 1 -->
        <div class="card">
          <div>
            <h3>E-Commerce Dashboard</h3>
            <p>A real-time analytics dashboard for online store owners featuring sales metrics, inventory tracking, and customer management.</p>
            <div class="tags">
              <span class="tag">React</span>
              <span class="tag">Node.js</span>
              <span class="tag">MongoDB</span>
            </div>
          </div>
          <a href="https://github.com/yourusername/project-one" target="_blank">View on GitHub →</a>
        </div>

        <!-- Project 2 -->
        <div class="card">
          <div>
            <h3>Task Automation CLI</h3>
            <p>A command-line tool built to automate repetitive developer workflows, environment setup, and deployment processes.</p>
            <div class="tags">
              <span class="tag">Python</span>
              <span class="tag">Docker</span>
              <span class="tag">Bash</span>
            </div>
          </div>
          <a href="https://github.com/yourusername/project-two" target="_blank">View on GitHub →</a>
        </div>

        <!-- Project 3 -->
        <div class="card">
          <div>
            <h3>Portfolio Web App</h3>
            <p>A lightweight, dark-themed personal portfolio website hosted seamlessly using GitHub Pages.</p>
            <div class="tags">
              <span class="tag">HTML5</span>
              <span class="tag">CSS3</span>
              <span class="tag">JavaScript</span>
            </div>
          </div>
          <a href="https://github.com/yourusername/project-three" target="_blank">View on GitHub →</a>
        </div>

      </div>
    </section>

    <!-- Skills Section -->
    <section id="skills">
      <h2>Skills & Technologies</h2>
      <div class="skills-list">
        <div class="skill-item">JavaScript (ES6+)</div>
        <div class="skill-item">TypeScript</div>
        <div class="skill-item">React / Next.js</div>
        <div class="skill-item">Node.js / Express</div>
        <div class="skill-item">Python</div>
        <div class="skill-item">HTML5 / CSS3</div>
        <div class="skill-item">Git / GitHub</div>
        <div class="skill-item">Docker</div>
        <div class="skill-item">RESTful APIs</div>
        <div class="skill-item">PostgreSQL / MongoDB</div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
      <h2>Get In Touch</h2>
      <p>I am currently open to new opportunities and collaborations. Feel free to reach out!</p>
      <p style="margin-top: 1rem;">
        Email: <a href="mailto:janedoe@example.com">janedoe@example.com</a>
      </p>
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <div class="social-links">
      <a href="https://github.com/yourusername" target="_blank">GitHub</a>
      <a href="https://linkedin.com/in/yourusername" target="_blank">LinkedIn</a>
      <a href="https://x.com/yourusername" target="_blank">X (Twitter)</a>
    </div>
    <p>&copy; 2026 Jane Doe. Built with HTML & CSS.</p>
  </footer>

</body>
</html>
