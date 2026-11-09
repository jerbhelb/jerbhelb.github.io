<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Developer Portfolio</title>
  <style>
    /* CSS Variables & Theme Setup */
    :root {
      --bg: #0d1117;
      --panel: #161b22;
      --border: #30363d;
      --text: #c9d1d9;
      --heading: #ffffff;
      --muted: #8b949e;
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
      background-color: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Header & Navbar */
    header {
      position: sticky;
      top: 0;
      background-color: rgba(13, 17, 23, 0.85);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--border);
      z-index: 100;
    }

    nav {
      max-width: 1000px;
      margin: 0 auto;
      padding: 1rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .brand {
      font-weight: 700;
      font-size: 1.2rem;
      color: var(--heading);
    }

    .nav-links {
      display: flex;
      gap: 1.5rem;
      list-style: none;
    }

    /* Layout Container */
    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 3rem 1.5rem;
    }

    section {
      margin-bottom: 4rem;
    }

    h2 {
      font-size: 1.75rem;
      color: var(--heading);
      border-bottom: 1px solid var(--border);
      padding-bottom: 0.5rem;
      margin-bottom: 1.5rem;
    }

    /* Hero Section */
    .hero {
      padding: 3rem 0;
    }

    .hero h1 {
      font-size: 2.8rem;
      color: var(--heading);
      margin-bottom: 0.5rem;
    }

    .hero p {
      font-size: 1.2rem;
      color: var(--muted);
      max-width: 650px;
      margin-bottom: 1.5rem;
    }

    .btn {
      display: inline-block;
      background-color: var(--accent);
      color: #ffffff;
      padding: 0.6rem 1.2rem;
      border-radius: 6px;
      font-weight: 600;
    }

    .btn:hover {
      background-color: var(--accent-hover);
      text-decoration: none;
    }

    /* Cards Grid */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background-color: var(--panel);
      border: 1px solid var(--border);
      border-radius: 8px;
      padding: 1.5rem;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .card h3 {
      color: var(--heading);
      margin-bottom: 0.5rem;
    }

    .card p {
      color: var(--muted);
      font-size: 0.95rem;
      margin-bottom: 1rem;
    }

    .tags {
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
      margin-bottom: 1rem;
    }

    .tag {
      background-color: rgba(88, 166, 255, 0.1);
      color: var(--accent);
      font-size: 0.8rem;
      padding: 0.2rem 0.5rem;
      border-radius: 12px;
    }

    /* Skills Badges */
    .skills-wrapper {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
    }

    .skill-badge {
      background-color: var(--panel);
      border: 1px solid var(--border);
      padding: 0.5rem 1rem;
      border-radius: 6px;
      font-size: 0.9rem;
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--border);
      padding: 2rem 1.5rem;
      text-align: center;
      color: var(--muted);
      font-size: 0.9rem;
    }

    .socials {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin-bottom: 1rem;
    }
  </style>
</head>
<body>

  <header>
    <nav>
      <div class="brand">Jerbhel</div>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="container">
    <section class="hero">
      <h1>Hello, I'm Jerbhel Beltran</h1>
      <p>An aspiring individual that aims to pursue Data Analytics and Sciences.</p>
      <a href="#projects" class="btn">View Projects</a>
    </section>

    <section id="about">
      <h2>About Me</h2>
      <p>
        I specialize in web development, working primarily with JavaScript, HTML/CSS, and backend systems. 
        This site is hosted directly using GitHub Pages.
      </p>
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <div class="grid">
        <div class="card">
          <div>
            <h3>Project One</h3>
            <p>A web dashboard built to track real-time analytics and user data.</p>
            <div class="tags">
              <span class="tag">HTML</span>
              <span class="tag">CSS</span>
              <span class="tag">JS</span>
            </div>
          </div>
          <a href="https://github.com/yourusername/project-one" target="_blank">Repository →</a>
        </div>

        <div class="card">
          <div>
            <h3>Project Two</h3>
            <p>A command-line interface tool designed for automated build workflows.</p>
            <div class="tags">
              <span class="tag">Node.js</span>
              <span class="tag">CLI</span>
            </div>
          </div>
          <a href="https://github.com/yourusername/project-two" target="_blank">Repository →</a>
        </div>
      </div>
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <div class="skills-wrapper">
        <span class="skill-badge">HTML5 / CSS3</span>
        <span class="skill-badge">JavaScript</span>
        <span class="skill-badge">Git & GitHub</span>
