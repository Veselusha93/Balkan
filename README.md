<!doctype html>
<html lang="bg">
<head>
  <!-- Основни настройки -->
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />

  <!-- SEO -->
  <title>Балкан – Професионално почистване | Варна</title>
  <meta name="description" content="Професионално почистване във Варна. Почистване след ремонт, машинно почистване, пране на мека мебел и абонаментно почистване. Безплатен оглед и гарантирано качество!" />
  <meta name="keywords" content="почистване Варна, професионално почистване, след ремонт, машинно почистване, пране на дивани, Балкан Варна" />
  <meta name="author" content="Балкан Професионално почистване - Варна" />

  <!-- Open Graph -->
  <meta property="og:type" content="website" />
  <meta property="og:title" content="Балкан – Професионално почистване | Варна" />
  <meta property="og:description" content="Почистване след ремонт, машинно почистване на подове, пране на мека мебел. Безплатен оглед в рамките на Варна." />
  <meta property="og:image" content="https://balkan-cleaning.bg/logo.jpg" />
  <meta property="og:url" content="https://balkan-cleaning.bg/" />

  <!-- Twitter -->
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Балкан – Професионално почистване | Варна" />
  <meta name="twitter:description" content="Професионално почистване и пране на мека мебел във Варна. Безплатен оглед!" />
  <meta name="twitter:image" content="https://balkan-cleaning.bg/logo.jpg" />

  <!-- Favicon -->
  <link rel="icon" type="image/png" href="favicon.png" />

  <!-- Стилове -->
  <style>
    :root {
      --primary:#c81010;
      --dark:#222;
      --muted:#666;
      --card:#fff;
      --bg:#f7f7f8;
    }
    *{margin:0; padding:0; box-sizing:border-box;}
    body{
      font-family:Inter, system-ui, "Segoe UI", Roboto, Arial;
      background:var(--bg);
      color:var(--dark);
      line-height:1.6;
    }
    header{
      background:#fff;
      padding:24px 20px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      box-shadow:0 2px 10px rgba(0,0,0,0.05);
      position:sticky;
      top:0;
      z-index:999;
    }
    .logo{display:flex; align-items:center; gap:12px;}
    .logo img{height:60px;}
    nav a{
      margin-left:18px;
      text-decoration:none;
      color:var(--dark);
      font-weight:600;
      transition:.2s;
    }
    nav a:hover{color:var(--primary);}
    .hero{
      padding:60px 20px;
      display:grid;
      grid-template-columns:1fr 400px;
      gap:40px;
      align-items:center;
    }
    .hero h1{font-size:42px; color:var(--primary); margin-bottom:12px;}
    .hero p{color:var(--muted); margin-bottom:18px;}
    .btn{
      display:inline-block;
      background:var(--primary);
      color:#fff;
      padding:12px 20px;
      border-radius:10px;
      text-decoration:none;
      font-weight:700;
      transition:.2s;
    }
    .btn:hover{background:#a70d0d;}
    .btn.alt{background:#fff; color:var(--primary); border:2px solid var(--primary);}
    .services{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(300px, 1fr));
      gap:20px;
      padding:20px;
    }
    .service{
      background:var(--card);
      border-radius:12px;
      padding:18px;
      box-shadow:0 6px 18px rgba(0,0,0,0.06);
      transition:.2s;
    }
    .service:hover{transform:translateY(-3px);}
    .service h3{margin-bottom:6px; color:var(--primary);}
    footer{
      background:#fff;
      padding:18px 20px;
      font-size:14px;
      color:var(--muted);
      display:flex;
      justify-content:space-between;
      flex-wrap:wrap;
      border-top:1px solid #eee;
    }
    footer a{color:var(--primary); text-decoration:none;}
    @media(max-width:900px){
      .hero{grid-template-columns:1fr; text-align:center;}
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">
      <img src="logo.jpg" alt="Балкан Почистване Варна - Лого" />
      <div>
        <strong style="font-size:18px;">Балкан</strong><br>
        <span style="font-size:13px; color:var(--muted)">Професионално почистване | Варна</span>
      </div>
    </div>
    <nav aria-label="Основна навигация">
      <a href="#uslugi">Услуги</a>
      <a href="#besplaten-ogled">Безплатен оглед</a>
      <a href="#kontakt">Контакти</a>
    </nav>
  </header>

  <main>
    <section class="hero">
      <div>
        <h1>Професионално почистване във Варна</h1>
        <p>Почистване след ремонт, машинно почистване на подове и пране на мека мебел. Надеждно обслужване и безплатен оглед на място.</p>
        <a href="#kontakt" class="btn">Заяви почистване</a>
        <a href="#uslugi" class="btn alt">Разгледай услуги</a>
      </div>
      <div class="card" style="background:#fff; padding:18px; border-radius:12px; box-shadow:0 6px 20px rgba(0,0,0,0.05);">
        <h3>Бърза заявка</h3>
        <form id="quickForm">
          <input type="text" name="name" placeholder="Име" required style="width:100%; padding:10px; margin:6px 0; border-radius:8px; border:1px solid #ddd;">
          <input type="tel" name="phone" placeholder="Телефон" required style="width:100%; padding:10px; margin:6px 0; border-radius:8px; border:1px solid #ddd;">
          <select name="service" required style="width:100%; padding:10px; margin:6px 0; border-radius:8px; border:1px solid #ddd;">
            <option value="" disabled selected>Изберете услуга</option>
            <option>Почистване след ремонт</option>
            <option>Машинно почистване на под</option>
            <option>Пране на мека мебел</option>
            <option>Почистване при нанасяне / изнасяне</option>
          </select>
          <button class="btn" type="submit" style="width:100%;">Изпрати</button>
        </form>
      </div>
    </section>

    <section id="uslugi" class="services">
      <div class="service">
        <h3>Почистване след ремонт</h3>
        <p>Цена: 6 лв./кв.м.<br>При силно замърсяване: +50%<br>При много силно замърсяване: +75%</p>
      </div>
      <div class="service">
        <h3>Машинно почистване на под</h3>
        <p>Цена: 3 лв./кв.м.<br>При силно замърсяване: +50%<br>При много силно замърсяване: +75%</p>
      </div>
      <div class="service">
        <h3>Почистване при нанасяне или изнасяне</h3>
        <p>Цена по договаряне.</p>
      </div>
      <div class="service">
        <h3>Почистване на вакантни жилища</h3>
        <p>Цена по договаряне.</p>
      </div>
      <div class="service">
        <h3>Почистване на офиси и бизнес сгради</h3>
        <p>Цена по договаряне.</p>
      </div>
      <div class="service">
        <h3>Пране на мека мебел</h3>
        <p>
          Единичен матрак (едностранно): 20 лв.<br>
          Единичен матрак (двустранно): 40 лв.<br>
          Двоен матрак (едностранно): 40 лв.<br>
          Двоен матрак (двустранно): 70 лв.<br>
          Стол: 15 лв.<br>
          Диван (на седящо място): 12 лв.<br>
          Табуретка: 10 лв.<br>
          Фотьойл: 30 лв.
        </p>
      </div>
    </section>

    <section id="besplaten-ogled" style="padding:20px; text-align:center;">
      <h2>Безплатен оглед</h2>
      <p>Наш екип ще извърши безплатен оглед и ще ви даде точна оферта спрямо състоянието на обекта.</p>
      <a href="tel:+359890522954" class="btn">Обади се за оглед</a>
    </section>
  </main>

  <footer id="kontakt">
    <div>© <span id="year"></span> Балкан – Професионално почистване, Варна</div>
    <div>Тел: <a href="tel:+359890522954">0890 522 954</a> | Имейл: <a href="mailto:officebalkan@mail.bg">officebalkan@mail.bg</a></div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    document.getElementById('quickForm').addEventListener('submit', e => {
      e.preventDefault();
      alert('Благодарим! Вашата заявка е получена. Ще се свържем с вас скоро.');
      e.target.reset();
    });
  </script>
</body>
</html>
