# UFC-
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>UFC 344</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* --- Общие стили --- */
    * { margin:0; padding:0; box-sizing:border-box; font-family:'Inter', sans-serif; }
    body { background-color:#111; color:#fff; line-height:1.5; }

    /* --- Хедер --- */
    header { display:flex; justify-content:center; align-items:center; padding:20px; background-color:#1a1a1a; border-bottom:2px solid #e60000; }
    header .logo { font-size:24px; font-weight:700; color:#e60000; }

    /* --- Контейнер --- */
    .container, .container2 { max-width:1200px; margin:0 auto; padding:20px; }

    /* --- Заголовок события --- */
    .event-header h1 { font-size:28px; margin-bottom:10px; text-align:center; }
    .event-header p { font-size:16px; text-align:center; color:#ccc; margin-bottom:30px; }

    /* --- Карточка боя --- */
    .fight-card, .fight-card2 { background-color:#1a1a1a; border:2px solid #e60000; border-radius:15px; padding:20px; margin-bottom:30px; }
    .fighters, .fighters2 { display:flex; justify-content:space-around; align-items:center; flex-wrap:wrap; gap:20px; }
    .fighter, .fighter2 { display:flex; flex-direction:column; align-items:center; text-align:center; }
    .fighter img, .fighter2 img { width:150px; height:150px; object-fit:cover; border-radius:50%; border:3px solid #e60000; transition:transform 0.3s; }
    .fighter img:hover, .fighter2 img:hover { transform:scale(1.05); }
    .name, .name2 { margin-top:10px; font-weight:600; font-size:18px; }
    .vs, .vs2 { font-size:28px; font-weight:700; color:#e60000; margin:0 20px; }
    .weight, .weight2 { margin-top:15px; font-size:16px; color:#ccc; text-align:center; font-weight:500; }

    /* --- Футер --- */
    footer { text-align:center; padding:20px; background-color:#1a1a1a; border-top:2px solid #e60000; color:#ccc; }

    /* --- Адаптивность --- */
    @media screen and (max-width:768px){
      .fighters, .fighters2 { flex-direction:column; }
      .vs, .vs2 { margin:10px 0; }
      .fighter img, .fighter2 img { width:120px; height:120px; }
      .name, .name2 { font-size:16px; }
      .weight, .weight2 { font-size:14px; }
      .event-header h1 { font-size:22px; }
      .event-header p { font-size:14px; }
    }
    @media screen and (max-width:480px){
      .fighter img, .fighter2 img { width:100px; height:100px; }
      .vs, .vs2 { font-size:22px; }
      .name, .name2 { font-size:14px; }
      .weight, .weight2 { font-size:12px; }
      .event-header h1 { font-size:20px; }
      .event-header p { font-size:12px; }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">UFC 344</div>
</header>

<div class="container">
  <div class="event-header">
    <h1>Главный кард — 5 Января</h1>
    <p>Место проведения: Рим, Италия</p>
  </div>

  <div class="fights" id="fightsContainer">
    <div class="fight-card">
      <div class="fighters">
        <div class="fighter">
          <img src="tomi.jpg" alt="Боец 1" id="tomi" title="Баккали Танат, действующий чемпион легкого веса">
          <div class="name">Танат</div>
        </div>

        <div class="vs">VS</div>

        <div class="fighter">
          <img src="ali.jpg" alt="Боец 2" id="ali" title="Дуйсен Али, действующий чемпион полулегкого веса">
          <div class="name">Али</div>
        </div>
      </div>
      <div class="weight">Лёгкий вес • Главный бой</div>
    </div>
  </div>
</div>

<div class="container2">
  <div class="fights2" id="fightsContainer2">
    <div class="fight-card2">
      <div class="fighters2">
        <div class="fighter2">
          <img src="beka.jpg" alt="Боец 3" id="beka" title="Бейсембай Бексултан, претендент на звание чемпиона в полусреднем весе">
          <div class="name2">Бексултан</div>
        </div>

        <div class="vs2">VS</div>

        <div class="fighter2">
          <img src="era.jpg" alt="Боец 4" id="era" title="Жумабай Ерасыл, претендент на звание чемпиона в полусреднем весе">
          <div class="name2">Ерасыл</div>
        </div>
      </div>
      <div class="weight2">Полусредний вес • Главный бой</div>
    </div>
  </div>
</div>

<footer>
  © 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
