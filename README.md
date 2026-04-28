
html


<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Рабочий дом | Помощь людям в трудной ситуации</title>
    <meta name="description" content="Помощь людям, попавшим в трудную жизненную ситуацию. Проживание, питание, работа, восстановление документов в Нижнем Новгороде.">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
            color: #1e293b;
            line-height: 1.5;
            scroll-behavior: smooth;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px;
        }

        /* Шапка */
        .header {
            background-color: #ffffff;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
            padding: 16px 0;
        }
        .header-inner {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 16px;
        }
        .logo {
            font-size: 1.6rem;
            font-weight: 700;
            color: #0f3b5c;
            letter-spacing: -0.3px;
        }
        .logo span {
            color: #e67e22;
        }
        .nav a {
            text-decoration: none;
            color: #334155;
            margin-left: 28px;
            font-weight: 500;
            transition: color 0.2s;
        }
        .nav a:hover {
            color: #e67e22;
        }
        .btn-contact {
            background-color: #e67e22;
            color: white !important;
            padding: 8px 20px;
            border-radius: 30px;
        }
        .btn-contact:hover {
            background-color: #d35400;
        }

        /* Герой секция */
        .hero {
            padding: 80px 0 60px;
            background: linear-gradient(135deg, #e8f0f5 0%, #fdf8f0 100%);
        }
        .hero-grid {
            display: flex;
            align-items: center;
            gap: 48px;
            flex-wrap: wrap;
        }
        .hero-content {
            flex: 1;
        }
        .hero-badge {
            background-color: #fee2d6;
            display: inline-block;
            padding: 6px 14px;
            border-radius: 30px;
            font-size: 0.85rem;
            font-weight: 600;
            color: #e67e22;
            margin-bottom: 20px;
        }
        .hero-title {
            font-size: 3rem;
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 20px;
            color: #0b2b3f;
        }
        .hero-title span {
            color: #e67e22;
        }
        .hero-desc {
            font-size: 1.1rem;
            color: #334155;
            margin-bottom: 28px;
            max-width: 500px;
        }
        .hero-stats {
            display: flex;
            gap: 32px;
            margin: 28px 0;
        }
        .stat h3 {
            font-size: 1.8rem;
            font-weight: 700;
            color: #e67e22;
        }
        .stat p {
            color: #475569;
        }
        .hero-image {
            flex: 1;
            background: linear-gradient(135deg, #e67e22, #f39c12);
            border-radius: 32px;
            padding: 40px 20px;
            text-align: center;
            color: white;
            font-weight: 500;
            box-shadow: 0 20px 25px -12px rgba(0,0,0,0.15);
        }
        .hero-image i {
            font-size: 4rem;
            margin-bottom: 15px;
            color: white;
        }
        .hero-image p {
            color: white;
        }
        .hero-image small {
            color: rgba(255,255,255,0.9);
        }

        /* Услуги */
        .services {
            padding: 80px 0;
        }
        .section-title {
            text-align: center;
            font-size: 2.2rem;
            font-weight: 700;
            margin-bottom: 16px;
            color: #0f3b5c;
        }
        .section-sub {
            text-align: center;
            color: #475569;
            max-width: 600px;
            margin: 0 auto 48px;
        }
        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 32px;
        }
        .card {
            background: white;
            border-radius: 24px;
            padding: 32px 24px;
            box-shadow: 0 4px 6px -2px rgba(0,0,0,0.05);
            transition: transform 0.2s ease, box-shadow 0.2s;
            text-align: center;
            border: 1px solid #e2e8f0;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -12px rgba(0,0,0,0.1);
        }
        .card-icon {
            background-color: #fef3e8;
            width: 70px;
            height: 70px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 20px;
            margin: 0 auto 24px;
        }
        .card-icon i {
            font-size: 32px;
            color: #e67e22;
        }
        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 12px;
        }
        .card p {
            color: #475569;
        }

        /* О нас */
        .about {
            background-color: #ffffff;
            padding: 70px 0;
            border-top: 1px solid #e2e8f0;
            border-bottom: 1px solid #e2e8f0;
        }
        .about-grid {
            display: flex;
            gap: 48px;
            align-items: center;
            flex-wrap: wrap;
        }
        .about-text {
            flex: 1;
        }
        .about-text h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #0f3b5c;
        }
        .about-text p {
            margin-bottom: 20px;
            color: #334155;
        }
        .about-feature {
            display: flex;
            gap: 16px;
            margin-top: 24px;
            align-items: center;
        }
        .about-feature i {
            color: #e67e22;
            font-size: 1.4rem;
        }

        /* Контакты + форма */
        .contact {
            padding: 80px 0;
            background-color: #fef9f4;
        }
        .contact-grid {
            display: flex;
            gap: 48px;
            flex-wrap: wrap;
        }
        .contact-info {
            flex: 1;
        }
        .contact-item {
            display: flex;
            align-items: center;
            gap: 16px;
            margin-bottom: 30px;
        }
        .contact-icon {
            width: 50px;
            height: 50px;
            background: #fef3e8;
            border-radius: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .contact-icon i {
            font-size: 1.4rem;
            color: #e67e22;
        }
        .contact-form {
            flex: 1;
            background: white;
            padding: 36px;
            border-radius: 28px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.05);
            border: 1px solid #e2e8f0;
        }
        .form-group {
            margin-bottom: 20px;
        }
        input, textarea {
            width: 100%;
            padding: 14px 18px;
            border: 1px solid #cbd5e1;
            border-radius: 16px;
            font-family: inherit;
            font-size: 1rem;
            transition: 0.2s;
        }
        input:focus, textarea:focus {
            outline: none;
            border-color: #e67e22;
            box-shadow: 0 0 0 3px rgba(230,126,34,0.1);
        }
        button {
            background-color: #e67e22;
            color: white;
            border: none;
            padding: 14px 28px;
            font-size: 1rem;
            font-weight: 600;
            border-radius: 40px;
            cursor: pointer;
            transition: background 0.2s;
            width: 100%;
        }
        button:hover {
            background-color: #d35400;
        }
        .footer {
            background-color: #0f172a;
            color: #94a3b8;
            text-align: center;
            padding: 32px 0;
            margin-top: 40px;
        }
        .footer a {
            color: #e67e22;
            text-decoration: none;
        }

        @media (max-width: 768px) {
            .hero-title {
                font-size: 2.2rem;
            }
            .nav a {
                margin-left: 12px;
                font-size: 0.9rem;
            }
            .header-inner {
                flex-direction: column;
            }
            .section-title {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>

<header class="header">
    <div class="container">
        <div class="header-inner">
            <div class="logo">Рабочий<span>Дом</span></div>
            <div class="nav">
                <a href="#home">Главная</a>
                <a href="#services">Услуги</a>
                <a href="#about">О нас</a>
                <a href="#contact" class="btn-contact">Связаться</a>
            </div>
        </div>
    </div>
</header>

<main>
    <!-- Hero / Главный экран -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-grid">
                <div class="hero-content">
                    <div class="hero-badge">Помощь здесь и сейчас</div>
                    <h1 class="hero-title">Рабочий дом — <span>помощь людям</span> в трудной жизненной ситуации</h1>
                    <p class="hero-desc">Мы верим, что каждый заслуживает второй шанс. Проживание, питание, работа и восстановление документов — всё, чтобы начать новую жизнь.</p>
                    <div class="hero-stats">
                        <div class="stat">
                            <h3>24/7</h3>
                            <p>Поддержка</p>
                        </div>
                        <div class="stat">
                            <h3>Бесплатно</h3>
                            <p>Проживание</p>
                        </div>
                        <div class="stat">
                            <h3>Срочно</h3>
                            <p>Помощь</p>
                        </div>
                    </div>
                </div>
                <div class="hero-image">
                    <i class="fas fa-hands-helping"></i>
                    <p>Мы рядом в трудную минуту</p>
                    <small>Работа с ежедневными выплатами</small>
                </div>
            </div>
        </div>
    </section>

    <!-- Услуги -->
    <section id="services" class="services">
        <div class="container">
            <h2 class="section-title">Что мы предлагаем</h2>
            <div class="section-sub">Полный комплекс помощи для восстановления в обществе</div>
            <div class="cards">
                <div class="card">
                    <div class="card-icon"><i class="fas fa-utensils"></i></div>
                    <h3>Бесплатное питание</h3>
                    <p>4-х разовое полноценное питание</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fas fa-briefcase"></i></div>
                    <h3>Работа</h3>
                    <p>Ежедневные выплаты</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fas fa-home"></i></div>
                    <h3>Проживание</h3>
                    <p>В социальных квартирах и городах по месту обращения</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fas fa-id-card"></i></div>
                    <h3>Восстановление документов</h3>
                    <p>Паспорт, СНИЛС, ИНН — всё по мере необходимости</p>
                </div>
            </div>
        </div>
    </section>

    <!-- О компании -->
    <section id="about" class="about">
        <div class="container">
            <div class="about-grid">
                <div class="about-text">
                    <h2>О проекте «Рабочий дом»</h2>
                    <p>Мы специализируемся на предоставлении необходимой помощи для восстановления в обществе. Каждый может столкнуться с трудностями – потеря работы, жилья, документов.</p>
                    <p>Наша миссия — помочь вернуться к нормальной жизни, сохраняя человеческое достоинство. Ценные вещи, документы и связь не изымаются.</p>
                    <div class="about-feature">
                        <i class="fas fa-check-circle"></i>
                        <span>Гарантия предоставления всех указанных условий</span>
                    </div>
                    <div class="about-feature">
                        <i class="fas fa-check-circle"></i>
                        <span>Для целеустремлённых — карьерный рост и обучение</span>
                    </div>
                    <div class="about-feature">
                        <i class="fas fa-check-circle"></i>
                        <span>Полная конфиденциальность и уважение</span>
                    </div>
                </div>
                <div class="hero-image" style="padding:30px;">
                    <i class="fas fa-shield-alt" style="font-size: 3rem;"></i>
                    <p>Документы, сотовая связь, ценные личные вещи не изымаются</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Контакты и форма -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Свяжитесь с нами</h2>
            <div class="section-sub">Напишите — мы обязательно поможем</div>
            <div class="contact-grid">
                <div class="contact-info">
                    <div class="contact-item">
                        <div class="contact-icon"><i class="fas fa-phone-alt"></i></div>
                        <div>
                            <h4>Телефон (круглосуточно)</h4>
                            <p>+7 (927) 046-24-24</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon"><i class="fas fa-envelope"></i></div>
                        <div>
                            <h4>Email</h4>
                            <p>help@workinghouse.ru</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon"><i class="fas fa-map-marker-alt"></i></div>
                        <div>
                            <h4>Нижний Новгород</h4>
                            <p>ул. Московское шоссе, 77</p>
                        </div>
                    </div>
                </div>
                <div class="contact-form">
                    <form action="#" method="post">
                        <div class="form-group">
                            <input type="text" placeholder="Ваше имя" required>
                        </div>
                        <div class="form-group">
                            <input type="tel" placeholder="Номер телефона" required>
                        </div>
                        <div class="form-group">
                            <textarea rows="4" placeholder="Опишите вашу ситуацию (какая нужна помощь)"></textarea>
                        </div>
                        <button type="submit">Отправить заявку <i class="fas fa-arrow-right"></i></button>
                        <p style="font-size: 0.75rem; margin-top: 15px; text-align: center;">Нажимая на кнопку, вы соглашаетесь на обработку данных</p>
                    </form>
                </div>
            </div>
        </div>
    </section>
</main>

<footer class="footer">
    <div class="container">
        <p>© 2026 Рабочий дом — помощь людям в трудной жизненной ситуации</p>
        <p style="margin-top: 10px; font-size: 0.8rem;">Каждый заслуживает второй шанс</p>
    </div>
</footer>

<!-- Обработчик формы -->
<script>
    const form = document.querySelector('form');
    if (form) {
        form.addEventListener('submit', (e) => {
            e.preventDefault();
            alert('Спасибо! Ваша заявка принята. Мы свяжемся с вами в ближайшее время.');
            form.reset();
        });
    }
</script>
</body>
</html>
