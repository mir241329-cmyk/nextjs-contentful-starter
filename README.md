!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fabulous Stationery</title>
  <style>
    /* Google Fonts */
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

    /* Reset + Base */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #f8f9fa, #e0f7fa);
      color: #333;
      overflow-x: hidden;
    }

    /* Header */
    header {
      background: linear-gradient(90deg, #4CAF50, #2E7D32);
      color: white;
      padding: 40px 20px;
      text-align: center;
      animation: fadeInDown 1.5s ease;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    }
    header h1 {
      font-size: 3rem;
      letter-spacing: 2px;
    }
    header p {
      margin-top: 10px;
      font-size: 1.2rem;
    }

    /* Navigation */
    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      background: #333;
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      transition: 0.3s;
    }
    nav a:hover {
      color: #4CAF50;
      transform: scale(1.1);
    }

    /* Section Styling */
    section {
      padding: 50px 10%;
      animation: fadeInUp 1.5s ease;
    }
    section h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 30px;
      color: #2E7D32;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
    }

    /* Product Grid */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
    }
    .card {
      background: white;
      border-radius: 15px;
      padding: 20px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      cursor: pointer;
      position: relative;
      overflow: hidden;
    }
    .card::before {
      content: "";
      position: absolute;
      top: -100%;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(120deg, rgba(76,175,80,0.2), rgba(255,255,255,0.1));
      transition: top 0.5s;
    }
    .card:hover::before {
      top: 0;
    }
    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 6px 30px rgba(0,0,0,0.2);
    }
    .card h3 {
      font-size: 1.5rem;
      color: #4CAF50;
      margin-bottom: 10px;
    }
    .card p {
      font-size: 0.95rem;
      line-height: 1.5;
    }
    .price {
      margin-top: 15px;
      font-size: 1.2rem;
      font-weight: bold;
      color: #E91E63;
    }

    /* Footer */
    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 30px;
      font-size: 0.9rem;
    }

    /* Animations */
    @keyframes fadeInUp {
      from { transform: translateY(40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
    @keyframes fadeInDown {
      from { transform: translateY(-40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Fabulous Stationery</h1>
    <p>Your Professional Hub for Books, Toys, Stationery & Fancy Items</p>
  </header>

  <nav>
    <a href="#books">Books</a>
    <a href="#toys">Toys</a>
    <a href="#stationery">Stationery</a>
    <a href="#fancy">Fancy Items</a>
  </nav>

  <!-- Books Section -->
  <section id="books">
    <h2>Books Collection</h2>
    <div class="grid">
      <div class="card">
        <h3>Classic Notebook</h3>
        <p>Durable notebooks with smooth pages. Ideal for students & professionals.</p>
        <p class="price">₹120</p>
      </div>
      <div class="card">
        <h3>Story Book</h3>
        <p>Imaginative tales for children that inspire creativity and moral lessons.</p>
        <p class="price">₹200</p>
      </div>
      <div class="card">
        <h3>Educational Workbook</h3>
        <p>Skill-building practice books for mathematics, science, and language learning.</p>
        <p class="price">₹180</p>
      </div>
      <div class="card">
        <h3>Exam Preparation Guide</h3>
        <p>Comprehensive material for competitive exam success.</p>
        <p class="price">₹350</p>
      </div>
    </div>
  </section>

  <!-- Toys Section -->
  <section id="toys">
    <h2>Toys Collection</h2>
    <div class="grid">
      <div class="card">
        <h3>Coloring Kit</h3>
        <p>Boosts imagination and creativity in kids with safe, vibrant colors.</p>
        <p class="price">₹350</p>
      </div>
      <div class="card">
        <h3>Puzzle Game</h3>
        <p>Sharpens analytical thinking and improves concentration.</p>
        <p class="price">₹499</p>
      </div>
      <div class="card">
        <h3>Building Blocks</h3>
        <p>Enhances motor skills and encourages problem-solving in young minds.</p>
        <p class="price">₹600</p>
      </div>
      <div class="card">
        <h3>Soft Toys</h3>
        <p>Cuddly companions that provide comfort and joy to children.</p>
        <p class="price">₹450</p>
      </div>
    </div>
  </section>

  <!-- Stationery Section -->
  <section id="stationery">
    <h2>Stationery Items</h2>
    <div class="grid">
      <div class="card">
        <h3>Pen Set</h3>
        <p>Stylish pens for smooth and elegant writing experience.</p>
        <p class="price">₹150</p>
      </div>
      <div class="card">
        <h3>Color Pencils</h3>
        <p>Premium colors to bring your artwork to life.</p>
        <p class="price">₹250</p>
      </div>
      <div class="card">
        <h3>Highlighters</h3>
        <p>Bright markers to organize and emphasize your notes.</p>
        <p class="price">₹180</p>
      </div>
      <div class="card">
        <h3>Sticky Notes</h3>
        <p>Perfect for reminders, planning, and quick jotting.</p>
        <p class="price">₹90</p>
      </div>
    </div>
  </section>

  <!-- Fancy Items Section -->
  <section id="fancy">
    <h2>Fancy Items</h2>
    <div class="grid">
      <div class="card">
        <h3>Designer Diary</h3>
        <p>Stylish diaries to record your thoughts, goals, and memories.</p>
        <p class="price">₹300</p>
      </div>
      <div class="card">
        <h3>Gift Items</h3>
        <p>Beautifully crafted gift items for every occasion.</p>
        <p class="price">₹450</p>
      </div>
      <div class="card">
        <h3>Decorative Lights</h3>
        <p>Enhance your room with vibrant and charming lighting effects.</p>
        <p class="price">₹700</p>
      </div>
      <div class="card">
        <h3>Fancy Pen Holder</h3>
        <p>Elegant desk accessory to keep your stationery organized.</p>
        <p class="price">₹250</p>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Fabulous Stationery | Crafted with Excellence</p>
  </footer>
</body>
</html>
