<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MEGA-FIT: Все тренировки в одном месте</title>
    <style>
        :root {
            --primary: #ff4757;
            --dark: #2f3542;
            --light: #f1f2f6;
        }
        body { font-family: 'Segoe UI', sans-serif; margin: 0; line-height: 1.6; background: var(--light); color: var(--dark); }
        
        /* Шапка и Навигация */
        header { background: var(--dark); color: white; padding: 1rem; position: sticky; top: 0; z-index: 1000; }
        nav { display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; }
        nav a { color: white; text-decoration: none; font-weight: bold; }
        nav a:hover { color: var(--primary); }

        .container { max-width: 1000px; margin: auto; padding: 20px; }
        section { margin-bottom: 50px; background: white; padding: 30px; border-radius: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); }
        
        h1, h2 { color: var(--primary); border-bottom: 2px solid var(--primary); padding-bottom: 10px; }

        /* Стили таблиц */
        table { width: 100%; border-collapse: collapse; margin-top: 20px; }
        th, td { padding: 12px; border: 1px solid #ddd; text-align: left; }
        th { background: var(--dark); color: white; }

        /* Кнопки и Интерактив */
        .btn { background: var(--primary); color: white; border: none; padding: 15px 25px; border-radius: 30px; cursor: pointer; font-size: 1.1em; display: inline-block; text-decoration: none; }
        .btn:hover { opacity: 0.9; transform: scale(1.02); }

        /* Карточки упражнений */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 20px; }
        .card { border: 1px solid #eee; padding: 15px; border-radius: 10px; text-align: center; }
        .video-link { color: #ff0000; font-weight: bold; text-decoration: none; }

        footer { text-align: center; padding: 20px; background: var(--dark); color: white; margin-top: 50px; }
    </style>
</head>
<body>

<header>
    <nav>
        <a href="#home">Главная</a>
        <a href="#gym">В зале</a>
        <a href="#home-work">Дома</a>
        <a href="#base">База упражнений</a>
        <a href="#generator">Генератор дня</a>
    </nav>
</header>

<div class="container">

    <section id="home">
        <h1>Твой личный тренировочный хаб</h1>
        <p>Добро пожаловать! Здесь собраны лучшие программы для тех, кто хочет изменить своё тело. Неважно, где ты — в элитном спортзале или в однушке на коврике.</p>
        <img src="https://images.unsplash.com/photo-1517836357463-d25dfeac3438?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80" alt="Fitness" style="width:100%; border-radius:15px;">
    </section>

    <section id="gym">
        <h2>Программы для зала (3 дня в неделю)</h2>
        <p>Классический сплит для набора массы и силы.</p>
        <table>
            <tr>
                <th>День</th>
                <th>Группа мышц</th>
                <th>Основные упражнения</th>
            </tr>
            <tr>
                <td>Пн</td>
                <td>Грудь / Трицепс</td>
                <td>Жим лежа, Брусья, Разводка</td>
            </tr>
            <tr>
                <td>Ср</td>
                <td>Спина / Бицепс</td>
                <td>Подтягивания, Тяга штанги, Молотки</td>
            </tr>
            <tr>
                <td>Пт</td>
                <td>Ноги / Плечи</td>
                <td>Присед, Жим ногами, Армейский жим</td>
            </tr>
        </table>
    </section>

    <section id="home-work">
        <h2>Тренировки дома (Без инвентаря)</h2>
        <div class="grid">
            <div class="card">
                <h3>Интенсивное Кардио</h3>
                <p>20 минут HIIT тренировки для сжигания жира.</p>
                <a href="https://www.youtube.com/results?search_query=hiit+workout+home" target="_blank" class="video-link">Смотреть видео ▶</a>
            </div>
            <div class="card">
                <h3>Крепкий пресс</h3>
                <p>8 упражнений на все отделы мышц живота.</p>
                <a href="https://www.youtube.com/results?search_query=abs+workout" target="_blank" class="video-link">Смотреть видео ▶</a>
            </div>
            <div class="card">
                <h3>Йога / Растяжка</h3>
                <p>Восстановление после тяжелого дня.</p>
                <a href="https://www.youtube.com/results?search_query=yoga+for+beginners" target="_blank" class="video-link">Смотреть видео ▶</a>
            </div>
        </div>
    </section>

    <section id="base">
        <h2>Энциклопедия упражнений</h2>
        <p>Кликни на упражнение, чтобы увидеть технику выполнения.</p>
        <ul>
            <li><a href="https://www.youtube.com/results?search_query=техника+приседаний" target="_blank">Приседания со штангой</a></li>
            <li><a href="https://www.youtube.com/results?search_query=техника+становой+тяги" target="_blank">Становая тяга</a></li>
            <li><a href="https://www.youtube.com/results?search_query=техника+отжиманий" target="_blank">Отжимания от пола</a></li>
            <li><a href="https://www.youtube.com/results?search_query=техника+планки" target="_blank">Планка (классическая)</a></li>
        </ul>
    </section>

    <section id="generator" style="text-align: center;">
        <h2>Рандомайзер тренировки</h2>
        <p>Не знаешь что делать? Нажми кнопку!</p>
        <div id="display-workout" style="font-size: 1.5rem; margin: 20px; font-weight: bold; color: var(--primary);">
            Нажми на кнопку ниже 👇
        </div>
        <button class="btn" onclick="generate()">Получить задание на сегодня</button>
    </section>

</div>

<footer>
    <p>&copy; 2024 Мой Фитнес Блог. Сделано с помощью Блокнота и Духа Спорта!</p>
</footer>

<script>
    function generate() {
        const tasks = [
            "100 Приседаний за минимальное время",
            "Планка 5 минут (суммарно)",
            "50 Отжиманий + 50 Скручиваний",
            "30 минут быстрой ходьбы",
            "День отдыха и растяжки",
            "10 минут прыжков со скакалкой"
        ];
        const random = tasks[Math.floor(Math.random() * tasks.length)];
        document.getElementById('display-workout').innerText = random;
    }
</script>

</body>
</html># -
