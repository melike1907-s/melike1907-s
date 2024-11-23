<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>My Personal Blog</title>

  <!-- Internal CSS -->
  <style>
    /* Reset styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background-color: #f4f4f4;
      color: #333;
    }

    header {
      background: #333;
      color: #fff;
      padding: 10px 0;
      text-align: center;
    }

    nav ul {
      list-style: none;
      padding: 0;
    }

    nav ul li {
      display: inline;
      margin: 0 20px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    .hero {
      background: #333 url('https://via.placeholder.com/1200x500') no-repeat center center/cover;
      color: white;
      padding: 80px 0;
      text-align: center;
    }

    .hero h1 {
      font-size: 2.5em;
    }

    .hero p {
      font-size: 1.2em;
    }

    .post-preview, .post {
      background: white;
      padding: 20px;
      margin: 20px 0;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .post-preview h3 a, .post h3 a {
      color: #333;
      text-decoration: none;
    }

    .post-preview p, .post p {
      font-size: 1em;
      color: #666;
    }

    .post h3, .post-preview h3 {
      font-size: 1.8em;
      color: #333;
    }

    .post img {
      width: 100%;
      height: auto;
      border-radius: 5px;
    }

    footer {
      background: #333;
      color: white;
      padding: 10px 0;
      text-align: center;
      margin-top: 20px;
    }

    .contact form input,
    .contact form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ddd;
      border-radius: 5px;
    }

    .contact form button {
      background: #333;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .contact form button:hover {
      background: #444;
    }

    .gallery img {
      width: 30%;
      margin: 10px;
      border-radius: 5px;
      transition: transform 0.3s ease;
    }

    .gallery img:hover {
      transform: scale(1.1);
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      nav ul li {
        display: block;
        text-align: center;
        margin: 10px 0;
      }

      .post-preview, .post {
        margin: 20px auto;
        width: 90%;
      }

      .gallery img {
        width: 100%;
        margin-bottom: 20px;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Home Section -->
  <section id="home" class="hero">
    <h1>Welcome to My Personal Blog!</h1>
    <p>Explore my articles, thoughts, and creativity.</p>
  </section>

  <!-- Featured Blog Posts -->
  <section id="blog" class="featured-posts">
    <h2>Featured Posts</h2>
    <div class="post-preview">
      <h3><a href="#post1">How to Stay Productive</a></h3>
      <p>Learn my top tips for staying focused and achieving your goals every day.</p>
    </div>
    <div class="post-preview">
      <h3><a href="#post2">The Power of Minimalism</a></h3>
      <p>Discover the benefits of living with less and creating a simplified lifestyle.</p>
    </div>
  </section>

  <!-- Blog Post Details (Post 1) -->
  <section id="post1" class="post">
    <h3>How to Stay Productive</h3>
    <p>Published on: January 15, 2024</p>
    <p>In this article, I'll share my best productivity tips and tricks to help you stay focused and get more done each day. It's all about mindset, routines, and managing distractions effectively.</p>
  </section>

  <!-- Blog Post Details (Post 2) -->
  <section id="post2" class="post">
    <h3>The Power of Minimalism</h3>
    <p>Published on: January 10, 2024</p>
    <p>Minimalism isn't just about decluttering your physical space; it's about simplifying your life to focus on what really matters. In this post, I share how embracing minimalism can lead to a happier, more fulfilled life.</p>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <p>Hi! I'm <strong>Melike Çetin</strong>, a software engineering student and lifelong learner. On this blog, I share my thoughts on productivity, minimalism, and personal growth. I hope my articles inspire you to live a simpler, more focused life.</p>
  </section>

  <!-- Gallery Section -->
  <section id="gallery" class="gallery">
    <h2>My Gallery</h2>
    <div>
      <img src="https://via.placeholder.com/300x300" alt="Gallery Image 1">
      <img src="https://via.placeholder.com/300x300" alt="Gallery Image 2">
      <img src="https://via.placeholder.com/300x300" alt="Gallery Image 3">
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <form id="contact-form">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="message">Message:</label>
      <textarea id="message" name="message" required></textarea>

      <button type="submit">Send Message</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>Copyright © 2024 - Melike Çetin's Blog</p>
  </footer>

  <!-- Internal JavaScript -->
  <script>
    // Simple form validation for the contact form
    document.getElementById('contact-form').addEventListener('submit', function(event) {
      event.preventDefault();
      alert('Your message has been sent!');
      document.getElementById('contact-form').reset();
    });
  </script>

</body>
</html>
