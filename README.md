<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>UFC 344</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }

    body {
      background: #111;
      color: #fff;
      padding: 10px;
    }

    /* HEADER */
    header {
      background: #1a1a1a;
      border-bottom: 2px solid #e60000;
      padding: 15px;
    }

    .header-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 22px;
      font-weight: 700;
      color: #e60000;
    }

    .header-btn {
      background: #e60000;
      color: #fff;
      text-decoration: none;
      padding: 6px 14px;
      border-radius: 20px;
      font-size: 14px;
      font-weight: 600;
    }

    /* EVENT */
    .event-header {
      text-align: center;
      margin: 20px 0;
    }

    .event-header h1 {
      font-size: 20px;
      margin-bottom: 4px;
    }

    .event-header p {
      font-size: 14px;
      color: #ccc;
    }

    /* FIGHT CARD */
    .fight-card {
      background: #1a1a1a;
      border: 2px solid #e60000;
      border-radius: 12px;
      padding: 15px;
      margin-bottom: 18px;
      display: flex;
      align-items: center;
      gap: 14px;
    }

    .fighter {
      display: flex;
      flex-direction: column;
      align-items: center;
      min-width: 90px;
      text-align: center;
    }

    .photo {
      width: 90px;
      height: 90px;
      border-radius: 50%;
      overflow: hidden;
      border: 3px solid #e60000;
      margin-bottom: 6px;
    }

    .photo.win {
      border-color: #34d665;
    }

    .photo img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .name {
      font-size: 15px;
      font-weight: 600;
    }

    .vs {
      font-size: 22px;
      font-weight: 700;
      color: #e60000;
    }

    .fight-info {
      flex: 1;
      text-align: right;
    }

    .weight {
      font-size: 13px;
      color: #ccc;
      margin-bottom: 6px;
    }

    .result {
      font-size: 14px;
      font-weight: 600;
    }

    .result.win {
      color: #34d665;
    }

    .result.cancel {
      color: red;
    }

    footer {
      text-align: center;
      padding: 15px;
      background: #1a1a1a;
      border-top: 2px solid #e60000;
      color: #ccc;
      font-size: 12px;
      margin-top: 20px;
    }

    @media (max-width: 480px) {
      .photo {
        width: 75px;
        height: 75px;
      }

      .fight-card {
        gap: 10px;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="header-inner">
    <div class="logo">UFC 344</div>
    <a class="header-btn" href="https://AlishkaNepo.github.io/ufc-343/" target="_blank">UFC 343</a>
  </div>
</header>

<div class="event-header">
  <h1>Главный кард — 6 Января</h1>
  <p>Место проведения: Рим, Италия</p>
</div>

<!-- БОЙ 1 -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo win"><img src="tomi.jpg"></div>
    <div class="name">Танат</div>
  </div>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo"><img src="ali.jpg"></div>
    <div class="name">Али</div>
  </div>

  <div class="fight-info">
    <div class="weight">Лёгкий вес • Главный бой</div>
    <div class="result win">Судейское решение • Р5 05:00</div>
  </div>
</div>

<!-- БОЙ 2 -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo win"><img src="beka2.jpg"></div>
    <div class="name">Бексултан</div>
  </div>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo"><img src="ibr.jpg"></div>
    <div class="name">Ибрахим</div>
  </div>

  <div class="fight-info">
    <div class="weight">Полусредний вес • Со-главный бой</div>
    <div class="result win">Добровольная сдача • Р1 04:45</div>
  </div>
</div>

<!-- БОЙ 3 -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo"><img src="jahan.jpg"></div>
    <div class="name">Жахан</div>
  </div>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo win"><img src="abosh.jpg"></div>
    <div class="name">Абылайхан</div>
  </div>

  <div class="fight-info">
    <div class="weight">Лёгкий вес</div>
    <div class="result win">Судейское решение • Р3 05:00</div>
  </div>
</div>

<!-- БОЙ 4 -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo"><img src="beka2.jpg"></div>
    <div class="name">Бексултан</div>
  </div>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo"><img src="era.jpg"></div>
    <div class="name">Ерасыл</div>
  </div>

  <div class="fight-info">
    <div class="weight">Полусредний вес • Со-главный бой</div>
    <div class="result cancel">Отменён</div>
  </div>
</div>

<!-- БОЙ 5 -->
<div class="fight-card">
  <div class="fighter">
    <div class="photo"><img src="jahan.jpg"></div>
    <div class="name">Жахан</div>
  </div>

  <div class="vs">VS</div>

  <div class="fighter">
    <div class="photo"><img src="ibr.jpg"></div>
    <div class="name">Ибрахим</div>
  </div>

  <div class="fight-info">
    <div class="weight">Полусредний вес</div>
    <div class="result cancel">Отменён</div>
  </div>
</div>

<footer>
  © 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
