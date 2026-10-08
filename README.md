<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AIConnect - Official Catalog</title>
  <style>
    :root {
      --primary: #d62883;
      --primary-hover: #b01b68;
      --dark-bg: #1f2937;
      --light-bg: #f9fafb;
      --card-bg: #ffffff;
      --text-main: #111827;
      --text-muted: #6b7280;
      --border: #e5e7eb;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: var(--light-bg);
      color: var(--text-main);
    }

    /* Header & Navigation */
    header {
      background: #ffffff;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 1.8rem;
      font-weight: 800;
      color: var(--text-main);
      text-decoration: none;
    }

    .logo span {
      color: var(--primary);
    }

    .nav-links {
      display: flex;
      gap: 1.5rem;
      list-style: none;
      align-items: center;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--text-main);
      font-weight: 600;
      transition: color 0.2s;
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    .btn-join {
      background-color: var(--primary);
      color: white !important;
      padding: 0.6rem 1.2rem;
      border-radius: 25px;
      transition: background-color 0.2s;
    }

    .btn-join:hover {
      background-color: var(--primary-hover);
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(135deg, #fff5f9 0%, #ffffff 100%);
      padding: 3.5rem 2rem;
      text-align: center;
      border-bottom: 1px solid var(--border);
    }

    .hero-content {
      max-width: 800px;
      margin: 0 auto;
    }

    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 0.8rem;
    }

    .hero h1 span {
      color: var(--primary);
    }

    .hero p {
      font-size: 1.1rem;
      color: var(--text-muted);
    }

    /* Filter & Search Bar */
    .controls-container {
      max-width: 1200px;
      margin: 2rem auto 0;
      padding: 0 2rem;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: space-between;
      align-items: center;
    }

    .search-input {
      padding: 0.75rem 1rem;
      border: 1px solid var(--border);
      border-radius: 8px;
      width: 100%;
      max-width: 300px;
      font-size: 0.95rem;
    }

    .filter-buttons {
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
    }

    .filter-btn {
      padding: 0.5rem 1rem;
      border: 1px solid var(--border);
      background: white;
      border-radius: 20px;
      cursor: pointer;
      font-weight: 600;
      font-size: 0.85rem;
      transition: all 0.2s;
    }

    .filter-btn.active, .filter-btn:hover {
      background: var(--primary);
      color: white;
      border-color: var(--primary);
    }

    /* Product Section */
    .products-section {
      max-width: 1200px;
      margin: 2rem auto;
      padding: 0 2rem;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
      gap: 1.5rem;
    }

    .product-card {
      background: var(--card-bg);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 1.5rem;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .product-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.06);
    }

    .product-badge {
      font-size: 0.75rem;
      font-weight: 700;
      color: var(--primary);
      text-transform: uppercase;
      letter-spacing: 0.5px;
      margin-bottom: 0.5rem;
    }

    .product-title {
      font-size: 1.05rem;
      font-weight: 700;
      margin-bottom: 1rem;
      color: var(--text-main);
      line-height: 1.3;
    }

    .product-price {
      font-size: 1.35rem;
      font-weight: 800;
      color: var(--primary);
      margin-bottom: 1.25rem;
    }

    .btn-add {
      background-color: var(--dark-bg);
      color: white;
      border: none;
      padding: 0.75rem;
      width: 100%;
      border-radius: 6px;
      font-weight: 600;
      cursor: pointer;
      transition: background-color 0.2s;
    }

    .btn-add:hover {
      background-color: #000000;
    }

    /* Footer */
    footer {
      background-color: var(--dark-bg);
      color: white;
      text-align: center;
      padding: 2rem;
      margin-top: 4rem;
    }

    footer p {
      color: #9ca3af;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="nav-container">
      <a href="#" class="logo">AI<span>Connect</span></a>
      <ul class="nav-links">
        <li><a href="#shop">Shop</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="https://aiconnect.biz/#shop" class="btn-join" target="_blank">Join AI Connect</a></li>
      </ul>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="about">
    <div class="hero-content">
      <h1>Start Your <span>Dropshipping</span> Business</h1>
      <p>Official catalog with standard regular pricing for all health, wellness, and beauty products.</p>
    </div>
  </section>

  <!-- Filter & Search Controls -->
  <div class="controls-container" id="shop">
    <input type="text" id="searchInput" class="search-input" placeholder="Search products..." onkeyup="filterProducts()">
    <div class="filter-buttons">
      <button class="filter-btn active" onclick="filterCategory('all', this)">All</button>
      <button class="filter-btn" onclick="filterCategory('gummies', this)">Gummies</button>
      <button class="filter-btn" onclick="filterCategory('skincare', this)">Skincare & Soaps</button>
      <button class="filter-btn" onclick="filterCategory('wellness', this)">Wellness</button>
    </div>
  </div>

  <!-- Product Catalog Grid -->
  <section class="products-section">
    <div class="product-grid" id="productGrid">

      <!-- Product Items -->
      <div class="product-card" data-category="gummies">
        <div>
          <div class="product-badge">Gummies</div>
          <h3 class="product-title">Glutathione Collagen Gummies</h3>
        </div>
        <div>
          <div class="product-price">₱1,497.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="gummies">
        <div>
          <div class="product-badge">Gummies</div>
          <h3 class="product-title">Apple Cider Vinegar Gummies</h3>
        </div>
        <div>
          <div class="product-price">₱997.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="gummies">
        <div>
          <div class="product-badge">Gummies</div>
          <h3 class="product-title">Barley Gummies</h3>
        </div>
        <div>
          <div class="product-price">₱997.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="gummies">
        <div>
          <div class="product-badge">Gummies</div>
          <h3 class="product-title">Berberine Gummies</h3>
        </div>
        <div>
          <div class="product-price">₱997.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="wellness">
        <div>
          <div class="product-badge">Wellness</div>
          <h3 class="product-title">Aurum Essentials</h3>
        </div>
        <div>
          <div class="product-price">₱999.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Skincare</div>
          <h3 class="product-title">Saskin Set</h3>
        </div>
        <div>
          <div class="product-price">₱500.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="wellness">
        <div>
          <div class="product-badge">Wellness</div>
          <h3 class="product-title">DeyliHerbs Vitality Herb Mix</h3>
        </div>
        <div>
          <div class="product-price">₱350.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Skincare</div>
          <h3 class="product-title">Wonder Bleach</h3>
        </div>
        <div>
          <div class="product-price">₱350.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Skincare</div>
          <h3 class="product-title">Ultrawhite Sunscreen</h3>
        </div>
        <div>
          <div class="product-price">₱180.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Personal Care</div>
          <h3 class="product-title">Kiffy-Fied</h3>
        </div>
        <div>
          <div class="product-price">₱150.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Personal Care</div>
          <h3 class="product-title">Kili-Kilified</h3>
        </div>
        <div>
          <div class="product-price">₱125.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Soap</div>
          <h3 class="product-title">Niacinamide Soap</h3>
        </div>
        <div>
          <div class="product-price">₱75.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

      <div class="product-card" data-category="skincare">
        <div>
          <div class="product-badge">Soap</div>
          <h3 class="product-title">OG-Kagayaku Soap</h3>
        </div>
        <div>
          <div class="product-price">₱75.00</div>
          <button class="btn-add">Add to Cart</button>
        </div>
      </div>

    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2026 AIConnect Official Distributor Catalog.</p>
  </footer>

  <!-- Filter & Search Script -->
  <script>
    let currentCategory = 'all';

    function filterCategory(category, btnElement) {
      currentCategory = category;
      
      // Update active button state
      document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
      btnElement.classList.add('active');

      filterProducts();
    }

    function filterProducts() {
      const searchQuery = document.getElementById('searchInput').value.toLowerCase();
      const cards = document.querySelectorAll('.product-card');

      cards.forEach(card => {
        const title = card.querySelector('.product-title').textContent.toLowerCase();
        const category = card.getAttribute('data-category');

        const matchesSearch = title.includes(searchQuery);
        const matchesCategory = (currentCategory === 'all' || category === currentCategory);

        if (matchesSearch && matchesCategory) {
          card.style.display = 'flex';
        } else {
          card.style.display = 'none';
        }
      });
    }
  </script>

</body>
</html>
