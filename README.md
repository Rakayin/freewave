freewave-portfolio/
│
├── index.html
├── style.css
└── script.js
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Freewave Band</title>
  <link rel="stylesheet" href="style.css"/>
</head>
<body>

  <header>
    <h1>Freewave</h1>
    <nav>
      <a href="#bio">About</a>
      <a href="#tour">Tour</a>
      <a href="#music">Music</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Feel the Wave of Sound</h2>
    <p>Alternative rock band from the coast.</p>
  </section>

  <section id="bio" class="section">
    <h2>About Us</h2>
    <p>Freewave blends the sounds of surf rock, indie, and experimental tones. Formed in 2019, we're a four-piece group making waves across the globe.</p>
  </section>

  <section id="tour" class="section">
    <h2>Upcoming Tour Dates</h2>
    <ul>
      <li>June 10 - Los Angeles, CA</li>
      <li>June 15 - Austin, TX</li>
      <li>June 22 - New York, NY</li>
    </ul>
  </section>

  <section id="music" class="section">
    <h2>Listen</h2>
    <iframe src="https://open.spotify.com/embed/artist/your_artist_id" width="300" height="80" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  </section>

  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <form id="contact-form">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Freewave. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: #fff;
  color: #333;
}

header {
  background: #0d0d0d;
  color: white;
  padding: 20px;
  text-align: center;
}

nav a {
  margin: 0 10px;
  color: white;
  text-decoration: none;
}

.hero {
  background: url('https://source.unsplash.com/1600x400/?band,concert') no-repeat center;
  background-size: cover;
  color: white;
  text-align: center;
  padding: 100px 20px;
}

.section {
  padding: 60px 20px;
  text-align: center;
}

form {
  max-width: 400px;
  margin: auto;
  display: flex;
  flex-direction: column;
}

form input, form textarea {
  margin: 10px 0;
  padding: 10px;
  font-size: 16px;
}

button {
  background: #333;
  color: white;
  border: none;
  padding: 10px;
  cursor: pointer;
}

footer {
  background: #f1f1f1;
  text-align: center;
  padding: 20px;
}
document.getElementById("contact-form").addEventListener("submit", function(e) {
  e.preventDefault();
  alert("Thanks for reaching out! We'll get back to you soon.");
});

