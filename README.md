<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Bogardus Bread</title>

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: Georgia, serif;
      background: #f8f1e7;
      color: #2f2018;
    }

    a { text-decoration: none; color: inherit; }

    header {
      min-height: 100vh;
      background:
        linear-gradient(rgba(30,20,15,.45), rgba(30,20,15,.55)),
        url("https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=1600&q=80");
      background-size: cover;
      background-position: center;
      color: white;
      display: flex;
      flex-direction: column;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 28px 7%;
      letter-spacing: 2px;
      text-transform: uppercase;
      font-size: .8rem;
    }

    .logo { font-size: 1.2rem; }

    nav a { margin-left: 28px; }

    .hero {
      flex: 1;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 7%;
    }

    .hero h1 {
      font-size: clamp(4rem, 10vw, 9rem);
      line-height: .85;
      letter-spacing: 4px;
      margin-bottom: 24px;
    }

    .hero p {
      font-style: italic;
      font-size: 1.5rem;
      margin-bottom: 34px;
    }

    .btn {
      display: inline-block;
      background: #8a5a32;
      color: white;
      padding: 15px 34px;
      border-radius: 0;
      text-transform: uppercase;
      letter-spacing: 2px;
      font: bold .75rem Arial, sans-serif;
    }

    section {
      padding: 90px 8%;
    }

    .split {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
      align-items: center;
    }

    h2 {
      font-size: clamp(2.4rem, 5vw, 4.5rem);
      line-height: 1;
      margin-bottom: 24px;
      font-weight: normal;
    }

    .eyebrow {
      text-transform: uppercase;
      letter-spacing: 3px;
      font: bold .75rem Arial, sans-serif;
      color: #8a5a32;
      margin-bottom: 18px;
    }

    p {
      font-size: 1.05rem;
      line-height: 1.8;
      max-width: 620px;
    }

    .sage {
      background: #d8dfc8;
    }

    .card-note {
      background: #fffaf1;
      padding: 42px;
      border: 1px solid #c8a77d;
      box-shadow: 0 20px 40px rgba(47,32,24,.12);
      transform: rotate(-1.5deg);
    }

    .menu {
      text-align: center;
    }

    .menu-grid {
      margin-top: 44px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
      gap: 28px;
    }

    .item {
      background: #fffaf1;
      padding: 20px;
      border: 1px solid #dfc9a9;
      transition: .25s;
    }

    .item:hover {
      transform: translateY(-8px);
    }

    .item img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      margin-bottom: 20px;
    }

    .item h3 {
      text-transform: uppercase;
      letter-spacing: 2px;
      font-size: 1rem;
      margin-bottom: 10px;
    }

    .price {
      margin-top: 14px;
      color: #8a5a32;
      font-weight: bold;
    }

    .august {
      background:
        linear-gradient(135deg, #f7e4b5, #c78950, #7b4a2b);
      color: white;
      text-align: center;
    }

    .august h2 {
      max-width: 850px;
      margin: 0 auto 24px;
    }

    .bread-club {
      background: #2f2018;
      color: #f8f1e7;
      text-align: center;
    }

    input {
      padding: 16px;
      width: min(400px, 90%);
      border: 1px solid #d6b98c;
      background: transparent;
      color: white;
      margin-top: 28px;
    }

    footer {
      padding: 45px 8%;
      background: #1f1510;
      color: #f8f1e7;
      display: flex;
      justify-content: space-between;
      gap: 24px;
      flex-wrap: wrap;
      font-size: .85rem;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    .tiny {
      font-size: .8rem;
      opacity: .75;
      margin-top: 18px;
    }

    .cone {
      font-size: 1.4rem;
      margin-top: 18px;
    }

    @media (max-width: 800px) {
      .split { grid-template-columns: 1fr; }
      nav { flex-direction: column; gap: 18px; }
      nav a { margin: 0 10px; }
      section { padding: 65px 7%; }
    }
  </style>
</head>

<body>

<header>
  <nav>
    <div class="logo">Bogardus Bread</div>
    <div>
      <a href="#story">Story</a>
      <a href="#menu">Menu</a>
      <a href="#club">Bread Club</a>
      <a href="mailto:hello@bogardusbread.com">Order</a>
    </div>
  </nav>

  <div class="hero">
    <div>
      <h1>Bogardus<br>Bread</h1>
      <p>Bread Worth Gathering For</p>
      <a class="btn" href="#menu">See This Week's Loaves</a>
    </div>
  </div>
</header>

<section id="story" class="split">
  <div>
    <div class="eyebrow">From Emma's Kitchen</div>
    <h2>Slow bread for complicated days.</h2>
    <p>
      Bogardus Bread began with one simple idea: bread should feel warm,
      honest, and worth sharing. Every loaf is made in small batches with
      simple ingredients, slow fermentation, and care you can taste.
    </p>
  </div>

  <div class="card-note">
    <div class="eyebrow">Kitchen Note</div>
    <p>
      Sometimes life is complicated. Fresh bread helps.
    </p>
    <p class="tiny">
      A little reminder from the Bogardus kitchen.
    </p>
    <div class="cone">△ ✦ ♡</div>
  </div>
</section>

<section class="sage split">
  <div>
    <img
      src="https://images.unsplash.com/photo-1598373182133-52452f7691ef?auto=format&fit=crop&w=900&q=80"
      alt="Fresh bread"
      style="width:100%; border-radius: 160px 160px 0 0;"
    />
  </div>

  <div>
    <div class="eyebrow">The Vibe</div>
    <h2>Warm, golden, and made to bring people in.</h2>
    <p>
      Think morning light, flour on the counter, glass cookie jars,
      sage green details, wooden shelves, and loaves that make everyone
      gather around the table.
    </p>
  </div>
</section>

<section id="menu" class="menu">
  <div class="eyebrow">This Week's Menu</div>
  <h2>Fresh From the Oven</h2>

  <div class="menu-grid">
    <div class="item">
      <img src="https://images.unsplash.com/photo-1586444248902-2f64eddc13df?auto=format&fit=crop&w=900&q=80" alt="Classic sourdough">
      <h3>Classic Sourdough</h3>
      <p>Crisp crust, soft inside, naturally fermented.</p>
      <div class="price">$10</div>
    </div>

    <div class="item">
      <img src="https://images.unsplash.com/photo-1608198093002-ad4e005484ec?auto=format&fit=crop&w=900&q=80" alt="Honey oat bread">
      <h3>Honey Oat</h3>
      <p>A cozy loaf with honey, oats, and a soft crumb.</p>
      <div class="price">$11</div>
    </div>

    <div class="item">
      <img src="https://images.unsplash.com/photo-1566698629409-787a68fc5724?auto=format&fit=crop&w=900&q=80" alt="Cinnamon bread">
      <h3>Cinnamon Swirl</h3>
      <p>Sweet, warm, and made for buttered toast.</p>
      <div class="price">$12</div>
    </div>
  </div>
</section>

<section class="august">
  <div class="eyebrow" style="color:white;">August Batch</div>
  <h2>Golden dough, warm flour, and late-summer light.</h2>
  <p style="margin: 0 auto;">
    A soft ombré moment for the bakers, the dreamers, and everyone who
    believes fresh bread can fix at least a little bit of the day.
  </p>
</section>

<section id="club" class="bread-club">
  <div class="eyebrow" style="color:#d6b98c;">Join</div>
  <h2>The Bread Club</h2>
  <p style="margin:0 auto;">
    Weekly menus, loaf drops, kitchen notes, and tiny bakery updates.
  </p>

  <form>
    <input type="email" placeholder="your email" />
    <br><br>
    <button class="btn" type="submit">Join the Club</button>
  </form>

  <p class="tiny">Coneheads welcome. Quietly. ♡</p>
</section>

<footer>
  <div>Bogardus Bread</div>
  <div>© 2026 · Bread Worth Gathering For</div>
  <div>△ ✦ ♡</div>
</footer>

</body>
</html>
