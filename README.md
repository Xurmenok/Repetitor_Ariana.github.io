# Repetitor_Ariana.github.io
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Репетитор по математике Ариан | Профессиональная подготовка</title>
    <style>
        /* Базовые стили */
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: #f9f9f9;
        }
        
        h1, h2, h3 {
            margin-bottom: 1rem;
            color: var(--primary-color);
        }
        
        p {
            margin-bottom: 1rem;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Шапка и навигация */
        header {
            background-color: var(--primary-color);
            color: white;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: var(--shadow);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: white;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav li {
            margin-left: 1.5rem;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: var(--secondary-color);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* Основные секции */
        section {
            padding: 5rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 0.5rem auto;
        }
        
        /* Главная секция */
        .hero {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            text-align: center;
            padding: 8rem 0 5rem;
            margin-top: 60px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: white;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent-color);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: #c0392b;
        }
        
        /* Обо мне */
        .about-container {
            display: flex;
            align-items: center;
            gap: 3rem;
        }
        
        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .about-text {
            flex: 1;
        }
        
        /* Услуги */
        .services {
            background-color: var(--light-color);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .service-card {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: var(--shadow);
            text-align: center;
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
        }
        
        .service-icon {
            width: 80px;
            height: 80px;
            margin: 0 auto 1rem;
            background-color: var(--light-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .service-icon svg {
            width: 40px;
            height: 40px;
            fill: var(--secondary-color);
        }
        
        /* Отзывы */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
        }
        
        .gallery-item {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: transform 0.3s;
        }
        
        .gallery-item:hover {
            transform: scale(1.03);
        }
        
        .gallery-item img {
            width: 100%;
            height: 350px;
            object-fit: cover;
            display: block;
        }
        
        /* Контакты */
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 3rem;
        }
        
        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
        
        .contact-icon {
            width: 50px;
            height: 50px;
            background-color: var(--light-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .contact-icon svg {
            width: 24px;
            height: 24px;
            fill: var(--secondary-color);
        }
        
        .contact-link {
            color: var(--text-color);
            text-decoration: none;
        }
        
        .contact-link:hover {
            color: var(--secondary-color);
        }
        
        /* Форма */
        .contact-form {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: var(--shadow);
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
        }
        
        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }
        
        .error {
            color: var(--accent-color);
            font-size: 0.9rem;
            margin-top: 0.3rem;
            display: none;
        }
        
        /* Футер */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 3rem 0 1.5rem;
        }
        
        .footer-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 2rem;
        }
        
        .social-links {
            display: flex;
            gap: 1.5rem;
        }
        
        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: background-color 0.3s;
        }
        
        .social-link:hover {
            background-color: var(--secondary-color);
        }
        
        .social-link svg {
            width: 20px;
            height: 20px;
            fill: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 1.5rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            width: 100%;
        }
        
        /* Адаптивность */
        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: block;
            }
            
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: var(--primary-color);
                flex-direction: column;
                padding: 1rem 0;
                box-shadow: var(--shadow);
            }
            
            nav ul.active {
                display: flex;
            }
            
            nav li {
                margin: 0;
                text-align: center;
            }
            
            nav a {
                display: block;
                padding: 0.8rem 1rem;
            }
            
            .about-container {
                flex-direction: column;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            section {
                padding: 3rem 0;
            }
        }
    </style>
</head>
<body>
    <!-- Шапка с навигацией -->
    <header>
        <div class="container header-container">
            <div class="logo">Ариан | Репетитор по математике</div>
            <button class="mobile-menu-btn">☰</button>
            <nav>
                <ul>
                    <li><a href="#home">Главная</a></li>
                    <li><a href="#about">Обо мне</a></li>
                    <li><a href="#services">Услуги</a></li>
                    <li><a href="#gallery">Отзывы</a></li>
                    <li><a href="#contacts">Контакты</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Главная секция -->
    <section id="home" class="hero">
        <div class="container">
            <h1>Профессиональный репетитор по математике</h1>
            <p>Помогаю школьникам и студентам понять математику, повысить успеваемость и подготовиться к экзаменам. Индивидуальный подход к каждому ученику.</p>
            <a href="#contacts" class="btn">Записаться на занятие</a>
        </div>
    </section>

    <!-- Обо мне -->
    <section id="about">
        <div class="container">
            <h2 class="section-title">Обо мне</h2>
            <div class="about-container">
                <div class="about-image">
                    <!-- Оригинальное фото репетитора -->
                    <img src="https://sun9-16.userapi.com/s/v1/ig2/GIQ7G-K--sMfU0oUbJZJGu7xuOsw_OqJ6hXD4tUXlNOTFLs-uqXQpJEdeI51KPpPdLiLvcXUBGlSmSLGoHfuMH0j.jpg?quality=95&as=32x43,48x64,72x96,108x144,160x213,240x320,360x480,480x640,540x720,640x853,720x960,1080x1440,1280x1707,1440x1920,1920x2560&from=bu&cs=1920x0" alt="Ариана - репетитор по математике">
                </div>
                <div class="about-text">
                    <p>Меня зовут Ариана, и я профессиональный репетитор по математике с 8-летним опытом работы. Я закончил механико-математический факультет МГУ с красным дипломом и с тех пор помогаю ученикам разных возрастов понять и полюбить математику.</p>
                    <p>Мой подход основан на индивидуальной работе с каждым учеником. Я считаю, что не бывает "неспособных" к математике людей - бывают неправильные методы объяснения. Моя задача - найти подход именно к вам или вашему ребенку.</p>
                    <p>За годы работы я подготовил более 100 учеников к ОГЭ и ЕГЭ, при этом средний балл моих подопечных составляет 85+. Многие из моих бывших учеников сейчас успешно учатся в ведущих технических вузах страны.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Услуги -->
    <section id="services" class="services">
        <div class="container">
            <h2 class="section-title">Мои услуги</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,16.5L18,9.5L16.59,8.09L11,13.67L7.91,10.59L6.5,12L11,16.5Z" />
                        </svg>
                    </div>
                    <h3>Подготовка к ОГЭ</h3>
                    <p>Системная подготовка к основному государственному экзамену по математике для учащихся 9 классов. Разбор всех типов задач, работа над пробелами в знаниях.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,16.5L18,9.5L16.59,8.09L11,13.67L7.91,10.59L6.5,12L11,16.5Z" />
                        </svg>
                    </div>
                    <h3>Подготовка к ЕГЭ</h3>
                    <p>Углубленная подготовка к единому государственному экзамену по математике (профильный уровень). Особое внимание сложным задачам второй части.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24">
                            <path d="M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,16.5L18,9.5L16.59,8.09L11,13.67L7.91,10.59L6.5,12L11,16.5Z" />
                        </svg>
                    </div>
                    <h3>Повышение успеваемости</h3>
                    <p>Помощь школьникам 5-11 классов в усвоении школьной программы, выполнении домашних заданий, подготовке к контрольным работам.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Отзывы -->
    <section id="otzavs">
        <div class="container">
            <h2 class="section-title">Отзывы</h2>
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="https://s3.iimg.su/s/16/th_gUmc6UGxYPpyBD6FJIinWAcWgnKF28EOn5d33yPL.png" alt="Отзыв_1">
                </div>
                <div class="gallery-item">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZTVlOGVmIi8+CiAgPHBvbHlnb24gcG9pbnRzPSIxMDAsMjUwIDIwMCwxMDAgMzAwLDI1MCIgZmlsbD0iI2ZmZiIgc3Ryb2tlPSIjMzQ5OGRiIiBzdHJva2Utd2lkdGg9IjIiLz4KICA8dGV4dCB4PSIyMDAiIHk9IjE3MCIgZm9udC1mYW1pbHk9IkFyaWFsIiBmb250LXNpemU9IjI0IiBmaWxsPSIjMzQ5OGRiIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIj5HZW9tZXRyaWE8L3RleHQ+Cjwvc3ZnPg==" alt="Геометрические фигуры">
                </div>
                <div class="gallery-item">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZTVlOGVmIi8+CiAgPHBhdGggZD0iTTEwMCAxNTAgTDE1MCAxMDAgTDIwMCAxNTAgTDI1MCAxMDAgTDMwMCAxNTAiIHN0cm9rZT0iIzM0OThkYiIgc3Ryb2tlLXdpZHRoPSIyIiBmaWxsPSJub25lIi8+CiAgPHRleHQgeD0iMjAwIiB5PSIyMDAiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSIyNCIgZmlsbD0iIzM0OThkYiIgdGV4dC1hbmNob3I9Im1pZGRsZSI+RnVuY3Rpb25zPC90ZXh0Pgo8L3N2Zz4=" alt="Графики функций">
                </div>
                <div class="gallery-item">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZTVlOGVmIi8+CiAgPGNpcmNsZSBjeD0iMTUwIiBjeT0iMTUwIiByPSI3MCIgZmlsbD0iI2ZmZiIgc3Ryb2tlPSIjMzQ5OGRiIiBzdHJva2Utd2lkdGg9IjIiLz4KICA8Y2lyY2xlIGN4PSIyNTAiIGN5PSIxNTAiIHI9IjcwIiBmaWxsPSIjZmZmIiBzdHJva2U9IiMzNDk4ZGIiIHN0cm9rZS13aWR0aD0iMiIvPgogIDx0ZXh0IHg9IjIwMCIgeT0iMjUwIiBmb250LWZhbWlseT0iQXJpYWwiIGZvbnQtc2l6ZT0iMjQiIGZpbGw9IiMzNDk4ZGIiIHRleHQtYW5jaG9yPSJtaWRkbGUiPlNldCBUaGVvcnk8L3RleHQ+Cjwvc3ZnPg==" alt="Теория множеств">
                </div>
            </div>
        </div>
    </section>

    <!-- Контакты -->
    <section id="contacts">
        <div class="container">
            <h2 class="section-title">Контакты</h2>
            <div class="contact-container">
                <div class="contact-info">
                    <div class="contact-item">
                        <div class="contact-icon">
                            <svg viewBox="0 0 24 24">
                                <path d="M6.62,10.79C8.06,13.62 10.38,15.94 13.21,17.38L15.41,15.18C15.69,14.9 16.08,14.82 16.43,14.93C17.55,15.3 18.75,15.5 20,15.5A1,1 0 0,1 21,16.5V20A1,1 0 0,1 20,21A17,17 0 0,1 3,4A1,1 0 0,1 4,3H7.5A1,1 0 0,1 8.5,4C8.5,5.25 8.7,6.45 9.07,7.57C9.18,7.92 9.1,8.31 8.82,8.59L6.62,10.79Z" />
                            </svg>
                        </div>
                        <div>
                            <h3>Телефон</h3>
                            <a href="tel:+79991234567" class="contact-link">+7 (999) 999-99-99</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <svg viewBox="0 0 24 24">
                                <path d="M20,8L12,13L4,8V6L12,11L20,6M20,4H4C2.89,4 2,4.89 2,6V18A2,2 0 0,0 4,20H20A2,2 0 0,0 22,18V6C22,4.89 21.1,4 20,4Z" />
                            </svg>
                        </div>
                        <div>
                            <h3>Email</h3>
                            <a href="mailto:arian.math@tutor.ru" class="contact-link">arianka_balbeska@gmail.com</a>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <svg viewBox="0 0 24 24">
                                <path d="M12,11.5A2.5,2.5 0 0,1 9.5,9A2.5,2.5 0 0,1 12,6.5A2.5,2.5 0 0,1 14.5,9A2.5,2.5 0 0,1 12,11.5M12,2A7,7 0 0,0 5,9C5,14.25 12,22 12,22C12,22 19,14.25 19,9A7,7 0 0,0 12,2Z" />
                            </svg>
                        </div>
                        <div>
                            <h3>Адрес</h3>
                            <p>г. Санкт-Петербург</p>
                        </div>
                    </div>
                </div>
                <div class="contact-form">
                    <form id="feedback-form">
                        <div class="form-group">
                            <label for="name">Ваше имя</label>
                            <input type="text" id="name" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" class="form-control" required>
                            <div class="error" id="email-error">Пожалуйста, введите корректный email</div>
                        </div>
                        <div class="form-group">
                            <label for="message">Сообщение</label>
                            <textarea id="message" class="form-control" required></textarea>
                        </div>
                        <button type="submit" class="btn">Отправить сообщение</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Футер -->
    <footer>
        <div class="container footer-container">
            <div class="social-links">
                <a href="#" class="social-link">
                    <svg viewBox="0 0 24 24">
                        <path d="M15.07 2H8.93C4.06 2 2 4.06 2 8.93V15.07C2 19.94 4.06 22 8.93 22H15.07C19.94 22 22 19.94 22 15.07V8.93C22 4.06 19.94 2 15.07 2M18.15 16.27H16.69C16.14 16.27 15.97 15.82 15 14.83C14.12 14 13.74 13.88 13.53 13.88C13.24 13.88 13.15 13.96 13.15 14.38V15.69C13.15 16.04 13.04 16.26 12.11 16.26C10.57 16.26 8.86 15.32 7.66 13.59C5.85 11.05 5.36 9.13 5.36 8.75C5.36 8.54 5.43 8.34 5.66 8.34H7.12C7.47 8.34 7.57 8.5 7.69 8.9C8.35 10.55 9.46 12.1 10.07 12.1C10.2 12.1 10.27 12.04 10.27 11.63V9.64C10.27 9.24 10.13 9.12 9.83 9.05C9.58 9 9.42 8.95 9.42 8.68C9.42 8.5 9.58 8.32 9.78 8.32H12.73C13.04 8.32 13.19 8.5 13.19 8.81V11.66C13.19 12.06 13.3 12.13 13.5 12.13C13.7 12.13 14.04 12.03 14.55 11.55C15.27 10.84 15.94 9.71 16.3 8.91C16.43 8.59 16.56 8.35 16.85 8.35H18.29C18.5 8.35 18.61 8.53 18.5 8.84C18.25 9.57 16.95 11.69 16.75 11.97C16.5 12.3 16.38 12.4 16.38 12.63C16.38 12.78 16.5 12.95 16.75 13.2C17.44 13.89 18.02 14.56 18.29 15.21C18.43 15.55 18.32 15.73 18 15.73Z" />
                    </svg>
                </a>
                <a href="#" class="social-link">
                    <svg viewBox="0 0 24 24">
                        <path d="M12,2C6.48,2 2,6.48 2,12C2,17.52 6.48,22 12,22C17.52,22 22,17.52 22,12C22,6.48 17.52,2 12,2ZM12,3C13.66,3 15,4.34 15,6C15,7.66 13.66,9 12,9C10.34,9 9,7.66 9,6C9,4.34 10.34,3 12,3ZM12,20C9.65,20 7.5,19.17 5.81,17.83C5.83,16.25 8.13,15 12,15C15.87,15 18.17,16.25 18.19,17.83C16.5,19.17 14.35,20 12,20Z" />
                    </svg>
                </a>
                <a href="#" class="social-link">
                    <svg viewBox="0 0 24 24">
                        <path d="M22.46,6C21.69,6.35 20.86,6.58 20,6.69C20.88,6.16 21.56,5.32 21.88,4.31C21.05,4.81 20.13,5.16 19.16,5.36C18.37,4.5 17.26,4 16,4C13.65,4 11.73,5.92 11.73,8.29C11.73,8.63 11.77,8.96 11.84,9.27C8.28,9.09 5.11,7.38 3,4.79C2.63,5.42 2.42,6.16 2.42,6.94C2.42,8.43 3.17,9.75 4.33,10.5C3.62,10.5 2.96,10.3 2.38,10C2.38,10 2.38,10 2.38,10.03C2.38,12.11 3.86,13.85 5.82,14.24C5.46,14.34 5.08,14.39 4.69,14.39C4.42,14.39 4.15,14.36 3.89,14.31C4.43,16 6,17.26 7.89,17.29C6.43,18.45 4.58,19.13 2.56,19.13C2.22,19.13 1.88,19.11 1.54,19.07C3.44,20.29 5.7,21 8.12,21C16,21 20.33,14.46 20.33,8.79C20.33,8.6 20.33,8.42 20.32,8.23C21.16,7.63 21.88,6.87 22.46,6Z" />
                    </svg>
                </a>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Репетитор по математике Ариан. Все права защищены.</p>
            </div>
        </div>
    </footer>

    <script>
        // Плавная прокрутка к якорям
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetElement.offsetTop - 70,
                    behavior: 'smooth'
                });
                
                // Закрытие мобильного меню после клика
                document.querySelector('nav ul').classList.remove('active');
            });
        });
        
        // Мобильное меню
        document.querySelector('.mobile-menu-btn').addEventListener('click', function() {
            document.querySelector('nav ul').classList.toggle('active');
        });
        
        // Валидация формы
        document.getElementById('feedback-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const emailInput = document.getElementById('email');
            const emailError = document.getElementById('email-error');
            const emailValue = emailInput.value;
            
            // Проверка email на наличие @
            if (!emailValue.includes('@')) {
                emailError.style.display = 'block';
                emailInput.focus();
                return;
            } else {
                emailError.style.display = 'none';
            }
            
            // В реальном приложении здесь был бы код отправки формы
            alert('Сообщение отправлено! Я свяжусь с вами в ближайшее время.');
            this.reset();
        });
    </script>
</body>
</html>
