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

    .event-header {
      text-align: center;
      margin: 20px 0;
    }

    .event-header h1 {
      font-size: 20px;
    }

    .event-header p {
      font-size: 14px;
      color: #ccc;
    }

    /* FIGHT CARD */
    .fight-card {
      position: relative;
      background: #1a1a1a;
      padding: 16px 16px 16px 20px;
      margin-bottom: 18px;
      display: flex;
      align-items: center;
      gap: 14px;
      width: 100%;
    }

    /* VERTICAL LINE */
    .fight-card::before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      bottom: 0;
      width: 4px;
      background: #e60000;
      border-radius: 2px;
    }

    .fight-card.win::before {
      background: #34d665;
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
