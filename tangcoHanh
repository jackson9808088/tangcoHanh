<!DOCTYPE html>
<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cô Hạnh yêu dấu</title>
    <meta
      name="description"
      content="Một trang tri ân Ngày Nhà giáo Việt Nam 20/11, nơi những kỷ niệm, lời chúc và cảm hứng được thắp sáng."
    />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Be+Vietnam+Pro:wght@300;400;600&display=swap"
      rel="stylesheet"
    />
    <style>
      *,
      *::before,
      *::after {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
      }

      html {
        scroll-behavior: smooth;
      }

      :root {
        --bg: radial-gradient(circle at 20% 20%, #ffc7a1 0, rgba(255, 199, 161, 0) 45%),
          radial-gradient(circle at 80% 15%, #ffd6ec 0, rgba(255, 214, 236, 0) 52%),
          radial-gradient(circle at 60% 80%, #dde7ff 0, rgba(221, 231, 255, 0) 50%),
          #f0f3ff;
        --card: rgba(255, 255, 255, 0.78);
        --glass: rgba(255, 255, 255, 0.55);
        --accent: #e4628bff;
        --accent-soft: rgba(233, 95, 139, 0.17);
        --text: #2c2a4a;
        --text-soft: rgba(44, 42, 74, 0.75);
        --shadow: 0 30px 70px rgba(46, 32, 86, 0.18);
        --radius-xl: 32px;
        --radius-lg: 24px;
        --radius-md: 18px;
        --blur: blur(18px);
        --sparkle: rgba(255, 255, 255, 0.55);
        font-size: 16px;
      }

      body {
        min-height: 100vh;
        font-family: "Be Vietnam Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
        background: var(--bg);
        color: var(--text);
        display: grid;
        place-items: center;
        padding: clamp(1.5rem, 5vw, 3rem);
      }

      .stage {
        position: relative;
        width: min(1100px, 100%);
        border-radius: var(--radius-xl);
        padding: clamp(2.5rem, 6vw, 4rem);
        background: rgba(255, 255, 255, 0.68);
        box-shadow: var(--shadow);
        overflow: hidden;
        backdrop-filter: blur(12px);
      }

      #sparkCanvas {
        position: absolute;
        inset: 0;
        width: 100%;
        height: 100%;
        pointer-events: none;
        mix-blend-mode: screen;
        opacity: 0.6;
      }

      .masthead {
        text-align: center;
        display: grid;
        gap: 1.25rem;
        margin-bottom: clamp(2.5rem, 6vw, 4rem);
        animation: fadeInUp 1s ease-out;
      }

      .masthead__badge {
        justify-self: center;
        font-family: "Playfair Display", serif;
        font-size: clamp(1.4rem, 4vw, 1.9rem);
        letter-spacing: 0.35em;
        padding: 0.55rem 1.5rem;
        border-radius: 999px;
        background: rgba(233, 95, 139, 0.15);
        border: 1px solid rgba(233, 95, 139, 0.4);
        text-transform: uppercase;
      }

      .masthead__title {
        font-family: "Playfair Display", serif;
        font-size: clamp(3.2rem, 6vw, 4.4rem);
        letter-spacing: 0.04em;
      }

      .masthead__subtitle {
        display: grid;
        gap: 0.6rem;
        font-size: clamp(1.05rem, 2vw, 1.3rem);
        color: var(--text-soft);
        max-width: 52ch;
        justify-self: center;
      }

      .masthead__cta {
        display: inline-flex;
        gap: 1rem;
        justify-self: center;
      }

      .masthead__cta button {
        padding: 0.9rem 1.8rem;
        border-radius: 999px;
        border: none;
        font-weight: 600;
        letter-spacing: 0.05em;
        cursor: pointer;
        transition: transform 200ms ease, box-shadow 200ms ease, background 200ms ease;
      }

      .masthead__cta button:first-child {
        background: linear-gradient(120deg, #ff97b7, #e95f8b);
        color: #fff;
        box-shadow: 0 18px 35px rgba(233, 95, 139, 0.35);
      }

      .masthead__cta button.ghost {
        background: rgba(255, 255, 255, 0.7);
        color: var(--text);
        border: 1px solid rgba(44, 42, 74, 0.08);
      }

      .masthead__cta button:hover,
      .masthead__cta button:focus-visible {
        transform: translateY(-4px) scale(1.05);
        box-shadow: 0 22px 38px rgba(233, 95, 139, 0.45);
      }

      .masthead__cta button.ghost:hover,
      .masthead__cta button.ghost:focus-visible {
        background: rgba(233, 95, 139, 0.12);
        box-shadow: 0 14px 30px rgba(44, 42, 74, 0.14);
      }

      nav {
        text-align: center;
        margin-bottom: 2rem;
      }

      nav a {
        margin: 0 1rem;
        color: var(--accent);
        text-decoration: none;
        font-weight: 600;
        transition: color 0.3s;
      }

      nav a:hover {
        color: var(--text);
      }

      .content {
        display: grid;
        gap: clamp(1.8rem, 4vw, 2.6rem);
      }

      .panel {
        background: var(--card);
        border-radius: var(--radius-lg);
        padding: clamp(1.8rem, 4vw, 2.6rem);
        box-shadow: 0 16px 40px rgba(46, 32, 86, 0.12);
        backdrop-filter: var(--blur);
        position: relative;
        overflow: hidden;
        animation: fadeInUp 1s ease-out;
        transition: transform 0.3s ease;
      }

      .panel:hover {
        transform: translateY(-5px);
      }

      .panel::before {
        content: "";
        position: absolute;
        inset: 0;
        background: linear-gradient(135deg, rgba(255, 255, 255, 0.18), transparent);
        opacity: 0.65;
        pointer-events: none;
      }

      .panel__header {
        display: grid;
        gap: 0.4rem;
        margin-bottom: 1.4rem;
        position: relative;
        z-index: 1;
      }

      .panel__eyebrow {
        font-size: 0.82rem;
        letter-spacing: 0.28em;
        text-transform: uppercase;
        color: rgba(44, 42, 74, 0.55);
      }

      .panel__header h2 {
        font-family: "Playfair Display", serif;
        font-size: clamp(1.8rem, 3vw, 2.4rem);
      }

      .panel p,
      .panel footer {
        position: relative;
        z-index: 1;
        color: var(--text-soft);
        line-height: 1.7;
        font-size: 1.02rem;
      }

      .panel footer {
        margin-top: 1rem;
        font-style: italic;
      }

      .panel--quote p {
        font-size: clamp(1.1rem, 2vw, 1.35rem);
        line-height: 1.75;
      }

      .timeline {
        list-style: none;
        display: grid;
        gap: 1.6rem;
        position: relative;
        z-index: 1;
      }

      .timeline::before {
        content: "";
        position: absolute;
        top: 0.4rem;
        bottom: 0.4rem;
        left: 1.25rem;
        width: 2px;
        background: linear-gradient(180deg, rgba(233, 95, 139, 0.45), rgba(233, 95, 139, 0));
      }

      .timeline li {
        display: grid;
        grid-template-columns: auto 1fr;
        gap: 1.4rem;
        align-items: start;
        transition: transform 0.3s ease, opacity 0.3s ease;
        opacity: 0;
        transform: translateX(-20px);
      }

      .timeline li.visible {
        opacity: 1;
        transform: translateX(0);
      }

      .timeline time {
        font-family: "Playfair Display", serif;
        font-size: 1.1rem;
        color: var(--accent);
        position: relative;
        padding-left: 2.5rem;
      }

      .timeline time::before {
        content: "";
        position: absolute;
        left: 0.4rem;
        top: 0.45rem;
        width: 9px;
        height: 9px;
        border-radius: 50%;
        background: #fff;
        border: 3px solid var(--accent);
        box-shadow: 0 0 0 6px rgba(233, 95, 139, 0.12);
      }

      .timeline strong {
        font-weight: 600;
        display: block;
        margin-bottom: 0.25rem;
        color: var(--text);
      }

      .panel--message {
        display: grid;
        gap: 1.6rem;
      }

      .message-form {
        display: grid;
        gap: 1rem;
        position: relative;
        z-index: 1;
      }

      .message-form label {
        display: grid;
        gap: 0.5rem;
        font-weight: 600;
        color: rgba(44, 42, 74, 0.8);
      }

      .message-form textarea {
        resize: vertical;
        min-height: 120px;
        border: none;
        border-radius: var(--radius-md);
        padding: 1rem 1.2rem;
        background: rgba(255, 255, 255, 0.85);
        box-shadow: inset 0 0 0 1px rgba(233, 95, 139, 0.12);
        font-family: "Be Vietnam Pro", sans-serif;
        font-size: 1rem;
        color: var(--text);
        transition: box-shadow 0.3s ease;
      }

      .message-form textarea:focus-visible {
        outline: none;
        box-shadow: 0 0 0 3px rgba(233, 95, 139, 0.25);
      }

      .message-form button {
        justify-self: end;
        padding: 0.75rem 1.6rem;
        border-radius: 999px;
        border: none;
        background: linear-gradient(120deg, #ffd3a4, #ff7aa5);
        color: #fff;
        font-weight: 600;
        letter-spacing: 0.05em;
        cursor: pointer;
        box-shadow: 0 16px 32px rgba(233, 95, 139, 0.28);
        transition: transform 200ms ease, box-shadow 200ms ease;
      }

      .message-form button:hover,
      .message-form button:focus-visible {
        transform: translateY(-3px) scale(1.05);
        box-shadow: 0 20px 36px rgba(233, 95, 139, 0.38);
      }

      .message-wall {
        display: grid;
        gap: 0.8rem;
      }

      .message-card {
        background: rgba(255, 255, 255, 0.92);
        border-radius: var(--radius-md);
        padding: 0.9rem 1.1rem;
        box-shadow: 0 14px 26px rgba(46, 32, 86, 0.1);
        animation: floatIn 400ms ease forwards;
      }

      .message-card p {
        font-size: 0.98rem;
        color: rgba(44, 42, 74, 0.85);
        line-height: 1.6;
      }

      .footer {
        margin-top: clamp(2.5rem, 4vw, 3.3rem);
        text-align: center;
        font-size: 0.95rem;
        letter-spacing: 0.28em;
        text-transform: uppercase;
        color: rgba(44, 42, 74, 0.55);
        animation: fadeInUp 1s ease-out 2s;
      }

      @keyframes fadeInUp {
        from {
          opacity: 0;
          transform: translateY(20px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }

      @keyframes floatIn {
        from {
          transform: translateY(16px);
          opacity: 0;
        }
        to {
          transform: translateY(0);
          opacity: 1;
        }
      }

      /* Carousel Styles */
      .fact-carousel {
        position: relative;
        max-width: 100%;
        margin-bottom: 2rem;
        animation: fadeInUp 1s ease-out;
      }

      .fact-carousel__viewport {
        overflow: hidden;
      }

      .fact-carousel__slides {
        display: flex;
        transition: transform 0.5s ease;
        list-style: none;
      }

      .fact-carousel__slide {
        flex: 0 0 100%;
        padding: 1rem;
        text-align: center;
        background: var(--card);
        border-radius: var(--radius-md);
        box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      }

      .fact-carousel__slide h3 {
        font-size: 1.5rem;
        margin-bottom: 0.5rem;
      }

      .fact-carousel__slide p {
        font-size: 1rem;
        color: var(--text-soft);
      }

      .fact-carousel__control {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        background: rgba(255,255,255,0.8);
        border: none;
        font-size: 2rem;
        cursor: pointer;
        padding: 0 1rem;
        transition: background 0.3s;
      }

      .fact-carousel__control:hover {
        background: rgba(233, 95, 139, 0.5);
      }

      .fact-carousel__control--prev {
        left: 0;
      }

      .fact-carousel__control--next {
        right: 0;
      }

      /* Confetti */
      .confetti {
        position: absolute;
        width: 10px;
        height: 10px;
        background: red;
        opacity: 0.8;
        animation: confetti-fall 3s linear infinite;
      }

      @keyframes confetti-fall {
        0% {
          transform: translateY(0) rotate(0);
          opacity: 1;
        }
        100% {
          transform: translateY(100vh) rotate(360deg);
          opacity: 0;
        }
      }

      @media (max-width: 768px) {
        body {
          padding: 1.5rem;
        }

        .stage {
          padding: clamp(1.8rem, 6vw, 2.4rem);
        }

        .masthead__cta {
          flex-direction: column;
          width: 100%;
        }

        .masthead__cta button,
        .message-form button {
          width: 100%;
        }

        .timeline::before {
          left: 0;
        }

        .timeline li {
          grid-template-columns: 1fr;
          padding-left: 1.8rem;
        }

        .timeline time {
          padding-left: 0;
        }

        .timeline time::before {
          left: -1.8rem;
        }

        nav {
          display: flex;
          flex-direction: column;
        }

        nav a {
          margin: 0.5rem 0;
        }
      }

      @media (max-width: 480px) {
        .masthead__title {
          font-size: 2.5rem;
        }

        .panel {
          padding: 1.5rem;
        }
      }
    </style>
  </head>
  <body>
    <div class="stage">
      <canvas id="sparkCanvas" aria-hidden="true"></canvas>
      <header class="masthead">
        <div class="masthead__badge">20 • 11</div>
        <h1 class="masthead__title">Thầy cô trong tim</h1>
        <p class="masthead__subtitle">
          <span>Tri ân những người viết nên tương lai bằng từng nét phấn trắng.</span>
          <span>Ngày Nhà giáo Việt Nam – khoảnh khắc để nói lời cảm ơn.</span>
        </p>
        <div class="masthead__cta">
          <button id="playSongBtn" type="button">Phát giai điệu tri ân</button>
          <button id="lightUpBtn" type="button" class="ghost">Thắp sáng lời chúc</button>
        </div>
      </header>
      <nav>
        <a href="#quote">Trích dẫn</a>
        <a href="#timeline">Dòng ký ức</a>
        <a href="#message">Lời nhắn gửi</a>
      </nav>
      <main class="content">
        <aside class="fact-carousel" aria-label="Số liệu nổi bật về ngày 20 tháng 11">
          <button class="fact-carousel__control fact-carousel__control--prev" aria-label="Xem thông tin trước">
            ‹
          </button>
          <div class="fact-carousel__viewport">
            <ul class="fact-carousel__slides" id="factSlides">
              <li class="fact-carousel__slide">
                <h3>Gần 1.28 triệu giáo viên</h3>
                <p>Toàn ngành giáo dục Việt Nam có gần 1.28 triệu giáo viên vào cuối năm học 2024-2025.</p>
              </li>
              <li class="fact-carousel__slide">
                <h3>Hơn 25 triệu học sinh, sinh viên</h3>
                <p>Năm học 2024-2025, cả nước có 25.255.251 học sinh, sinh viên.</p>
              </li>
              <li class="fact-carousel__slide">
                <h3>Thiếu hơn 120.000 giáo viên</h3>
                <p>Cả nước đang thiếu hơn 120.000 giáo viên các cấp.</p>
              </li>
              <li class="fact-carousel__slide">
                <h3>Gần 54.000 cơ sở giáo dục</h3>
                <p>Có 53.979 cơ sở giáo dục trên toàn quốc.</p>
              </li>
              <li class="fact-carousel__slide">
                <h3>43 năm Ngày Nhà giáo</h3>
                <p>Năm 2025 kỷ niệm 43 năm Ngày Nhà giáo Việt Nam (từ 1982).</p>
              </li>
            </ul>
          </div>
          <button class="fact-carousel__control fact-carousel__control--next" aria-label="Xem thông tin tiếp theo">
            ›
          </button>
        </aside>
        <section class="panel panel--quote" id="quote">
          <div class="panel__header">
            <span class="panel__eyebrow">Trích dẫn</span>
            <h2>Bàn tay người cô yêu dấu</h2>
          </div>
          <p>
            “Nếu có một điều bất biến giữa muôn vàn đổi thay, đó chính là ánh mắt tin tưởng của cô Hạnh dành cho học trò.
            Ánh mắt ấy đã nâng những ước mơ bay cao, đã xoa dịu bao lần vấp ngã, và đã dạy chúng ta cách yêu thương trọn vẹn.”
          </p>
          <footer>— Theo học sinh 9/9</footer>
        </section>
        <section class="panel panel--timeline" id="timeline">
          <div class="panel__header">
            <span class="panel__eyebrow">Dòng ký ức</span>
            <h2>Quá trình phát triển</h2>
          </div>
          <ul class="timeline">
            <li>
              <time>1958</time>
              <div>
                <strong>Ngày đầu tri ân</strong>
                <p>Miền Bắc hưởng ứng “Ngày Quốc tế các Nhà giáo”, mở đầu cho truyền thống tri ân ngày 20/11.</p>
              </div>
            </li>
            <li>
              <time>1982</time>
              <div>
                <strong>Chính thức hoá</strong>
                <p>Quyết định 167/HĐBT ghi nhận 20/11 là Ngày Nhà giáo Việt Nam trên toàn quốc.</p>
              </div>
            </li>
            <li>
              <time>2008</time>
              <div>
                <strong>Thời đại mới</strong>
                <p>Lớp học số hoá, bài giảng trực tuyến giúp tình thầy trò vượt qua khoảng cách địa lý.</p>
              </div>
            </li>
            <li>
              <time>Hôm nay</time>
              <div>
                <strong>Lời chúc lan toả</strong>
                <p>Bức thư viết tay, bông hoa điểm 10... tất cả cùng nói một lời: “Chúng em biết ơn thầy cô”.</p>
              </div>
            </li>
          </ul>
        </section>
        <section class="panel panel--message" id="message">
          <div class="panel__header">
            <span class="panel__eyebrow">Lời nhắn gửi</span>
            <h2>Viết cho cô</h2>
          </div>
          <form class="message-form" id="messageForm">
            <label>
              <span>Lời cảm ơn</span>
              <textarea id="messageInput" rows="4" placeholder="Viết vài dòng dành cho thầy cô yêu quý của bạn..."></textarea>
            </label>
            <button type="submit">Gửi bằng trái tim</button>
          </form>
          <div class="message-wall" id="messageWall" aria-live="polite"></div>
        </section>
      </main>
      <footer class="footer">
        <small>Trao yêu thương • Giữ truyền thống • Vun tương lai</small>
      </footer>
      <audio id="gratitudeTrack" src="https://cdn.pixabay.com/download/audio/2022/03/08/audio_4a31c5ed5e.mp3?filename=nostalgic-piano-112199.mp3"></audio>
    </div>
    <script defer>
      (() => {
        const canvas = document.getElementById('sparkCanvas');
        const playSongBtn = document.getElementById('playSongBtn');
        const lightUpBtn = document.getElementById('lightUpBtn');
        const audio = document.getElementById('gratitudeTrack');
        const messageForm = document.getElementById('messageForm');
        const messageInput = document.getElementById('messageInput');
        const messageWall = document.getElementById('messageWall');
        const panels = Array.from(document.querySelectorAll('.panel'));
        const timelineItems = Array.from(document.querySelectorAll('.timeline li'));

        // Sparkle canvas -----------------------------------------------------------
        const config = {
          count: 80,
          minSize: 2,
          maxSize: 5,
          minSpeed: 0.15,
          maxSpeed: 0.6,
        };

        let ctx;
        let sparks = [];
        let frame;

        const resizeCanvas = () => {
          if (!canvas) return;
          canvas.width = canvas.offsetWidth;
          canvas.height = canvas.offsetHeight;
          ctx = canvas.getContext('2d');
          createSparks();
        };

        const createSparks = () => {
          sparks = Array.from({ length: config.count }, () => ({
            x: Math.random() * canvas.width,
            y: Math.random() * canvas.height,
            size: config.minSize + Math.random() * (config.maxSize - config.minSize),
            speed: config.minSpeed + Math.random() * (config.maxSpeed - config.minSpeed),
            angle: Math.random() * Math.PI * 2,
            alpha: 0.4 + Math.random() * 0.4,
          }));
        };

        const drawSparks = () => {
          if (!ctx) return;
          ctx.clearRect(0, 0, canvas.width, canvas.height);
          sparks.forEach((spark) => {
            ctx.beginPath();
            const gradient = ctx.createRadialGradient(spark.x, spark.y, 0, spark.x, spark.y, spark.size * 2);
            gradient.addColorStop(0, `rgba(255,255,255,${spark.alpha})`);
            gradient.addColorStop(1, 'rgba(255,255,255,0)');
            ctx.fillStyle = gradient;
            ctx.arc(spark.x, spark.y, spark.size * 2, 0, Math.PI * 2);
            ctx.fill();

            spark.x += Math.cos(spark.angle) * spark.speed;
            spark.y += Math.sin(spark.angle) * spark.speed;
            spark.angle += (Math.random() - 0.5) * 0.05;

            if (spark.x < -20) spark.x = canvas.width + 20;
            if (spark.x > canvas.width + 20) spark.x = -20;
            if (spark.y < -20) spark.y = canvas.height + 20;
            if (spark.y > canvas.height + 20) spark.y = -20;
          });
          frame = requestAnimationFrame(drawSparks);
        };

        // Audio control ------------------------------------------------------------
        if (playSongBtn && audio) {
          playSongBtn.addEventListener('click', () => {
            if (audio.paused) {
              audio.play().catch(() => {});
              playSongBtn.textContent = 'Tạm dừng giai điệu';
            } else {
              audio.pause();
              playSongBtn.textContent = 'Phát giai điệu tri ân';
            }
          });

          audio.addEventListener('ended', () => {
            playSongBtn.textContent = 'Phát lại giai điệu';
          });
        }

        // Light up panels ---------------------------------------------------------
        let lit = false;
        if (lightUpBtn) {
          lightUpBtn.addEventListener('click', () => {
            lit = !lit;
            panels.forEach((panel, index) => {
              panel.style.transition = 'box-shadow 400ms ease, transform 400ms ease';
              if (lit) {
                const offset = (index % 2 === 0 ? 1 : -1) * 6;
                panel.style.boxShadow = `0 26px 60px rgba(233, 95, 139, 0.28)`;
                panel.style.transform = `translateY(${offset}px)`;
              } else {
                panel.style.boxShadow = '0 16px 40px rgba(46, 32, 86, 0.12)';
                panel.style.transform = 'translateY(0)';
              }
            });
            lightUpBtn.textContent = lit ? 'Ánh sáng đã lên' : 'Thắp sáng lời chúc';
          });
        }

        // Message wall ------------------------------------------------------------
        const createMessageCard = (message) => {
          const card = document.createElement('div');
          card.className = 'message-card';
          const paragraph = document.createElement('p');
          paragraph.textContent = message;
          card.appendChild(paragraph);
          return card;
        };

        if (messageForm && messageInput && messageWall) {
          messageForm.addEventListener('submit', (event) => {
            event.preventDefault();
            const text = messageInput.value.trim();
            if (!text) return;
            const card = createMessageCard(text);
            messageWall.prepend(card);
            messageInput.value = '';
            messageInput.focus();
            triggerConfetti();
          });
        }

        // Carousel ----------------------------------------------------------------
        const prevBtn = document.querySelector('.fact-carousel__control--prev');
        const nextBtn = document.querySelector('.fact-carousel__control--next');
        const slidesContainer = document.getElementById('factSlides');
        const slides = Array.from(slidesContainer.children);
        let currentIndex = 0;

        const showSlide = (index) => {
          slidesContainer.style.transform = `translateX(-${index * 100}%)`;
        };

        if (prevBtn && nextBtn && slides.length > 0) {
          prevBtn.addEventListener('click', () => {
            currentIndex = (currentIndex - 1 + slides.length) % slides.length;
            showSlide(currentIndex);
          });

          nextBtn.addEventListener('click', () => {
            currentIndex = (currentIndex + 1) % slides.length;
            showSlide(currentIndex);
          });

          // Auto slide
          setInterval(() => {
            currentIndex = (currentIndex + 1) % slides.length;
            showSlide(currentIndex);
          }, 5000);
        }

        // Confetti effect
        const colors = ['#ff0000', '#00ff00', '#0000ff', '#ffff00', '#ff00ff', '#00ffff'];

        const triggerConfetti = () => {
          for (let i = 0; i < 100; i++) {
            const confetti = document.createElement('div');
            confetti.className = 'confetti';
            confetti.style.position = 'fixed';
            confetti.style.left = `${Math.random() * 100}vw`;
            confetti.style.top = '-10px';
            confetti.style.background = colors[Math.floor(Math.random() * colors.length)];
            confetti.style.animationDelay = `${Math.random() * 2}s`;
            confetti.style.animationDuration = `${3 + Math.random() * 2}s`;
            document.body.appendChild(confetti);
            setTimeout(() => {
              confetti.remove();
            }, 5000);
          }
        };

        // Timeline animation
        const observer = new IntersectionObserver((entries) => {
          entries.forEach((entry, index) => {
            if (entry.isIntersecting) {
              setTimeout(() => {
                entry.target.classList.add('visible');
              }, index * 200);
            }
          });
        }, { threshold: 0.1 });

        timelineItems.forEach(item => observer.observe(item));

        // Initialise --------------------------------------------------------------
        const init = () => {
          if (!canvas) return;
          resizeCanvas();
          window.addEventListener('resize', () => {
            cancelAnimationFrame(frame);
            resizeCanvas();
            drawSparks();
          });
          drawSparks();
        };

        init();
      })();
    </script>
  </body>
</html>
