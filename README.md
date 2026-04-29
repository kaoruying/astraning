<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>主任必修課程｜晉升後3～6個月增員培訓課程</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Microsoft JhengHei", "Noto Sans TC", Arial, sans-serif;
      background:
        radial-gradient(circle at 15% 10%, rgba(0, 145, 255, 0.45), transparent 28%),
        radial-gradient(circle at 85% 15%, rgba(255, 153, 0, 0.35), transparent 24%),
        linear-gradient(135deg, #031026 0%, #071c44 48%, #020817 100%);
      color: #ffffff;
      overflow-x: hidden;
    }

    body::before {
      content: "";
      position: fixed;
      inset: 0;
      background-image:
        linear-gradient(rgba(255,255,255,0.06) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,255,255,0.06) 1px, transparent 1px);
      background-size: 44px 44px;
      pointer-events: none;
      opacity: 0.45;
      z-index: 0;
    }

    .page {
      position: relative;
      z-index: 1;
      max-width: 1180px;
      margin: 0 auto;
      padding: 36px 18px 56px;
    }

    .hero {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 32px;
      align-items: center;
      min-height: 640px;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 9px 18px;
      border: 1px solid rgba(255, 199, 87, 0.8);
      border-radius: 999px;
      background: rgba(255, 170, 35, 0.13);
      color: #ffe3a1;
      font-weight: 800;
      letter-spacing: 1px;
      box-shadow: 0 0 22px rgba(255, 171, 35, 0.18);
    }

    h1 {
      margin-top: 24px;
      font-size: clamp(48px, 7vw, 82px);
      line-height: 1.05;
      font-weight: 950;
      letter-spacing: -2px;
      text-shadow: 0 8px 28px rgba(0,0,0,0.5);
    }

    .gold {
      background: linear-gradient(135deg, #fff1b8, #ffad2f 45%, #ff6f00);
      -webkit-background-clip: text;
      color: transparent;
      filter: drop-shadow(0 0 12px rgba(255, 167, 38, 0.3));
    }

    .subtitle {
      margin-top: 20px;
      font-size: clamp(21px, 2.2vw, 30px);
      font-weight: 900;
      color: #ffd873;
    }

    .lead {
      margin-top: 20px;
      max-width: 680px;
      color: rgba(236, 246, 255, 0.92);
      font-size: 18px;
      line-height: 1.9;
      font-weight: 500;
    }

    .highlight {
      margin-top: 26px;
      padding: 18px 22px;
      border-radius: 22px;
      border: 1px solid rgba(255, 203, 93, 0.75);
      background: linear-gradient(90deg, rgba(255, 164, 28, 0.28), rgba(255, 111, 0, 0.18));
      box-shadow: 0 12px 35px rgba(255, 128, 0, 0.16);
      font-size: clamp(20px, 2.3vw, 30px);
      font-weight: 950;
      color: #fff0bd;
    }

    .visual-card {
      position: relative;
      border-radius: 32px;
      padding: 28px;
      border: 1px solid rgba(161, 207, 255, 0.35);
      background: rgba(255,255,255,0.09);
      backdrop-filter: blur(14px);
      box-shadow: 0 30px 80px rgba(0,0,0,0.35);
      overflow: hidden;
    }

    .visual-card::before {
      content: "";
      position: absolute;
      width: 300px;
      height: 300px;
      right: -90px;
      top: -80px;
      background: radial-gradient(circle, rgba(255, 157, 29, 0.5), transparent 68%);
    }

    .rocket {
      position: relative;
      height: 360px;
      border-radius: 26px;
      background:
        radial-gradient(circle at 72% 28%, rgba(255, 193, 7, 0.55), transparent 18%),
        linear-gradient(160deg, rgba(10, 45, 100, 0.95), rgba(2, 12, 31, 0.9));
      border: 1px solid rgba(255,255,255,0.15);
      overflow: hidden;
    }

    .rocket-icon {
      position: absolute;
      right: 52px;
      top: 52px;
      font-size: 90px;
      transform: rotate(22deg);
      filter: drop-shadow(0 0 22px rgba(255, 185, 49, 0.75));
      animation: float 2.8s ease-in-out infinite;
    }

    .arrow {
      position: absolute;
      left: 48px;
      bottom: 72px;
      width: 72%;
      height: 72px;
      border-top: 14px solid #ffb12b;
      border-right: 14px solid #ffb12b;
      transform: skewX(-20deg) rotate(-18deg);
      border-radius: 8px;
      box-shadow: 0 0 28px rgba(255, 166, 31, 0.55);
    }

    .bars {
      position: absolute;
      left: 34px;
      bottom: 34px;
      display: flex;
      align-items: end;
      gap: 12px;
    }

    .bar {
      width: 32px;
      border-radius: 10px 10px 0 0;
      background: linear-gradient(#43c7ff, #0b65cf);
      box-shadow: 0 0 18px rgba(54, 186, 255, 0.55);
    }

    .bar:nth-child(1) { height: 58px; }
    .bar:nth-child(2) { height: 92px; }
    .bar:nth-child(3) { height: 130px; }
    .bar:nth-child(4) { height: 172px; }

    .mini-title {
      margin-top: 24px;
      font-size: 26px;
      font-weight: 950;
    }

    .mini-desc {
      margin-top: 10px;
      color: rgba(229, 241, 255, 0.86);
      line-height: 1.7;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0) rotate(22deg); }
      50% { transform: translateY(-12px) rotate(22deg); }
    }

    .section {
      margin-top: 42px;
      border-radius: 32px;
      padding: 30px;
      background: rgba(255,255,255,0.1);
      border: 1px solid rgba(255,255,255,0.16);
      backdrop-filter: blur(14px);
      box-shadow: 0 24px 60px rgba(0,0,0,0.22);
    }

    .section-title {
      display: flex;
      align-items: center;
      gap: 12px;
      margin-bottom: 22px;
      font-size: clamp(28px, 3vw, 42px);
      font-weight: 950;
    }

    .number {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 42px;
      height: 42px;
      border-radius: 50%;
      background: linear-gradient(135deg, #ffd66b, #ff8a00);
      color: #06142f;
      font-weight: 950;
      box-shadow: 0 0 18px rgba(255, 168, 33, 0.55);
      flex-shrink: 0;
    }

    .pain-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 14px;
    }

    .pain-card {
      padding: 20px 16px;
      border-radius: 22px;
      background: #ffffff;
      color: #0c1d3d;
      min-height: 145px;
      box-shadow: 0 16px 34px rgba(0,0,0,0.2);
      border: 2px solid rgba(255, 166, 31, 0.18);
    }

    .pain-card .icon {
      font-size: 30px;
      margin-bottom: 12px;
    }

    .pain-card p {
      font-weight: 850;
      line-height: 1.5;
    }

    .course-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 22px;
    }

    .course-card {
      background: #ffffff;
      color: #0d1c3a;
      border-radius: 28px;
      padding: 28px;
      border: 3px solid rgba(255, 166, 31, 0.22);
      box-shadow: 0 24px 50px rgba(0,0,0,0.28);
    }

    .course-card h3 {
      font-size: 32px;
      font-weight: 950;
      color: #0a2f70;
    }

    .course-card .focus {
      margin-top: 8px;
      font-weight: 900;
      color: #e67400;
      line-height: 1.5;
    }

    .course-card ul {
      margin-top: 20px;
      list-style: none;
      display: grid;
      gap: 12px;
    }

    .course-card li {
      display: flex;
      gap: 10px;
      line-height: 1.55;
      font-weight: 750;
      padding: 12px 14px;
      border-radius: 16px;
      background: #eef6ff;
    }

    .course-card li::before {
      content: "✓";
      width: 23px;
      height: 23px;
      border-radius: 50%;
      background: #ff8a00;
      color: #ffffff;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-weight: 950;
      flex-shrink: 0;
    }

    .r-layout {
      display: grid;
      grid-template-columns: 0.95fr 1.05fr;
      gap: 26px;
      align-items: stretch;
    }

    .r-buttons {
      display: grid;
      gap: 12px;
    }

    .r-btn {
      border: 1px solid rgba(255,255,255,0.18);
      background: rgba(255,255,255,0.1);
      color: white;
      padding: 16px;
      border-radius: 18px;
      cursor: pointer;
      text-align: left;
      font-size: 17px;
      font-weight: 850;
      transition: 0.25s;
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .r-btn:hover,
    .r-btn.active {
      transform: translateX(6px);
      background: linear-gradient(90deg, rgba(255, 168, 38, 0.35), rgba(21, 114, 255, 0.22));
      border-color: rgba(255, 210, 107, 0.8);
      box-shadow: 0 0 24px rgba(255, 170, 35, 0.2);
    }

    .r-code {
      padding: 7px 12px;
      border-radius: 12px;
      background: #051433;
      color: #ffd66b;
      font-weight: 950;
    }

    .r-display {
      background: #ffffff;
      color: #0b1b38;
      border-radius: 28px;
      padding: 30px;
      min-height: 410px;
      box-shadow: 0 22px 48px rgba(0,0,0,0.25);
      position: relative;
      overflow: hidden;
    }

    .r-display::after {
      content: "";
      position: absolute;
      right: -70px;
      top: -80px;
      width: 220px;
      height: 220px;
      background: radial-gradient(circle, rgba(255, 165, 0, 0.35), transparent 68%);
    }

    .r-display h3 {
      font-size: 46px;
      color: #0a2f70;
      font-weight: 950;
    }

    .r-display h4 {
      margin-top: 10px;
      font-size: 26px;
      color: #e67400;
      font-weight: 950;
    }

    .r-display .desc {
      margin-top: 18px;
      font-size: 18px;
      line-height: 1.75;
      font-weight: 700;
      color: #273852;
    }

    .info-box {
      margin-top: 18px;
      padding: 18px;
      border-radius: 20px;
      background: #eef6ff;
      border-left: 7px solid #ff9d16;
    }

    .info-box b {
      color: #0a2f70;
      display: block;
      margin-bottom: 8px;
      font-size: 18px;
    }

    .outcome-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 16px;
    }

    .outcome-card {
      padding: 24px;
      border-radius: 24px;
      background: rgba(255,255,255,0.12);
      border: 1px solid rgba(255,255,255,0.15);
      min-height: 210px;
    }

    .outcome-card .icon {
      font-size: 36px;
      margin-bottom: 16px;
    }

    .outcome-card h3 {
      color: #ffd66b;
      font-size: 24px;
      margin-bottom: 10px;
      font-weight: 950;
    }

    .outcome-card p {
      color: rgba(235, 246, 255, 0.88);
      line-height: 1.7;
      font-weight: 650;
    }

    .quiz-wrap {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 22px;
    }

    .quiz-card {
      background: #ffffff;
      color: #0b1b38;
      border-radius: 28px;
      padding: 28px;
      box-shadow: 0 24px 50px rgba(0,0,0,0.25);
    }

    .quiz-card h3 {
      font-size: 30px;
      color: #0a2f70;
      font-weight: 950;
      margin-bottom: 10px;
    }

    .quiz-desc {
      color: #536179;
      line-height: 1.7;
      font-weight: 650;
      margin-bottom: 20px;
    }

    .question {
      margin-top: 20px;
    }

    .question-title {
      font-weight: 950;
      margin-bottom: 10px;
    }

    .option {
      width: 100%;
      text-align: left;
      padding: 13px 15px;
      margin-bottom: 9px;
      border-radius: 14px;
      border: 1px solid #ccd7e8;
      background: #f8fbff;
      cursor: pointer;
      font-weight: 750;
      color: #19304f;
      transition: 0.2s;
    }

    .option:hover,
    .option.selected {
      background: #fff1d7;
      border-color: #ff9d16;
      color: #d86600;
    }

    .result-box {
      background:
        linear-gradient(135deg, rgba(255, 160, 28, 0.24), rgba(0, 110, 255, 0.18)),
        rgba(255,255,255,0.1);
      border: 1px solid rgba(255, 213, 119, 0.45);
      border-radius: 28px;
      padding: 28px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .result-box h3 {
      font-size: 30px;
      font-weight: 950;
      color: #ffd66b;
    }

    .result-text {
      margin-top: 18px;
      font-size: 22px;
      line-height: 1.7;
      font-weight: 900;
      color: #ffffff;
    }

    .cta {
      margin-top: 42px;
      text-align: center;
      padding: 44px 28px;
      border-radius: 36px;
      border: 1px solid rgba(255, 210, 107, 0.55);
      background:
        radial-gradient(circle at 15% 30%, rgba(255, 171, 35, 0.32), transparent 25%),
        linear-gradient(135deg, rgba(9, 43, 105, 0.96), rgba(119, 58, 0, 0.85));
      box-shadow: 0 30px 80px rgba(0,0,0,0.36);
    }

    .cta h2 {
      font-size: clamp(42px, 6vw, 78px);
      line-height: 1.08;
      font-weight: 950;
      margin-bottom: 16px;
    }

    .cta p {
      font-size: 22px;
      line-height: 1.8;
      font-weight: 800;
      color: rgba(255,255,255,0.9);
    }

    .cta-buttons {
      margin-top: 28px;
      display: flex;
      justify-content: center;
      gap: 14px;
      flex-wrap: wrap;
    }

    .btn {
      border: none;
      padding: 16px 28px;
      border-radius: 16px;
      cursor: pointer;
      font-size: 18px;
      font-weight: 950;
      transition: 0.25s;
    }

    .btn-primary {
      background: linear-gradient(135deg, #ffd66b, #ff8a00);
      color: #06142f;
      box-shadow: 0 14px 30px rgba(255, 145, 0, 0.28);
    }

    .btn-secondary {
      background: rgba(255,255,255,0.13);
      color: white;
      border: 1px solid rgba(255,255,255,0.35);
    }

    .btn:hover {
      transform: translateY(-3px);
      filter: brightness(1.05);
    }

    .footer-note {
      margin-top: 22px;
      color: rgba(232, 244, 255, 0.7);
      font-size: 14px;
      text-align: center;
    }

    @media (max-width: 980px) {
      .hero,
      .r-layout,
      .quiz-wrap,
      .course-grid {
        grid-template-columns: 1fr;
      }

      .pain-grid {
        grid-template-columns: 1fr 1fr;
      }

      .outcome-grid {
        grid-template-columns: 1fr 1fr;
      }

      .hero {
        min-height: auto;
      }
    }

    @media (max-width: 620px) {
      .page {
        padding: 24px 14px 42px;
      }

      .section {
        padding: 22px;
        border-radius: 26px;
      }

      .pain-grid,
      .outcome-grid {
        grid-template-columns: 1fr;
      }

      .visual-card {
        padding: 18px;
      }

      .rocket {
        height: 260px;
      }

      .rocket-icon {
        font-size: 72px;
        right: 35px;
      }

      .course-card,
      .quiz-card,
      .r-display {
        padding: 22px;
      }

      .cta {
        padding: 34px 20px;
      }
    }
  </style>
</head>

<body>
  <div class="page">

    <section class="hero">
      <div>
        <div class="badge">★ 主任必修課程 ★</div>

        <h1>
          晉升後 <span class="gold">3～6個月</span><br />
          增員培訓課程
        </h1>

        <div class="subtitle">以 R 線為主軸，打造主任增員實戰力</div>

        <p class="lead">
          晉升主任後，真正的挑戰，不只是延續個人業績，
          而是開始面對增員、推進增員，並建立屬於自己的增員節奏。
          這堂課以公司 R 線增員流程為主軸，
          從 R1 取得名單到 R6 新人報聘，
          系統化培養主任在各階段需要具備的增員能力。
        </p>

        <div class="highlight">
          把增員從「知道重要」，變成「知道怎麼做」
        </div>
      </div>

      <div class="visual-card">
        <div class="rocket">
          <div class="rocket-icon">🚀</div>
          <div class="arrow"></div>
          <div class="bars">
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
          </div>
        </div>

        <div class="mini-title">從業務高手，走向增員推手</div>
        <p class="mini-desc">
          讓主任不只會做業績，更能掌握名單、接觸、需求、邀約、追蹤與報聘推進。
        </p>
      </div>
    </section>

    <section class="section">
      <div class="section-title">
        <span class="number">1</span>
        為什麼要上這堂課？
      </div>

      <div class="pain-grid">
        <div class="pain-card">
          <div class="icon">📍</div>
          <p>想增員，卻不知道從哪裡開始</p>
        </div>
        <div class="pain-card">
          <div class="icon">👥</div>
          <p>有名單，卻不知道怎麼接觸與往下推</p>
        </div>
        <div class="pain-card">
          <div class="icon">💬</div>
          <p>會聊天，卻不一定能發掘準增需求</p>
        </div>
        <div class="pain-card">
          <div class="icon">⚠️</div>
          <p>邀約常卡住，異議來了不知如何處理</p>
        </div>
        <div class="pain-card">
          <div class="icon">⏱️</div>
          <p>想把增員做穩，卻缺少完整方法與節奏</p>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-title">
        <span class="number">2</span>
        你可以學到什麼？
      </div>

      <div class="course-grid">
        <div class="course-card">
          <h3>主任經典基礎班</h3>
          <div class="focus">聚焦增員起步與基本功建立｜打穩 R1～R2 基礎能力</div>
          <ul>
            <li>看懂 R 線全貌</li>
            <li>建立緣故名單與推薦人名單</li>
            <li>掌握增員定聯分級</li>
            <li>學會運用行為模式測驗開啟接觸</li>
            <li>學會邀約準增參加活動</li>
            <li>補強退休、稅務、保障等高效行銷切入點</li>
          </ul>
        </div>

        <div class="course-card">
          <h3>主任進階班</h3>
          <div class="focus">聚焦需求挖掘與推進能力｜強化 R2～R4 關鍵做法</div>
          <ul>
            <li>學會網路增員與陌生開發</li>
            <li>學會發掘準增需求與六大面向提問</li>
            <li>學會 FAB 邀約法與邀約下一步</li>
            <li>學會異議問題處理</li>
            <li>建立活動量管理與穩定增員節奏</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-title">
        <span class="number">3</span>
        R 線互動檢核
      </div>

      <div class="r-layout">
        <div class="r-buttons">
          <button class="r-btn active" onclick="showR(0, this)">
            <span class="r-code">R1</span> 取得名單
          </button>
          <button class="r-btn" onclick="showR(1, this)">
            <span class="r-code">R2</span> 啟動接觸
          </button>
          <button class="r-btn" onclick="showR(2, this)">
            <span class="r-code">R3</span> 發掘需求
          </button>
          <button class="r-btn" onclick="showR(3, this)">
            <span class="r-code">R4</span> 邀約推進
          </button>
          <button class="r-btn" onclick="showR(4, this)">
            <span class="r-code">R5</span> 面談追蹤
          </button>
          <button class="r-btn" onclick="showR(5, this)">
            <span class="r-code">R6</span> 新人報聘
          </button>
        </div>

        <div class="r-display">
          <h3 id="rCode">R1</h3>
          <h4 id="rTitle">取得名單</h4>
          <p class="desc" id="rDesc">
            建立緣故名單、推薦人名單，讓增員不是想到才做，而是有來源、有紀錄、有追蹤。
          </p>

          <div class="info-box">
            <b>常見卡點</b>
            <span id="rPain">不知道名單從哪裡來，或名單寫了卻沒有後續動作。</span>
          </div>

          <div class="info-box">
            <b>課程補強</b>
            <span id="rCourse">緣故名單盤點、推薦人名單建立、增員名單分類。</span>
          </div>

          <div class="info-box">
            <b>一句推進提醒</b>
            <span id="rTip">名單不是等出來的，是整理出來、問出來、累積出來的。</span>
          </div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-title">
        <span class="number">4</span>
        上完這堂課，你可以成為什麼樣的主任？
      </div>

      <div class="outcome-grid">
        <div class="outcome-card">
          <div class="icon">🛡️</div>
          <h3>角色更到位</h3>
          <p>清楚知道晉升後，主任每個階段該做什麼。</p>
        </div>

        <div class="outcome-card">
          <div class="icon">🎯</div>
          <h3>行銷有方向</h3>
          <p>不只會做業績，也懂得用議題切入市場。</p>
        </div>

        <div class="outcome-card">
          <div class="icon">📈</div>
          <h3>增員有方法</h3>
          <p>從名單、接觸、需求、邀約到推進，知道如何往下走。</p>
        </div>

        <div class="outcome-card">
          <div class="icon">⚙️</div>
          <h3>習慣能落地</h3>
          <p>不再只靠感覺增員，而是建立可持續的節奏與方法。</p>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-title">
        <span class="number">5</span>
        30 秒找出你的增員卡點
      </div>

      <div class="quiz-wrap">
        <div class="quiz-card">
          <h3>主任增員卡點檢測</h3>
          <p class="quiz-desc">
            請選出最接近你目前狀態的選項，完成後會出現建議學習方向。
          </p>

          <div class="question">
            <div class="question-title">1. 我現在最常卡在：</div>
            <button class="option" onclick="selectOption(0, 'basic', this)">不知道名單從哪裡來</button>
            <button class="option" onclick="selectOption(0, 'basic', this)">有名單但不敢接觸</button>
            <button class="option" onclick="selectOption(0, 'advance', this)">聊得起來但推不下去</button>
            <button class="option" onclick="selectOption(0, 'advance', this)">邀約或異議處理卡住</button>
          </div>

          <div class="question">
            <div class="question-title">2. 我最想補強的是：</div>
            <button class="option" onclick="selectOption(1, 'basic', this)">建立完整增員流程</button>
            <button class="option" onclick="selectOption(1, 'basic', this)">提升接觸與邀約能力</button>
            <button class="option" onclick="selectOption(1, 'advance', this)">發掘準增需求</button>
            <button class="option" onclick="selectOption(1, 'advance', this)">建立穩定增員節奏</button>
          </div>

          <div class="question">
            <div class="question-title">3. 目前我的增員狀態比較像：</div>
            <button class="option" onclick="selectOption(2, 'basic', this)">知道重要，但還沒開始</button>
            <button class="option" onclick="selectOption(2, 'basic', this)">偶爾做，但不穩定</button>
            <button class="option" onclick="selectOption(2, 'advance', this)">有行動，但缺方法</button>
            <button class="option" onclick="selectOption(2, 'advance', this)">想做出固定成果</button>
          </div>

          <button class="btn btn-primary" style="width:100%; margin-top:22px;" onclick="showResult()">
            查看建議課程
          </button>
        </div>

        <div class="result-box">
          <div>
            <h3>你的建議學習方向</h3>
            <div class="result-text" id="resultText">
              完成左側三題後，點選「查看建議課程」。
            </div>
          </div>

          <div style="margin-top:26px; padding:20px; border-radius:22px; background:rgba(255,255,255,0.1);">
            <h3 style="font-size:24px;">適合對象</h3>
            <p style="margin-top:10px; line-height:1.8; font-weight:800;">
              新晉升主任 3～6 個月內<br />
              想穩住角色、建立方法、養成節奏、做出成果。
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="cta">
      <h2>
        從業務高手，<br />
        到 <span class="gold">增員推手</span>
      </h2>
      <p>
        主任經典基礎班 × 主任進階班<br />
        邀請你在晉升後的關鍵時刻，打穩增員實戰力。
      </p>

      <div class="cta-buttons">
        <button class="btn btn-primary" onclick="alert('可在這裡串接報名表連結')">
          我要報名課程
        </button>
        <button class="btn btn-secondary" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
          回到課程介紹
        </button>
      </div>
    </section>

    <div class="footer-note">
      主任必修課程｜以 R 線為主軸，打造主任增員實戰力
    </div>

  </div>

  <script>
    const rData = [
      {
        code: "R1",
        title: "取得名單",
        desc: "建立緣故名單、推薦人名單，讓增員不是想到才做，而是有來源、有紀錄、有追蹤。",
        pain: "不知道名單從哪裡來，或名單寫了卻沒有後續動作。",
        course: "緣故名單盤點、推薦人名單建立、增員名單分類。",
        tip: "名單不是等出來的，是整理出來、問出來、累積出來的。"
      },
      {
        code: "R2",
        title: "啟動接觸",
        desc: "透過自然話題、行為模式測驗或活動邀約，開啟與準增的第一步接觸。",
        pain: "怕太像推銷、不知道怎麼開口，或接觸後不知道如何延續。",
        course: "定聯分級、行為模式測驗應用、準增接觸話術。",
        tip: "好的接觸，不是急著說服，而是先讓對方願意聊下去。"
      },
      {
        code: "R3",
        title: "發掘需求",
        desc: "從對方的工作、收入、時間、成長期待中，找出真正重視的工作條件。",
        pain: "聊很多，但沒有問到關鍵；知道對方現況，卻沒有挖出轉換動機。",
        course: "六大面向提問、需求引導、工作價值釐清。",
        tip: "準增不是被說服的，而是被問到自己也開始思考。"
      },
      {
        code: "R4",
        title: "邀約推進",
        desc: "根據準增需求，用合適的理由邀約活動、面談或下一步接觸。",
        pain: "邀約常被「我再想想」「沒時間」「先不用」擋住。",
        course: "FAB 邀約法、活動邀約、下一步推進設計。",
        tip: "邀約不是把人拉來，而是讓對方看見下一步值得了解。"
      },
      {
        code: "R5",
        title: "面談追蹤",
        desc: "在面談後持續追蹤，釐清對方疑慮，協助準增跨過猶豫點。",
        pain: "對方說再看看就停住，不知道該怎麼追、不敢追、追了又怕有壓力。",
        course: "異議問題處理、追蹤節奏、活動量管理。",
        tip: "追蹤不是催促，而是陪對方把問題想清楚。"
      },
      {
        code: "R6",
        title: "新人報聘",
        desc: "協助準增完成報聘前的確認，並銜接新人起步與後續陪跑。",
        pain: "快成交卻鬆掉，或新人進來後缺少明確起步安排。",
        course: "報聘推進、關鍵行動確認、新人起步節奏。",
        tip: "報聘不是結束，而是主任開始帶人的第一步。"
      }
    ];

    function showR(index, button) {
      const item = rData[index];

      document.getElementById("rCode").textContent = item.code;
      document.getElementById("rTitle").textContent = item.title;
      document.getElementById("rDesc").textContent = item.desc;
      document.getElementById("rPain").textContent = item.pain;
      document.getElementById("rCourse").textContent = item.course;
      document.getElementById("rTip").textContent = item.tip;

      const buttons = document.querySelectorAll(".r-btn");
      buttons.forEach(btn => btn.classList.remove("active"));
      button.classList.add("active");
    }

    const answers = {};

    function selectOption(questionIndex, value, button) {
      answers[questionIndex] = value;

      const question = button.parentElement;
      const options = question.querySelectorAll(".option");
      options.forEach(option => option.classList.remove("selected"));

      button.classList.add("selected");
    }

    function showResult() {
      const resultText = document.getElementById("resultText");

      if (Object.keys(answers).length < 3) {
        resultText.textContent = "還差一點點，請先完成三題檢測，才能產出建議方向。";
        return;
      }

      let basic = 0;
      let advance = 0;

      Object.values(answers).forEach(value => {
        if (value === "basic") basic++;
        if (value === "advance") advance++;
      });

      if (basic > advance) {
        resultText.textContent =
          "你目前最需要的是打穩增員起步基本功。建議優先參加「主任經典基礎班」，先把 R1～R2 的名單、接觸、邀約基礎建立起來。";
      } else if (advance > basic) {
        resultText.textContent =
          "你目前已經有行動基礎，但需要更強的推進能力。建議優先參加「主任進階班」，強化 R2～R4 的需求挖掘、FAB 邀約與異議處理。";
      } else {
        resultText.textContent =
          "你適合兩班銜接學習。先用「主任經典基礎班」建立流程，再用「主任進階班」強化需求、邀約與推進，讓增員節奏完整落地。";
      }
    }
  </script>
</body>
</html>
