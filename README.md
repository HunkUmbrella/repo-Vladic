<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мое Портфолио</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #e9ecef;
            color: #333;
        }
        header {
            background: linear-gradient(to right, #35424a, #5a7d8c);
            color: #ffffff;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        nav {
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            color: #ffffff;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #d9d9d9;
        }
        section {
            margin-bottom: 20px;
            background: #ffffff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        footer {
            text-align: center;
            margin-top: 20px;
            font-size: 0.8em;
            color: #666;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        form input {
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            transition: border 0.3s;
        }
        form input:focus {
            border-color: #35424a;
            outline: none;
        }
        form button {
            padding: 10px;
            background-color: #35424a;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        form button:hover {
            background-color: #3d5b75;
        }
        @media (max-width: 600px) {
            nav {
                display: flex;
                flex-direction: column;
                align-items: center;
            }
            nav a {
                margin: 5px 0;
            }
        }
    </style>
    <script>
        function openProjects() {
            // Скрываем все секции
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                section.style.display = 'none';
            });

            // Создаем новую секцию для проектов
            const projectsSection = document.createElement('section');
            projectsSection.innerHTML = `
                <h2>Проекты</h2>
                <p>Здесь будут мои проекты (сейчас пока пусто).</p>
            `;

            // Добавляем новую секцию на страницу
            document.body.appendChild(projectsSection);
        }
    </script>
</head>
<body>

<header>
    <h1>Мое Портфолио</h1>
</header>

<nav>
    <a href="#about">О себе</a>
    <a href="#skills">Навыки</a>
    <a href="#portfolio" onclick="openProjects()">Проекты</a>
    <a href="#contact">Контакты</a>
</nav>

<section id="about">
    <h2>О себе</h2>
    <p>Привет, меня зовут Влад, я студент 4 курса, учусь по специальности айти программист. У меня есть опыт работы в написании проектов VisualStudio2022 на языке программирования C#. И я люблю заниматься такими вещами как создание проектов с дизайном и продвижение своего опыта в создании своего собственного игрового движка для игр. На текущий момент, сейчас занимаюсь созданию портфолио.</p>
</section>

<section id="skills">
    <h2>Навыки</h2>
    <ul>
        <li>Языки программирования: C#, JavaScript, HTML, CSS</li>
        <li>Знание баз данных: SQL, NoSQL</li>
        <li>Навыки взаимодействия с другими разработчиками и участие в командных проектах помогают создавать более комплексные программы.</li>
    </ul>
</section>

<section id="portfolio">
    <h2>Портфолио</h2>
    <p>Здесь вы можете увидеть мои проекты и работы, над которыми я работал.</p>
    <ul>
       <li><a href="file://192.168.3.250/Veda/4%20%D0%9A%D1%83%D1%80%D1%81/%D0%98%D0%A1%D0%9F%2043-9,%20%D0%98%D0%A1%D0%9F%2044-11/%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B8%20%D1%80%D0%B0%D0%B7%D1%80%D0%B0%D0%B1%20%D0%B2%D0%B5%D0%B1%20%D0%BF%D1%80%D0%B8%D0%BB/%D0%91%D0%B0%D0%BA%D0%B0%D0%B5%D0%B2/index22.html">Проекты</a></li>    </ul>

    <h3>Авторизация</h3>
    <form id="login-form">
        <input type="email" placeholder="Электронная почта" required>
        <input type="password" placeholder="Пароль" required>
        <button type="submit">Войти</button>
    </form>

    <h3>Регистрация</h3>
    <form id="registration-form">
        <input type="text" placeholder="Имя" required>
        <input type="email" placeholder="Электронная почта" required>
        <input type="password" placeholder="Пароль" required>
        <button type="submit">Зарегистрироваться</button>
    </form>
</section>

<section id="contact">
    <h2>Контакты</h2>
    <p>Вы можете связаться со мной по электронной почте: <a href="mailto:vladbakaev7@gmail.com">vladbakaev7@gmail.com</a></p>
</section>

<footer>
    <p>&copy; 2025 Мое Имя</p>
</footer>

</body>
</html>
