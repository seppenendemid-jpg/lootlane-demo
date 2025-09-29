<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Демо сайт кейсов</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <div class="page">
    <!-- left sidebar -->
    <aside class="sidebar">
      <div class="site-name">Название сайта</div>
      <nav class="menu">
        <a href="#">Игры</a>
        <a href="#">Кейсы</a>
        <a href="#">Шарики</a>
        <a href="#">Апгрейды</a>
        <a href="#">Казино</a>
      </nav>
    </aside>

    <!-- main content -->
    <main class="main">
      <!-- top running skins bar -->
      <div class="topbar">
        <div class="ticker" aria-hidden="true">
          <div class="ticker-track" id="tickerTrack">
            <!-- skin items (insert images or placeholders) -->
            <div class="skin">AWP | Asiimov</div>
            <div class="skin">AK-47 | Redline</div>
            <div class="skin">M4A1 | Hot Rod</div>
            <div class="skin">Desert Eagle | Blaze</div>
            <div class="skin">Knife | Doppler</div>
            <div class="skin">AWP | Asiimov</div>
            <div class="skin">AK-47 | Redline</div>
          </div>
        </div>
      </div>

      <!-- central content area -->
      <section class="center">
        <div class="hero-row">
          <div class="welcome-box">
            <div class="welcome-text">
              <h2>Добро пожаловать<br>на наш сайт</h2>
            </div>
            <button id="loginBtn" class="btn steam">Войти через Steam (демо)</button>
          </div>

          <div class="promo-box">
            <div class="promo-text">
              <h2>Забери 3 кейса<br>бесплатно</h2>
            </div>
            <button id="claimBtn" class="btn">Забрать</button>
          </div>
        </div>

        <div class="tiles">
          <div class="tile">Рулетка</div>
          <div class="tile">Апгрейд</div>
          <div class="tile">Казино</div>
          <div class="tile">Шарики</div>
          <div class="tile">Кейсы</div>
        </div>

        <div class="status-row">
          <div class="last-wins">Последние выигрыши: <span id="lastWins">—</span></div>
          <div class="balance">Баланс кейсов: <span id="balance">0</span></div>
        </div>
      </section>

      <!-- right chat bar -->
      <aside class="chatbar">
        <div class="chat-vertical">chat</div>
        <div class="chat-window" id="chatWindow">
          <!-- messages -->
        </div>
      </aside>
    </main>
  </div>

  <!-- modal for demo steam login -->
  <div id="modal" class="modal hidden" role="dialog" aria-modal="true">
    <div class="modal-content">
      <button class="close" id="modalClose">&times;</button>
      <h3>Войти через Steam (демо)</h3>
      <p class="modal-note">Это демонстрационный вход. <strong>Не вводите реальные пароли Steam.</strong></p>
      <label>
        Ник:
        <input id="demoNick" type="text" placeholder="Введите ник" />
      </label>
      <button id="doLogin" class="btn steam">Войти</button>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
