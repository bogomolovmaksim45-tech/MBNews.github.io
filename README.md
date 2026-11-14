# Bogomolovmaksim45-tech.github.io

<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MBN — M. B. News</title>

<style>
:root {
    --bg: #242625;
    --panel: #303331;
    --accent: #c5e52c;
    --text: #f5f5f0;
    --muted: #a5aaa4;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    background: var(--bg);
    color: var(--text);
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

header {
    background: #191b1a;
    padding: 20px 7%;
    border-bottom: 3px solid var(--accent);
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.logo {
    display: flex;
    gap: 5px;
    align-items: center;
}

.logo span {
    background: var(--accent);
    color: white;
    font-size: 25px;
    font-weight: 900;
    padding: 5px 9px;
    letter-spacing: -1px;
}

.brand {
    margin-left: 12px;
    font-size: 13px;
    color: var(--muted);
    letter-spacing: 2px;
}

nav {
    display: flex;
    gap: 22px;
}

nav a {
    color: white;
    text-decoration: none;
    font-size: 14px;
    transition: .2s;
}

nav a:hover {
    color: var(--accent);
}

.container {
    max-width: 1050px;
    margin: auto;
    padding: 35px 22px;
}

.category {
    color: var(--accent);
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 2px;
    text-transform: uppercase;
}

.hero {
    padding: 40px 0;
    border-bottom: 1px solid #464a46;
}

.hero h1 {
    font-size: clamp(32px, 6vw, 57px);
    line-height: 1.12;
    max-width: 850px;
    margin: 15px 0;
    letter-spacing: -2px;
}

.hero h1 span {
    color: var(--accent);
}

.hero p {
    color: var(--muted);
    max-width: 650px;
    font-size: 17px;
}

.meta {
    color: #89908a;
    font-size: 12px;
    margin-top: 20px;
}

.page {
    display: none;
    animation: appear .35s ease;
}

.page.active {
    display: block;
}

@keyframes appear {
    from {opacity: 0; transform: translateY(8px);}
    to {opacity: 1; transform: translateY(0);}
}

.article-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    margin-top: 28px;
}

.article {
    background: var(--panel);
    padding: 23px;
    border-left: 3px solid var(--accent);
    border-radius: 4px;
}

.article h3 {
    font-size: 19px;
    margin: 9px 0;
}

.article p {
    color: #b8bdb7;
    font-size: 14px;
}

.article-number {
    color: var(--accent);
    font-size: 12px;
    font-weight: bold;
}

.section-title {
    font-size: 25px;
    margin: 35px 0 15px;
}

.highlight {
    background: #373d2a;
    border: 1px solid #788c25;
    padding: 22px;
    margin: 25px 0;
    border-radius: 5px;
}

.highlight strong {
    color: var(--accent);
}

ul {
    padding-left: 22px;
    color: #c5c9c4;
}

li {
    margin: 10px 0;
}

.quote {
    font-size: 23px;
    font-weight: bold;
    padding: 25px;
    border-left: 4px solid var(--accent);
    margin: 25px 0;
}

.pagination {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 9px;
    margin: 45px 0 25px;
}

.pagination button {
    background: var(--panel);
    color: white;
    border: 1px solid #555b55;
    padding: 10px 16px;
    cursor: pointer;
    border-radius: 4px;
    font-weight: bold;
    transition: .2s;
}

.pagination button:hover {
    border-color: var(--accent);
    color: var(--accent);
}

.pagination button.active {
    background: var(--accent);
    color: #20231c;
    border-color: var(--accent);
}

.pagination button:disabled {
    opacity: .3;
    cursor: not-allowed;
}

.page-indicator {
    text-align: center;
    color: var(--muted);
    font-size: 12px;
    margin-top: -12px;
}

footer {
    background: #191b1a;
    padding: 25px 7%;
    text-align: center;
    color: #929892;
    font-size: 12px;
    border-top: 1px solid #414541;
}

footer strong {
    color: var(--accent);
}

@media(max-width:650px) {
    header {justify-content: center;}
    nav {width:100%; justify-content:center; gap:15px;}
    .article-grid {grid-template-columns: 1fr;}
    .hero h1 {letter-spacing: -1px;}
}
</style>
</head>

<body>

<header>
    <div class="logo">
        <span>M</span>
        <span>B</span>
        <span>N</span>
        <div class="brand">M. B. NEWS</div>
    </div>

    <nav>
        <a href="#" onclick="showPage(1);return false;">Главная</a>
        <a href="#" onclick="showPage(2);return false;">Аналитика</a>
        <a href="#" onclick="showPage(3);return false;">Советы</a>
    </nav>
</header>

<main class="container">

<!-- PAGE 1 -->
<section class="page active" id="page1">

<div class="category">Специальный репортаж • Образ жизни</div>

<div class="hero">
    <h1>У тебя всего 24 часа. <span>Почему ты тратишь их впустую?</span></h1>
    <p>
        Время — единственный ресурс, который невозможно восстановить.
        Узнай, как перестать откладывать жизнь на потом и начать
        распоряжаться каждым днём осознанно.
    </p>
    <div class="meta">MBN EDITORIAL • 15 НОЯБРЯ 2026</div>
</div>

<h2 class="section-title">Куда исчезает наше время?</h2>

<div class="article-grid">
    <article class="article">
        <div class="article-number">01 / ПРОКРАСТИНАЦИЯ</div>
        <h3>«Сделаю это позже» — самая дорогая фраза</h3>
        <p>Откладывая небольшие задачи, мы превращаем их в огромную
        гору дел. Чем дольше ожидание, тем сложнее начать.</p>
    </article>

    <article class="article">
        <div class="article-number">02 / ЦИФРОВЫЕ ОТВЛЕЧЕНИЯ</div>
        <h3>Пять минут в телефоне превращаются в час</h3>
        <p>Бесконечная лента, уведомления и короткие видео
        незаметно отнимают время, которое могло быть потрачено
        на что-то полезное.</p>
    </article>

    <article class="article">
        <div class="article-number">03 / ПЛАНИРОВАНИЕ</div>
        <h3>Занятость не равна продуктивности</h3>
        <p>Можно весь день быть занятым и при этом не выполнить
        ни одной действительно важной задачи.</p>
    </article>

    <article class="article">
        <div class="article-number">04 / ПРИВЫЧКИ</div>
        <h3>Маленькие действия создают большие результаты</h3>
        <p>Даже 20 минут ежедневной работы над целью за год
        превращаются в более чем 120 часов практики.</p>
    </article>
</div>

<div class="highlight">
    <strong>ГЛАВНАЯ МЫСЛЬ:</strong>
    Не обязательно успевать всё. Гораздо важнее успевать то,
    что действительно имеет значение.
</div>
</section>

<!-- PAGE 2 -->
<section class="page" id="page2">

<div class="category">Аналитика • Тайм-менеджмент</div>

<div class="hero">
    <h1>24 часа: <span>куда на самом деле уходит твой день?</span></h1>
    <p>Рациональное распределение времени начинается
    с понимания собственных приоритетов.</p>
</div>

<h2 class="section-title">Раздели день на категории</h2>

<div class="article-grid">
    <article class="article">
        <div class="article-number">СОН</div>
        <h3>7–9 часов</h3>
        <p>Полноценный сон помогает поддерживать концентрацию,
        память и работоспособность.</p>
    </article>

    <article class="article">
        <div class="article-number">РАБОТА И УЧЁБА</div>
        <h3>Основные задачи</h3>
        <p>Выделяй время на обязательства и самые важные дела,
        пока уровень энергии достаточно высок.</p>
    </article>

    <article class="article">
        <div class="article-number">ОТДЫХ</div>
        <h3>Восстановление</h3>
        <p>Перерывы, прогулки, хобби и общение —
        не потеря времени, а необходимая часть жизни.</p>
    </article>

    <article class="article">
        <div class="article-number">ЛИЧНОЕ РАЗВИТИЕ</div>
        <h3>Инвестиция в себя</h3>
        <p>Чтение, изучение языков, спорт и освоение
        новых навыков помогают двигаться вперёд.</p>
    </article>
</div>

<div class="quote">
    «Управлять временем — значит управлять собственными решениями».
</div>

<h2 class="section-title">Три принципа разумного планирования</h2>
<ul>
    <li>Не перегружай день десятками невыполнимых задач.</li>
    <li>Сначала выполняй важное, а не просто самое лёгкое.</li>
    <li>Оставляй свободное время на непредвиденные обстоятельства.</li>
</ul>

<div class="highlight">
    <strong>ВАЖНО:</strong> Не существует универсального расписания.
    Оптимальный режим зависит от возраста, обязанностей,
    потребностей и индивидуального ритма жизни.
</div>

</section>

<!-- PAGE 3 -->
<section class="page" id="page3">

<div class="category">Практика • Руководство</div>

<div class="hero">
    <h1>Перестань обещать себе. <span>Начни действовать.</span></h1>
    <p>Пять простых способов вернуть контроль над собственным временем.</p>
</div>

<h2 class="section-title">5 привычек продуктивного человека</h2>

<div class="article-grid">
    <article class="article">
        <div class="article-number">01</div>
        <h3>Планируй следующий день заранее</h3>
        <p>Вечером запиши 3 главные задачи на завтра.
        Так будет проще начать утро без лишней суеты.</p>
    </article>

    <article class="article">
        <div class="article-number">02</div>
        <h3>Используй правило 25 минут</h3>
        <p>Попробуй 25 минут сосредоточенной работы,
        после которых сделай короткий перерыв.</p>
    </article>

    <article class="article">
        <div class="article-number">03</div>
        <h3>Убери лишние уведомления</h3>
        <p>Отключи ненужные оповещения и убери телефон
        подальше во время важных занятий.</p>
    </article>

    <article class="article">
        <div class="article-number">04</div>
        <h3>Разбивай большие задачи</h3>
        <p>Вместо «выучить весь предмет» поставь
        конкретную цель: изучить одну тему.</p>
    </article>

    <article class="article">
        <div class="article-number">05</div>
        <h3>Не забывай отдыхать</h3>
        <p>Постоянная работа без восстановления
        снижает концентрацию и повышает утомляемость.</p>
    </article>
</div>

<div class="highlight">
    <strong>ТВОЁ ЗАДАНИЕ НА СЕГОДНЯ:</strong>
    Выбери одну задачу, которую давно откладываешь.
    Удели ей хотя бы 15 минут. Не жди идеального момента.
</div>

<div class="quote">
    Твоё будущее складывается из того, как ты распоряжаешься сегодняшним днём.
</div>

</section>

<!-- PAGINATION -->
<div class="pagination">
    <button id="prev" onclick="changePage(-1)">←</button>
    <button class="active" onclick="showPage(1)">1</button>
    <button onclick="showPage(2)">2</button>
    <button onclick="showPage(3)">3</button>
    <button id="next" onclick="changePage(1)">→</button>
</div>

<div class="page-indicator" id="indicator">
    СТРАНИЦА 1 ИЗ 3
</div>

</main>

<footer>
    <div class="logo" style="justify-content:center;margin-bottom:12px">
        <span>M</span><span>B</span><span>N</span>
    </div>
    <strong>M. B. NEWS</strong> — Новости, идеи и знания.
    <br>© 2026 MBN. ALL RIGHTS RESERVED.
</footer>

<script>
let currentPage = 1;
const totalPages = 3;

function showPage(number) {
    currentPage = number;

    document.querySelectorAll('.page').forEach(page => {
        page.classList.remove('active');
    });

    document.getElementById('page' + number).classList.add('active');

    document.querySelectorAll('.pagination button').forEach(btn => {
        btn.classList.remove('active');
    });

    document.querySelectorAll('.pagination button')[number].classList.add('active');

    document.getElementById('indicator').textContent =
        `СТРАНИЦА ${number} ИЗ ${totalPages}`;

    document.getElementById('prev').disabled = number === 1;
    document.getElementById('next').disabled = number === totalPages;

    window.scrollTo({top: 0, behavior: 'smooth'});
}

function changePage(direction) {
    const nextPage = currentPage + direction;

    if (nextPage >= 1 && nextPage <= totalPages) {
        showPage(nextPage);
    }
}

showPage(1);
</script>

</body>
</html>
