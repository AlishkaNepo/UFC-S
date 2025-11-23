<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>UFC 344 - Мобильная версия</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* --- Общие стили --- */
    * { margin:0; padding:0; box-sizing:border-box; font-family:'Inter', sans-serif; }
    body { background-color:#111; color:#fff; line-height:1.5; padding:10px; }

    /* --- Хедер --- */
    header { text-align:center; padding:15px; background-color:#1a1a1a; border-bottom:2px solid #e60000; }
    header .logo { font-size:22px; font-weight:700; color:#e60000; }

    /* --- Заголовок события --- */
    .event-header { margin:20px 0; text-align:center; }
    .event-header h1 { font-size:20px; margin-bottom:5px; }
    .event-header p { font-size:14px; color:#ccc; }

    /* --- Карточка боя --- */
    .fight-card { background-color:#1a1a1a; border:2px solid #e60000; border-radius:12px; padding:15px; margin-bottom:20px; }
    .fighters { display:flex; flex-direction:column; align-items:center; gap:10px; }
    .fighter { display:flex; flex-direction:column; align-items:center; text-align:center; }
    .fighter img { width:100px; height:100px; object-fit:cover; border-radius:50%; border:3px solid #e60000; margin-bottom:5px; }
    .name { font-weight:600; font-size:16px; }
    .vs { font-size:24px; font-weight:700; color:#e60000; margin:10px 0; }
    .weight { font-size:14px; color:#ccc; text-align:center; margin-top:5px; }

    /* --- Футер --- */
    footer { text-align:center; padding:15px; background-color:#1a1a1a; border-top:2px solid #e60000; color:#ccc; font-size:12px; }

    /* --- Адаптивные улучшения --- */
    @media screen and (min-width:500px) {
      .fighters { flex-direction:row; justify-content:space-around; }
      .fighter img { width:120px; height:120px; }
      .name { font-size:18px; }
      .vs { font-size:28px; }
      .weight { font-size:16px; }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">UFC 344</div>
</header>

<div class="event-header">
  <h1>Главный кард — 5 Января</h1>
  <p>Место проведения: Рим, Италия</p>
</div>

<!-- Первый бой -->
<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <img src="tomi.jpg" alt="Танат" title="Баккали Танат, действующий чемпион легкого веса">
      <div class="name">Танат</div>
    </div>
    <div class="vs">VS</div>
    <div class="fighter">
      <img src="ali.jpg" alt="Али" title="Дуйсен Али, действующий чемпион полулегкого веса">
      <div class="name">Али</div>
    </div>
  </div>
  <div class="weight">Лёгкий вес • Главный бой</div>
</div>

<!-- Второй бой -->
<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <img src="beka.jpg" alt="Бексултан" title="Бейсембай Бексултан, претендент на звание чемпиона в полусреднем весе">
      <div class="name">Бексултан</div>
    </div>
    <div class="vs">VS</div>
    <div class="fighter">
      <img src="era.jpg" alt="Ерасыл" title="Жумабай Ерасыл, претендент на звание чемпиона в полусреднем весе">
      <div class="name">Ерасыл</div>
    </div>
  </div>
  <div class="weight">Полусредний вес • Главный бой</div>
</div>

<footer>
  © 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
