<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8" />
    <title>ПВЗ Онлайн</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0; 
            padding: 0; 
            background-color: #f4f4f4;
        }
        header {
            background-color: #2d74da;
            color: white;
            padding: 20px;
            text-align: center;
        }
        section {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h2 {
            color: #2d74da;
        }
        .map {
            width: 100%;
            height: 300px;
            margin-top: 15px;
            background-color: #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #555;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin-top: 10px;
        }
        input, textarea {
            padding: 8px;
            margin-top: 5px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }
        button {
            margin-top: 15px;
            padding: 10px;
            background-color: #2d74da;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #1e5bb8;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #2d74da;
            color: white;
            margin-top: 40px;
        }
    </style>
</head>
<body>

<header>
    <h1>ПВЗ "Ваш Пункт Выдачи"</h1>
</header>

<section>
    <h2>Расположение</h2>
    <p>Адрес: г. Москва, ул. Примерная, д. 10</p>
    <div class="map">
        <!-- Здесь можно вставить карту Google Maps или аналог, при необходимости -->
        Карта будет тут
    </div>
</section>

<section>
    <h2>График работы</h2>
    <ul>
        <li>Пн-Пт: 09:00 - 18:00</li>
        <li>Сб: 10:00 - 16:00</li>
        <li>Вс: выходной</li>
    </ul>
</section>

<section>
    <h2>Связаться или оставить заявку</h2>
    <form id="contactForm">
        <label for="name">Имя:</label>
        <input type="text" id="name" name="name" required />

        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required />

        <label for="message">Сообщение:</label>
        <textarea id="message" name="message" rows="4" required></textarea>

        <button type="submit">Отправить</button>
    </form>
</section>

<footer>
    &copy; 2024 Ваш ПВЗ. Все права защищены.
</footer>

<script>
    document.getElementById('contactForm').addEventListener('submit', function(e) {
        e.preventDefault();
        alert('Спасибо за обращение! Мы свяжемся с вами.');
        this.reset();
    });
</script>

</body>
</html>
