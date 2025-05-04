# PRODIGY_WD_04
My Portfolio as a Web Developer 

<!DOCTYPE html>
<html lang="en">
<head>
  <title>My Portfolio</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff;
      color: #333;
    }

    a {
      text-decoration: none;
    }

    ul {
      padding: 0;
      margin: 0;
      list-style-type: none;
    }

    /* Navbar */
    #navbar {
      position: fixed;
      width: 100%;
      top: 0;
      background-color: #a2d5f2;
      padding: 10px 0;
      z-index: 1000;
      box-shadow: 0 1px 4px rgba(0, 0, 0, 0.08);
      transition: background-color 0.3s;
    }

    #navbar.scrolled {
      background-color: #89c2d9;
    }

    #navbar ul {
      display: flex;
      justify-content: center;
    }

    #navbar ul li {
      margin: 0 15px;
    }

    #navbar ul li a {
      color: white;
      padding: 8px 15px;
      border-radius: 5px;
      transition: background 0.3s, color 0.3s;
    }

    #navbar ul li a:hover {
      background-color: #fdf0f0;
      color: #333;
    }

    /* Sections */
    .content {
      padding-top: 70px;
    }

    section {
      padding: 60px 20px;
      text-align: center;
    }

    section:nth-child(even) {
      background-color: #f1f9f9;
    }

    /* Home Section */
    .home-container {
      max-width: 600px;
      margin: auto;
    }

    .profile-photo {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      margin-bottom: 20px;
      object-fit: cover;
      border: 4px solid #d0e8f2;
    }

    .highlight {
      color: #3498db;
    }

    /* Lists */
    section ul {
      max-width: 600px;
      margin: 20px auto;
      text-align: left;
    }

    section ul li {
      padding: 10px 0;
      border-bottom: 1px solid #ddd;
    }

    /* Contact Links */
    #contact a {
      color: #3498db;
    }

    /* Responsive */
    @media (max-width: 600px) {
      nav ul {
        flex-direction: column;
        align-items: center;
      }
      nav ul li {
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav id="navbar">
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About Me</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Page Content -->
  <div class="content">
    <!-- Home Section -->
    <section id="home">
      <div class="home-container">
        <img src="https://via.placeholder.com/150" alt="Profile Photo" class="profile-photo" />
        <h1>Hello, I'm <span class="highlight">Sreeja Reddy</span></h1>
        <p>I'm a passionate web developer skilled in HTML, CSS, JavaScript, and modern web frameworks.</p>
      </div>
    </section>

    <!-- About Section -->
    <section id="about">
      <h2>About Me</h2>
      <p>I’m a web developer with a strong interest in front-end development, UI/UX design, and responsive web applications.</p>
      <ul>
        <li><strong>Education:</strong> B.Tech in Computer Science</li>
        <li><strong>Experience:</strong> Internships at Prodigy InfoTech</li>
        <li><strong>Skills:</strong> HTML, CSS, JavaScript, React, Git, UI Design</li>
      </ul>
    </section>

    <!-- Projects Section -->
    <section id="projects">
      <h2>Projects</h2>
      <ul>
        <li><strong>Portfolio Website:</strong> Designed with HTML/CSS</li>
        <li><strong>ToDo List App:</strong> JavaScript DOM Project</li>
        <li><strong>Weather Forecast App:</strong> Uses OpenWeatherMap API</li>
      </ul>
    </section>

    <!-- Contact Section -->
    <section id="contact">
      <h2>Contact</h2>
      <p>Email: skondaka3@gitam.in</p>
      <p>LinkedIn: <a href="https://linkedin.com/in/kondakallasreeja" target="_blank">linkedin.com/in/kondakallasreeja</a></p>
    </section>
  </div>

  <!-- JavaScript for Scroll -->
  <script>
    window.addEventListener('scroll', () => {
      const nav = document.getElementById('navbar');
      nav.classList.toggle('scrolled', window.scrollY > 50);
    });
  </script>

</body>
</html>
