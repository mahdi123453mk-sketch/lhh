# lhh[index (5).html](https://github.com/user-attachments/files/23286227/index.5.html)
<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>اختبار الكيمياء — طبقة الأوزون والمفاهيم العامة</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <main id="app">
    <!-- شاشة الترحيب -->
    <section id="welcome" class="card">
      <h1>اختبار الكيمياء (اختيار من متعدد)</h1>
      <p class="meta">الأسئلة: <span id="totalQuestions">40</span> — مدة الاختبار: <strong>50:00</strong></p>

      <label>اسم الطالب:
        <input id="studentName" type="text" placeholder="ادخل اسمك" />
      </label>

      <label>اختر الشعبة:
        <select id="sectionSelect">
          <option value="">-- اختر الشعبة --</option>
          <option value="1">الشعبة 1</option>
          <option value="2">الشعبة 2</option>
          <option value="3">الشعبة 3</option>
          <option value="4">الشعبة 4</option>
          <option value="5">الشعبة 5</option>
          <option value="6">الشعبة 6</option>
          <option value="7">الشعبة 7</option>
        </select>
      </label>

      <div class="small">عند اختيار الشعبة ستتحول خلفية الصفحة إلى أزرق.</div>

      <div class="actions">
        <button id="startBtn" class="primary">ابدأ الاختبار</button>
      </div>

      <div class="credits-foot">الوقت الافتراضي 50 دقيقة. بعدها يتم إنهاء الاختبار تلقائياً.</div>
    </section>

    <!-- شاشة العد التنازلي قبل البدء -->
    <section id="preStart" class="card hidden">
      <h2>الاختبار سيبدأ بعد</h2>
      <div id="preCountdown" class="big">3</div>
      <div class="small">استعد وكن جاهزًا</div>
    </section>

    <!-- شاشة الأسئلة -->
    <section id="quiz" class="card hidden">
      <header class="quiz-header">
        <div>الطالب: <span id="displayName"></span></div>
        <div>الشعبة: <span id="displaySection"></span></div>
        <div>الوقت المتبقي: <span id="timer">50:00</span></div>
        <div>السؤال <span id="currentIndex">1</span> من <span id="qCount">40</span></div>
      </header>

      <div id="questionArea" class="question-area">
        <h3 id="questionText">نص السؤال...</h3>
        <div id="options" class="options"></div>
      </div>

      <div id="feedback" class="feedback hidden"></div>
    </section>

    <!-- شاشة النتيجة النهائية -->
    <section id="result" class="card hidden">
      <h2>النتيجة النهائية</h2>
      <div class="score">
        <div>درجتك: <strong id="scorePercent">0%</strong></div>
        <div id="scoreLevel" class="level"></div>
      </div>

      <h3>تفاصيل الأسئلة والإجابات</h3>
      <div id="review" class="review"></div>

      <h3>طاقم العمل الرئيس</h3>
      <div class="team">
        مهدي البطاط (الرئيس) — مبارك الشهراني — صالح المحيبس — سامي الشمري — عماد الرشود — عبدالله الدوسري
      </div>

      <div class="actions">
        <button id="restartBtn">إعادة الاختبار</button>
      </div>
    </section>
  </main>

  <script src="script.js"></script>
</body>
</html>
