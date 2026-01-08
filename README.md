<!DOCTYPE html>
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
  background: #0e0e0e;
  color: #fff;
  padding: 16px;
  overflow-x: auto; /* 🔥 если экран узкий — скролл, но одна строка */
}

/* ===== HEADER ===== */
header {
  background: #111;
  border-bottom: 2px solid #e60000;
  padding: 14px;
  margin-bottom: 24px;
}

header h1 {
  color: #e60000;
  text-align: center;
  font-size: 20px;
}

/* ===== TITLE ===== */
.event-info {
  text-align: center;
  margin-bottom: 28px;
}

.event-info .title {
  font-weight: 600;
}

.event-info .place {
  font-size: 13px;
  color: #aaa;
  margin-top: 4px;
}

/* ===== FIGHT CARD ===== */
.fight-card {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: nowrap;              /* 🔥 ОДНА СТРОКА */
  gap: 20px;
  background: #141414;
  border: 2px solid #e60000;
  border-radius: 14px;
  padding: 16px;
  margin-bottom: 22px;
  min-width: 520px;               /* 🔥 защита от ломания */
}

/* ===== FIGHTERS ===== */
.fighters {
  display: flex;
  align-items: center;
  gap: 12px;
  flex-wrap: nowrap;
  white-space: nowrap;
}

.fighter {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 13px;
}

.photo {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  border: 3px solid #e60000;
  overflow: hidden;
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

.vs {
  font-size: 18px;
  font-weight: 700;
  color: #e60000;
}

/* ===== INFO ===== */
.fight-info {
  text-align: right;
  white-space: nowrap;
}

.weight {
  font-size: 13px;
  color: #ccc;
}

.result {
  margin-top: 6px;
  font-size: 13px;
}

.win-text {
  color: #34d665;
}

.cancel {
  color: #e60000;
  font-weight: 600;
}

/* ===== MOBILE — ТОЛЬКО УМЕНЬШЕНИЕ ===== */
@media (max-width: 600px) {

  header h1 {
    font-size: 18px;
  }

  .fight-card {
    padding: 10px;
    gap: 14px;
  }

  .photo {
    width: 55px;
    height: 55px;
  }

  .fighter {
    font-size: 11px;
  }

  .vs {
    font-size: 14px;
  }

  .weight,
  .result {
    font-size: 11px;
  }
}

/* ===== FOOTER ===== */
footer {
  text-align: center;
  color: #666;
  font-size: 12px;
  margin-top: 40px;
}
</style>
</head>

<body>

<header>
  <h1>UFC 344</h1>
</header>

<div class="event-info">
  <div class="title">Главный кард — 6 января</div>
  <div class="place">Место проведения: Рим, Италия</div>
</div>

<!-- 1 -->
<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <div class="photo win"><img src="tomi.jpg"></div>
      <span>Танат</span>
    </div>
    <span class="vs">VS</span>
    <div class="fighter">
      <div class="photo"><img src="ali.jpg"></div>
      <span>Али</span>
    </div>
  </div>
  <div class="fight-info">
    <div class="weight">Лёгкий вес • Главный бой</div>
    <div class="result win-text">Судейское решение • Р5 05:00</div>
  </div>
</div>

<!-- 2 -->
<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <div class="photo win"><img src="beka2.jpg"></div>
      <span>Бексултан</span>
    </div>
    <span class="vs">VS</span>
    <div class="fighter">
      <div class="photo"><img src="ibr.jpg"></div>
      <span>Ибрахим</span>
    </div>
  </div>
  <div class="fight-info">
    <div class="weight">Полусредний вес • Со-главный бой</div>
    <div class="result win-text">Добровольная сдача • Р1 04:45</div>
  </div>
</div>

<!-- 3 -->
<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <div class="photo"><img src="jahan.jpg"></div>
      <span>Жахан</span>
    </div>
    <span class="vs">VS</span>
    <div class="fighter">
      <div class="photo win"><img src="abosh.jpg"></div>
      <span>Абылайхан</span>
    </div>
  </div>
  <div class="fight-info">
    <div class="weight">Лёгкий вес</div>
    <div class="result win-text">Судейское решение • Р3 05:00</div>
  </div>
</div>

<!-- 4 -->
<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <div class="photo"><img src="beka2.jpg"></div>
      <span>Бексултан</span>
    </div>
    <span class="vs">VS</span>
    <div class="fighter">
      <div class="photo"><img src="era.jpg"></div>
      <span>Ерасыл</span>
    </div>
  </div>
  <div class="fight-info">
    <div class="weight">Полусредний вес</div>
    <div class="result cancel">Отменен</div>
  </div>
</div>

<div class="fight-card">
  <div class="fighters">
    <div class="fighter">
      <div class="photo"><img src="jahan.jpg"></div>
      <span>Жахан</span>
    </div>
    <span class="vs">VS</span>
    <div class="fighter">
      <div class="photo"><img src="ibr.jpg"></div>
      <span>Ибрахим</span>
    </div>
  </div>
  <div class="fight-info">
    <div class="weight">Полусредний вес</div>
    <div class="result cancel">Отменен</div>
  </div>
</div>

<footer>
  © 2025 My Fight Promotion. Все права защищены.
</footer>

</body>
</html>
