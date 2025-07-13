<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sidebar Portfolio with Photo</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      display: flex;
      min-height: 100vh;
      background: linear-gradient(to right, #f0f4f8, #e0eafc);
      color: #333;
    }

    /* Sidebar */
    .sidebar {
      width: 220px;
      background-color: #1f2937;
      color: white;
      padding: 30px 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      position: fixed;
      height: 100vh;
    }

    .profile-img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 3px solid #00d9ff;
      object-fit: cover;
      margin-bottom: 15px;
    }

    .sidebar h1 {
      font-size: 20px;
      color: #00d9ff;
      text-align: center;
      margin-bottom: 30px;
    }

    nav ul {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 15px;
      width: 100%;
      align-items: center;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-size: 16px;
      padding: 8px 14px;
      border-radius: 6px;
      transition: background 0.3s;
    }

    nav a:hover {
      background-color: #00d9ff;
      color: #000;
    }

    /* Main Content */
    .main {
      margin-left: 240px;
      padding: 40px;
      flex: 1;
    }

    section {
      margin-bottom: 60px;
    }

    h2 {
      color: #1f2937;
      margin-bottom: 15px;
      border-bottom: 3px solid #00d9ff;
      display: inline-block;
      padding-bottom: 5px;
    }

    p {
      font-size: 16px;
      line-height: 1.6;
      max-width: 800px;
    }

    .project {
      background: #fff;
      padding: 20px;
      margin: 20px 0;
      border-left: 5px solid #00d9ff;
      border-radius: 8px;
      box-shadow: 0 0 8px rgba(0,0,0,0.1);
    }

    footer {
      text-align: center;
      padding: 20px;
      color: #777;
    }

    @media (max-width: 768px) {
      body {
        flex-direction: column;
      }

      .sidebar {
        position: static;
        width: 100%;
        height: auto;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
      }

      nav ul {
        flex-direction: row;
        gap: 10px;
      }

      .main {
        margin-left: 0;
        padding: 20px;
      }

      .profile-img {
        width: 60px;
        height: 60px;
        margin-bottom: 0;
      }

      .sidebar h1 {
        font-size: 16px;
        margin-bottom: 0;
      }
    }
  </style>
</head>
<body>

  <div class="sidebar">
    <h1>Krishnam Soni</h1>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </div>

  <div class="main">
    <section id="about">
      <h2>About Me</h2>
      <p>Hello! I'm a web developer passionate about creating clean, creative, and responsive websites. I love turning ideas into reality using code.</p>
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <div class="project">
        <h3>Personal Portfolio</h3>
        <p>A modern, single-page portfolio using HTML and CSS with responsive layout.</p>
      </div>
  
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <p>Email: krishnamsni413@gmail.com</p>
    </section>

    <footer>
      <p>&copy; 2025 Krishna Soni. All rights reserved.</p>
    </footer>
  </div>

</body>
</html>
