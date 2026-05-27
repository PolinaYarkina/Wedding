<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes, viewport-fit=cover">
  <title>Свадьба Полины и Димы • 06 августа 2026</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;1,400;1,600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Montserrat', sans-serif;
      background: #fdf7f2;
      color: #4a3b32;
      line-height: 1.6;
      overflow-x: hidden;
      scroll-behavior: smooth;
    }
    .petals-bg {
      position: fixed; top: 0; left: 0; width: 100%; height: 100%;
      pointer-events: none; z-index: 1; overflow: hidden;
    }
    .petal {
      position: absolute;
      background: radial-gradient(circle at 30% 30%, #f9d8c6, #f7c5b5);
      width: 25px; height: 25px;
      border-radius: 100% 0 100% 0;
      transform: rotate(45deg); opacity: 0.5;
      animation: fall linear infinite;
      box-shadow: 0 10px 20px rgba(0,0,0,0.03);
    }
    @keyframes fall {
      0% { transform: translateY(-10vh) rotate(0deg); opacity: 0.6; }
      80% { opacity: 0.5; }
      100% { transform: translateY(110vh) rotate(360deg); opacity: 0; }
    }
    .site-container {
      position: relative; z-index: 10;
      max-width: 900px; margin: 0 auto; padding: 2rem 1.5rem 4rem;
    }
    section {
      background: #fffaf5;
      border-radius: 2.5rem;
      padding: 2.8rem 2rem;
      margin-bottom: 2.5rem;
      box-shadow: 0 25px 45px -12px rgba(0,0,0,0.08), 0 8px 18px rgba(0,0,0,0.03);
      border: 1px solid rgba(232, 203, 182, 0.4);
      text-align: center;
      transition: transform 0.2s;
    }
    section:hover {
      transform: translateY(-3px);
      box-shadow: 0 30px 55px -15px rgba(0,0,0,0.1);
    }
    h1, h2 { font-family: 'Cormorant Garamond', serif; font-weight: 500; }
    h1 {
      font-size: clamp(3.2rem, 10vw, 5rem);
      color: #b48c6c; margin-bottom: 0.5rem;
      font-weight: 600; font-style: italic;
    }
    .ampersand { font-size: 3.5rem; color: #d9b99b; font-family: 'Cormorant Garamond', serif; font-style: italic; }
    .date-main { font-size: 1.8rem; color: #7f6b5c; margin: 1rem 0 0.3rem; letter-spacing: 2px; }
    .sub-text { font-size: 1.1rem; color: #9b897b; text-transform: uppercase; letter-spacing: 3px; margin-bottom: 1.5rem; }
    .decor-line {
      width: 90px; height: 2px; background: #e5cfbc;
      margin: 1.5rem auto; position: relative;
    }
    .decor-line::before {
      content: "♥";
      position: absolute; top: -13px; left: 50%;
      transform: translateX(-50%);
      background: #fffaf5; padding: 0 12px;
      color: #dbb094; font-size: 1.2rem;
    }
    .details-grid {
      display: flex; flex-wrap: wrap; justify-content: center;
      gap: 2.5rem; margin-top: 1.8rem;
    }
    .detail-item { display: flex; flex-direction: column; align-items: center; gap: 0.6rem; }
    .detail-icon {
      font-size: 2.2rem; background: #f9ede3;
      width: 65px; height: 65px;
      display: flex; align-items: center; justify-content: center;
      border-radius: 50%; color: #b48c6c;
    }
    .detail-title { font-weight: 500; font-size: 0.9rem; text-transform: uppercase; letter-spacing: 2px; color: #9b897b; }
    .detail-desc { font-family: 'Cormorant Garamond', serif; font-size: 1.5rem; font-weight: 500; color: #4a3b32; }
    .timing-list { list-style: none; margin: 1.8rem 0 1rem; }
    .timing-list li {
      display: flex; justify-content: space-between; align-items: baseline;
      padding: 1rem 0; border-bottom: 1px dashed #e8cfbc; font-size: 1.1rem;
    }
    .timing-list li:last-child { border-bottom: none; }
    .time-badge {
      background: #f7e2d4; color: #6b4f3c;
      padding: 0.2rem 1rem; border-radius: 30px;
      font-weight: 500; font-size: 0.9rem; letter-spacing: 1px;
    }
    .rsvp-form {
      display: flex; flex-direction: column; gap: 1.2rem;
      max-width: 500px; margin: 1.5rem auto 0; text-align: left;
    }
    .form-row { display: flex; flex-wrap: wrap; gap: 1rem; }
    .form-group { flex: 1 1 200px; display: flex; flex-direction: column; gap: 0.3rem; }
    label { font-size: 0.8rem; text-transform: uppercase; letter-spacing: 1.5px; font-weight: 500; color: #7f6b5c; }
    input, select, textarea {
      background: #fffdf9; border: 1px solid #e7d3c0;
      border-radius: 30px; padding: 0.9rem 1.4rem;
      font-family: 'Montserrat', sans-serif; font-size: 0.95rem;
      outline: none; transition: 0.2s; resize: vertical;
    }
    input:focus, select:focus, textarea:focus {
      border-color: #c9a78b;
      box-shadow: 0 0 0 3px rgba(201, 167, 139, 0.15);
    }
    .btn {
      background: linear-gradient(135deg, #cfb197, #b58b6b);
      border: none; color: white;
      padding: 1rem 2.2rem; border-radius: 40px;
      font-weight: 500; letter-spacing: 2px; text-transform: uppercase;
      font-size: 0.9rem; cursor: pointer;
      box-shadow: 0 8px 18px rgba(181, 139, 107, 0.3);
      transition: all 0.25s; margin-top: 0.5rem;
    }
    .btn:hover {
      background: linear-gradient(135deg, #dbbc9b, #c49a7a);
      box-shadow: 0 12px 24px rgba(181, 139, 107, 0.4);
      transform: translateY(-2px);
    }
    .success-message {
      background: #e2f0da; color: #4a6741;
      border-radius: 2rem; padding: 2rem; margin-top: 2rem;
      font-size: 1.1rem; font-weight: 500;
      display: none;
    }
    .success-message.visible { display: block; }
    .error-message {
      color: #b15e5e; margin-top: 1rem; font-weight: 500;
    }
    @media (max-width: 500px) {
      section { padding: 2rem 1.2rem; }
    }
  </style>
</head>
<body>
<div class="petals-bg" id="petalsContainer"></div>

<div class="site-container">
  
  <section>
    <h1>Полина & Дима</h1>
    <div class="decor-line"></div>
    <p class="date-main">06 • 08 • 2026</p>
    <p class="sub-text">Мы женимся!</p>
    <p style="margin-top: 1rem; font-style: italic; color: #8b7768;">Дорогие гости, приглашаем разделить с нами этот особенный день.</p>
  </section>

  <section>
    <h2 style="font-size: 2.4rem; color: #b48c6c;">Когда и где</h2>
    <div class="decor-line"></div>
    <div class="details-grid">
      <div class="detail-item">
        <div class="detail-icon">📅</div>
        <span class="detail-title">Дата</span>
        <span class="detail-desc">06 августа 2026</span>
        <span>Четверг</span>
      </div>
      <div class="detail-item">
        <div class="detail-icon">📍</div>
        <span class="detail-title">Место</span>
        <span class="detail-desc">Волгоградская область</span>
        <span>Светлоярский район, село Райгород</span>
      </div>
      <div class="detail-item">
        <div class="detail-icon">🕊️</div>
        <span class="detail-title">Сбор гостей</span>
        <span class="detail-desc">15:30</span>
      </div>
    </div>
    <p style="margin-top: 1.5rem; background: #fdf3ea; padding: 0.8rem; border-radius: 30px; font-size: 0.95rem;">
      Точный адрес и схема проезда придут вместе с подтверждением.
    </p>
  </section>

  <section>
    <h2 style="font-size: 2.4rem; color: #b48c6c;">Расписание</h2>
    <div class="decor-line"></div>
    <ul class="timing-list">
      <li><span>🌸 Сбор гостей</span> <span class="time-badge">15:30</span></li>
      <li><span>💍 Церемония</span> <span class="time-badge">16:15</span></li>
      <li><span>🥂 Фуршет и фото</span> <span class="time-badge">17:00</span></li>
      <li><span>🍽️ Свадебный ужин</span> <span class="time-badge">18:30</span></li>
      <li><span>🎂 Торт и сюрпризы</span> <span class="time-badge">21:00</span></li>
      <li><span>🎶 Танцы</span> <span class="time-badge">22:00</span></li>
    </ul>
  </section>

  <section id="rsvp">
    <h2 style="font-size: 2.4rem; color: #b48c6c;">Подтвердите присутствие</h2>
    <div class="decor-line"></div>
    <p>Пожалуйста, ответьте <strong>до 1 августа 2026</strong></p>

    <form class="rsvp-form" id="rsvpForm" 
      action="https://formspree.io/f/mdajydrw" 
      method="POST">
  <!-- Скрытое поле для возврата на сайт после отправки -->
  <input type="hidden" name="_next" value="https://polina-dima-wedding.netlify.app/?sent=yes">
  <input type="hidden" name="_subject" value="Подтверждение – Свадьба Полины и Димы">

  <div class="form-row">
    <div class="form-group">
      <label>Имя и фамилия *</label>
      <input type="text" name="Имя" placeholder="Анна Смирнова" required>
    </div>
    <div class="form-group">
      <label>Email (необязательно)</label>
      <input type="email" name="Email" placeholder="для связи">
    </div>
  </div>
  <div class="form-group">
    <label>Я буду *</label>
    <select name="Присутствие" required>
      <option value="" disabled selected>Выберите вариант</option>
      <option value="Обязательно буду">Обязательно буду!</option>
      <option value="Постараюсь">Постараюсь, уточню позже</option>
      <option value="Не смогу">К сожалению, не смогу</option>
    </select>
  </div>
  <div class="form-group">
    <label>Пожелания / аллергии</label>
    <textarea name="Пожелания" rows="2" placeholder="Если есть особые пожелания..."></textarea>
  </div>
  <button type="submit" class="btn">Отправить</button>
</form>

    <div id="successBlock" class="success-message">
      💌 Спасибо! Ваш ответ уже у Полины и Димы. <br>До встречи на свадьбе!
    </div>
    <div id="errorBlock" class="error-message" style="display:none;"></div>
  </section>

  <section>
    <h2 style="font-size: 2.4rem; color: #b48c6c;">С любовью</h2>
    <div class="decor-line"></div>
    <p style="font-size: 1.4rem; font-family: 'Cormorant Garamond', serif;">Полина & Дима</p>
  </section>
</div>

<script>
  (function() {
    // Падающие лепестки
    const petalsContainer = document.getElementById('petalsContainer');
    for (let i = 0; i < 24; i++) {
      const petal = document.createElement('div');
      petal.classList.add('petal');
      const size = Math.floor(Math.random() * 22 + 14);
      petal.style.width = size + 'px';
      petal.style.height = size + 'px';
      petal.style.left = Math.random() * 100 + '%';
      petal.style.animationDelay = Math.random() * 18 + 's';
      petal.style.animationDuration = Math.random() * 14 + 14 + 's';
      petal.style.opacity = Math.random() * 0.4 + 0.25;
      petalsContainer.appendChild(petal);
    }

    // Обработка формы через AJAX (без перезагрузки)
    const form = document.getElementById('rsvpForm');
    const successDiv = document.getElementById('successBlock');
    const errorDiv = document.getElementById('errorBlock');
    const submitBtn = document.getElementById('submitBtn');

    form.addEventListener('submit', async (e) => {
      e.preventDefault(); // Отменяем стандартную отправку

      // Скрываем предыдущие сообщения
      successDiv.classList.remove('visible');
      errorDiv.style.display = 'none';

      // Меняем кнопку на время отправки
      submitBtn.disabled = true;
      submitBtn.textContent = 'Отправляю...';

      // Собираем данные формы
      const formData = new FormData(form);
      // Добавляем скрытые поля, которые были в старом варианте
      formData.append('_subject', 'Новое подтверждение – Свадьба Полины и Димы');
      formData.append('_captcha', 'false');
      formData.append('_template', 'table');
      // _next не нужен при AJAX

      try {
        const response = await fetch('https://formsubmit.co/ajax/polinayarkina12@gmail.com', {
          method: 'POST',
          body: formData
        });

        const result = await response.json();

        if (response.ok && result.success) {
          // Успех
          successDiv.classList.add('visible');
          form.reset(); // Очищаем поля
          // Прокручиваем к сообщению
          successDiv.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
        } else {
          throw new Error(result.message || 'Ошибка при отправке');
        }
      } catch (error) {
        console.error('Ошибка отправки:', error);
        errorDiv.style.display = 'block';
        errorDiv.textContent = '⚠️ Что-то пошло не так. Проверьте соединение или повторите попытку позже.';
        errorDiv.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
      } finally {
        // Возвращаем кнопку
        submitBtn.disabled = false;
        submitBtn.textContent = 'Отправить';
      }
    });
  })();
</script>
</body>
</html>
