<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Памятка для волонтёров ДОД • Химический факультет МГУ</title>
    <link href="https://fonts.googleapis.com/css2?family=Spectral:wght@400;600;700&family=IBM+Plex+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #1a5490;
            --secondary: #2d7dd2;
            --accent: #e74c3c;
            --bg-light: #f8f9fa;
            --bg-white: #ffffff;
            --text-dark: #1a1a1a;
            --text-gray: #4a4a4a;
            --border: #e0e0e0;
            --highlight: #fff3cd;
            --success: #28a745;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'IBM Plex Sans', -apple-system, BlinkMacSystemFont, sans-serif;
            line-height: 1.7;
            color: var(--text-dark);
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 20px;
            animation: fadeIn 0.6s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            background: var(--bg-white);
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
            overflow: hidden;
            animation: slideUp 0.8s ease-out;
        }

        @keyframes slideUp {
            from { 
                opacity: 0;
                transform: translateY(30px);
            }
            to { 
                opacity: 1;
                transform: translateY(0);
            }
        }

        .header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 60px 50px;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -10%;
            width: 500px;
            height: 500px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            animation: float 20s infinite ease-in-out;
        }

        @keyframes float {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            33% { transform: translate(30px, -30px) rotate(120deg); }
            66% { transform: translate(-20px, 20px) rotate(240deg); }
        }

        .header h1 {
            font-family: 'Spectral', serif;
            font-size: 3.2em;
            font-weight: 700;
            margin-bottom: 15px;
            position: relative;
            z-index: 1;
            letter-spacing: -1px;
        }

        .header .subtitle {
            font-size: 1.3em;
            opacity: 0.95;
            font-weight: 300;
            position: relative;
            z-index: 1;
        }

        .content {
            padding: 50px;
        }

        .welcome {
            background: linear-gradient(to right, #ffeaa7, #fdcb6e);
            border-left: 5px solid #e17055;
            padding: 25px 30px;
            margin-bottom: 40px;
            border-radius: 10px;
            font-size: 1.1em;
            animation: slideIn 0.6s ease-out 0.3s both;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-20px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .section {
            margin-bottom: 45px;
            animation: slideIn 0.6s ease-out both;
        }

        .section:nth-child(1) { animation-delay: 0.1s; }
        .section:nth-child(2) { animation-delay: 0.2s; }
        .section:nth-child(3) { animation-delay: 0.3s; }
        .section:nth-child(4) { animation-delay: 0.4s; }
        .section:nth-child(5) { animation-delay: 0.5s; }

        h2 {
            font-family: 'Spectral', serif;
            font-size: 2em;
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 12px;
            border-bottom: 3px solid var(--secondary);
            display: inline-block;
            font-weight: 600;
        }

        h3 {
            font-family: 'Spectral', serif;
            font-size: 1.5em;
            color: var(--secondary);
            margin: 30px 0 15px 0;
            font-weight: 600;
        }

        h4 {
            font-size: 1.2em;
            color: var(--text-dark);
            margin: 20px 0 12px 0;
            font-weight: 600;
        }

        p {
            margin-bottom: 15px;
            color: var(--text-gray);
        }

        .streams-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin: 25px 0;
        }

        .stream-card {
            background: var(--bg-light);
            padding: 20px;
            border-radius: 12px;
            border-left: 4px solid var(--secondary);
            transition: all 0.3s ease;
        }

        .stream-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
            border-left-color: var(--accent);
        }

        .stream-card strong {
            display: block;
            color: var(--primary);
            margin-bottom: 8px;
            font-size: 1.1em;
        }

        .requirements-list {
            background: linear-gradient(135deg, #e3f2fd 0%, #bbdefb 100%);
            padding: 25px 30px;
            border-radius: 12px;
            margin: 20px 0;
        }

        .requirements-list ul {
            list-style: none;
            padding: 0;
        }

        .requirements-list li {
            padding: 12px 0 12px 35px;
            position: relative;
            color: var(--text-dark);
            font-weight: 400;
        }

        .requirements-list li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--success);
            font-weight: bold;
            font-size: 1.3em;
        }

        .important-box {
            background: var(--highlight);
            border: 2px solid #ffc107;
            padding: 20px 25px;
            border-radius: 10px;
            margin: 20px 0;
            font-weight: 500;
        }

        .important-box strong {
            color: var(--accent);
            font-size: 1.1em;
        }

        .timeline {
            position: relative;
            padding-left: 40px;
            margin: 25px 0;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 10px;
            top: 0;
            bottom: 0;
            width: 3px;
            background: var(--secondary);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 20px;
            padding-left: 20px;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -33px;
            top: 5px;
            width: 15px;
            height: 15px;
            border-radius: 50%;
            background: var(--secondary);
            border: 3px solid white;
            box-shadow: 0 0 0 2px var(--secondary);
        }

        .timeline-item strong {
            color: var(--primary);
            font-size: 1.1em;
            display: block;
            margin-bottom: 5px;
        }

        .faq-item {
            background: white;
            border: 1px solid var(--border);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 15px;
            transition: all 0.3s ease;
        }

        .faq-item:hover {
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            border-color: var(--secondary);
        }

        .faq-question {
            font-weight: 600;
            color: var(--primary);
            margin-bottom: 10px;
            font-size: 1.05em;
        }

        .faq-answer {
            color: var(--text-gray);
            line-height: 1.6;
        }

        .link-button {
            display: inline-block;
            background: var(--secondary);
            color: white;
            padding: 12px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            margin: 5px 5px 5px 0;
        }

        .link-button:hover {
            background: var(--primary);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .roles-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .role-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
            transition: all 0.3s ease;
        }

        .role-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.25);
        }

        .role-card h3 {
            color: white;
            margin-top: 0;
            font-size: 1.6em;
        }

        .role-card ul {
            list-style: none;
            padding: 0;
        }

        .role-card li {
            padding: 8px 0;
            padding-left: 25px;
            position: relative;
        }

        .role-card li::before {
            content: '→';
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        .highlight-text {
            background: linear-gradient(120deg, #84fab0 0%, #8fd3f4 100%);
            padding: 2px 8px;
            border-radius: 4px;
            font-weight: 500;
        }

        .footer {
            background: var(--bg-light);
            padding: 30px 50px;
            text-align: center;
            color: var(--text-gray);
            font-size: 0.95em;
        }

        @media (max-width: 768px) {
            .header {
                padding: 40px 30px;
            }

            .header h1 {
                font-size: 2.2em;
            }

            .content {
                padding: 30px 25px;
            }

            .streams-grid,
            .roles-section {
                grid-template-columns: 1fr;
            }

            .timeline {
                padding-left: 30px;
            }
        }

        .badge {
            display: inline-block;
            padding: 5px 12px;
            background: var(--accent);
            color: white;
            border-radius: 20px;
            font-size: 0.85em;
            font-weight: 600;
            margin-left: 10px;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }

        .info-card {
            background: white;
            border: 2px solid var(--border);
            border-radius: 10px;
            padding: 15px 20px;
            transition: all 0.3s ease;
        }

        .info-card:hover {
            border-color: var(--secondary);
            transform: translateX(5px);
        }

        .info-card strong {
            display: block;
            color: var(--secondary);
            margin-bottom: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Памятка для волонтёров ДОД</h1>
            <div class="subtitle">Химический факультет МГУ имени М.В.Ломоносова</div>
        </div>

        <div class="content">
            <div class="welcome">
                <strong>Привет!</strong> Спасибо, что согласился/ась помочь и представить наш факультет. Тебе предстоит рассказать абитуриентам и их родителям о поступлении в МГУ и на Химический факультет.
            </div>

            <div class="section">
                <h2>Структура ДОДа</h2>
                <p>Весь День открытых дверей состоит из трёх важных частей:</p>
                
                <div class="info-grid">
                    <div class="info-card">
                        <strong>ГЗ</strong>
                        Ответы на вопросы абитуриентов и их родителей
                    </div>
                    <div class="info-card">
                        <strong>Встреча гостей на химфаке</strong>
                        Координация людей на факультете
                    </div>
                    <div class="info-card">
                        <strong>Экскурсии по лабораториям кафедр</strong>
                        Собираем группу гостей и провожаем их до лабораторий в соответствии с маршрутом
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>Общий план ДОДа</h2>
                <div class="timeline">
                    <div class="timeline-item">
                        <strong>9:00</strong>
                        Сбор волонтёров у стенда Химфака в ГЗ, подготовка
                    </div>
                    <div class="timeline-item">
                        <strong>10:00</strong>
                        Официальное начало ДОДа в ГЗ
                    </div>
                    <div class="timeline-item">
                        <strong>12:00</strong>
                        Лекция Садовничего в актовом зале ГЗ (будет трансляция на сайте ДОДа)
                    </div>
                    <div class="timeline-item">
                        <strong>13:00</strong>
                        Сбор волонтёров на Химфаке, подготовка
                    </div>
                    <div class="timeline-item">
                        <strong>13:30</strong>
                        Консультация по поступлению (аудитория 02 в ГЗ)
                    </div>
                    <div class="timeline-item">
                        <strong>14:30</strong>
                        Начало ДОДа на факультетах, в том числе на Химфаке
                    </div>
                    <div class="timeline-item">
                        <strong>16:00-16:30</strong>
                        Начало экскурсий по лабораториям кафедр на Химфаке
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>Общие требования ко всем волонтёрам</h2>
                <div class="requirements-list">
                    <ul>
                        <li><strong>Дресс-код:</strong> опрятный белый верх (футболка с символикой Химфака), чёрный (тёмный) низ</li>
                        <li>Как только приходим на точку, нужно написать в чате в телеграм разделе "Время" время прихода в формате "Фамилия Имя пришёл/пришла в ХХ:ХХ", и аналогично с временем завершения работы</li>
                        <li>Быть счастливыми и выспавшимися 😊</li>
                        <li>Взять с собой водичку и небольшой перекус (говорить будем много + будет душно)</li>
                        <li>Быть на связи и оперативно реагировать на звонки/сообщения</li>
                    </ul>
                </div>
            </div>

            <div class="section">
                <h2>Инструкции для разных потоков</h2>
                
                <div class="roles-section">
                    <div class="role-card">
                        <h3>Волонтёрам ГЗ</h3>
                        <ul>
                            <li><strong>Сбор:</strong> 9:00 в ГЗ у стенда Химфака</li>
                            <li>Куртку оставляем в гардеробе + сменка для комфорта</li>
                            <li>Не знаем ответ? Направляем к старшим или за стойку факультета</li>
                            <li><strong>Главная задача:</strong> показать, что на Химфаке круто и интересно учиться!</li>
                        </ul>
                    </div>

                    <div class="role-card" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);">
                        <h3>ХФ начало</h3>
                        <ul>
                            <li><strong>Сбор:</strong> 13:00 на Химфаке (заходим в 168а за футболкой и бейджем)</li>
                            <li>13:00-13:10 — расстановка на позиции</li>
                            <li>с 13:30 можно запускать в БХА (будут научно-популярные фильмы)</li>
                            <li>до 14:50 — встреча гостей</li>
                            <li>14:30-16:00 — лекция в БХА</li>
                            <li>16:30-19:00 — экскурсии</li>
                        </ul>
                    </div>

                    <div class="role-card" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);">
                        <h3>Экскурсии</h3>
                        <ul>
                            <li><strong>Сбор:</strong> 16:00-16:30 в Сачке</li>
                            <li>Распределение по маршрутам будет позже</li>
                            <li>Всё будет в таблице, следите за обновлениями!</li>
                            <li>После лекции в БХА люди пойдут на экскурсии</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>FAQ: Часто задаваемые вопросы</h2>
                
                <h3>Бытовые вопросы</h3>
                
                <div class="faq-item">
                    <div class="faq-question">Где можно покушать/сходить в туалет?</div>
                    <div class="faq-answer">
                        <strong>Туалеты:</strong> нужно пройти в сторону выхода, в прямоугольном холле перед круглым холлом будут слева и справа.<br>
                        <strong>Питание:</strong> будет работать круглый холл или кафе поблизости от МГУ, также на факультете — Кофепорт (с 12:00 до 17:30) и Алхимик (скорее всего с 10:00 до 19:00).
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Где находится стенд другого факультета?</div>
                    <div class="faq-answer">
                        Естественно-научные и точные факультеты находятся на 1 этаже, остальные, в том числе СУНЦ и филиалы — на 2 этаже. На стойке будут лежать карты с расположением.
                        <br><br>
                        <strong>Важно:</strong> Круглый холл не называем "шайбой", говорим "круглый холл" (можно упомянуть красные колонны).
                    </div>
                </div>

                <h3>О химфаке и МГУ</h3>

                <div class="faq-item">
                    <div class="faq-question">Что по общежитиям?</div>
                    <div class="faq-answer">
                        Студенты Химфака МГУ с 1 по 3 курс живут в новых общежитиях квартирного типа. Среднее время от общаги до универа — 15 минут. После 3 курса переезжают в здание ещё ближе к химфаку (5 минут).<br>
                        <strong>Стоимость:</strong> в МГУ самое дешевое проживание — 4 руб/сут + 520 рублей в месяц за коммунальные услуги.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Где можно узнать всю информацию?</div>
                    <div class="faq-answer">
                        На факультете ведётся активная информационная работа. Есть официальная группа Абитуриентов, где публикуется текущая информация о приёме документов, проведении ДВИ и ссылки на списки на сайте приёмной комиссии.<br><br>
                        Также есть группа Студенческой комиссии Профкома ХФ, официальная группа ХФ ВКонтакте и канал в ТГ. QR-коды и ссылки будут на стойке в распечатанном виде.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Сколько лет учиться?</div>
                    <div class="faq-answer">
                        <strong>Специалитет:</strong> 6 лет (для граждан РФ, Беларуси, Казахстана, Кыргызстана и др.)<br>
                        <strong>Бакалавриат:</strong> 4 года (только для иностранных граждан)<br>
                        <strong>Магистратура:</strong> 2 года<br>
                        <strong>Аспирантура:</strong> 4 года
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Кем я смогу работать после выпуска?</div>
                    <div class="faq-answer">
                        После окончания химического факультета можно податься в любую область: бóльшая часть выпускников идёт в науку (60%), некоторые — в фармкомпании, нефть, удобрения, Ростех, Росатом, Унихимтек и др. Часть уходит в преподавание.<br><br>
                        <span class="highlight-text">ПОСЛЕ ОКОНЧАНИЯ ХИМФАКА ОЧЕНЬ СЛОЖНО СТАТЬ НЕУСПЕШНЫМ</span>
                    </div>
                </div>

                <h3>Поступление на специалитет</h3>

                <div class="faq-item">
                    <div class="faq-question">Сколько баллов нужно набрать?</div>
                    <div class="faq-answer">
                        Среднего балла нет — это один из многих факторов. В среднем, если написать каждый из 5 экзаменов (4 ЕГЭ + ДВИ) на 85 баллов, вы с большой вероятностью поступите. По конкретным вопросам направляем на стойку.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Какие экзамены для поступления?</div>
                    <div class="faq-answer">
                        <strong>ДВИ по химии</strong> — дополнительное вступительное испытание в письменной форме (сдаётся во второй половине июля на факультете)<br>
                        <strong>ЕГЭ:</strong> химия, математика (профильная), физика или биология (на выбор, наивысший результат), русский язык
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Как подготовиться к ДВИ?</div>
                    <div class="faq-answer">
                        Есть платные онлайн-курсы от ХФ для подготовки к ЕГЭ и ДВИ по всем предметам: <a href="https://do.chem.msu.ru/dl/" class="link-button">Дистанционные курсы</a><br><br>
                        К факультету относится Школа Юного Химика (обучение бесплатное для победителей олимпиад).<br><br>
                        Ежегодно выпускается сборник с разбором заданий ДВИ — его можно приобрести в книжном киоске на 2 этаже ХФ.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Дополнительные баллы</div>
                    <div class="faq-answer">
                        <strong>Значок ГТО:</strong> 2 балла<br>
                        <strong>Аттестат с отличием / медаль / диплом колледжа с отличием:</strong> 6 баллов<br>
                        <strong>Итоговое сочинение:</strong> 2 балла<br>
                        <strong>Спортивные достижения высокого уровня:</strong> дополнительные баллы
                    </div>
                </div>

                <h3>О магистратуре</h3>

                <div class="faq-item">
                    <div class="faq-question">Программы магистратуры</div>
                    <div class="faq-answer">
                        <strong>Направления:</strong> 04.04.01 "Химия" и 18.04.01 "Химическая технология"<br>
                        <strong>Форма:</strong> очная, 2 года<br>
                        <strong>Вступительное испытание:</strong> письменный экзамен по химии<br>
                        <strong>Бюджет:</strong> 12 мест на "Химию", 15 мест на "Химическую технологию"<br>
                        Также есть платные места и 3 англоязычные программы в области радиохимии.
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>Самые потрясающие кафедры ХФ</h2>
                
                <div class="faq-item">
                    <div class="faq-question">Кафедра медицинской химии</div>
                    <div class="faq-answer">
                        Основная задача — подготовка химиков-органиков, специализирующихся в области синтеза и конструирования физиологически активных веществ и лекарственных препаратов.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Кафедра аналитической химии</div>
                    <div class="faq-answer">
                        Разработка оригинальных методов химического анализа, решение задач анализа экологических, биомедицинских, технических объектов. Много современных приборов, на которых работают даже студенты младших курсов.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Кафедра органической химии</div>
                    <div class="faq-answer">
                        Направления: молекулярный дизайн, целевой синтез, элементоорганические соединения как реагенты и катализаторы, катализ, супрамолекулярная химия, фотохимия, современные методы анализа.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Кафедра радиохимии</div>
                    <div class="faq-answer">
                        Исследования: ядерный топливный цикл нового поколения, радиофармацевтическая химия, ядерная медицина, химическая физика f-элементов, квантово-химические расчёты.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Кафедра химической энзимологии</div>
                    <div class="faq-answer">
                        Физическая химия ферментов, генетическая и белковая инженерия, инженерная энзимология и биотехнология, применение ферментов в медицине и ветеринарии.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">Кафедра химии и электрохимии</div>
                    <div class="faq-answer">
                        НИЛ с множеством специалистов: работа с суперконденсаторами, органическими электролитами, электродами из рисовой шелухи, металлоорганических комплексов. Высококлассное оборудование для исследований.
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>Студенческая жизнь</h2>
                <p>На факультете очень сильный институт студенческих организаций. Студенты в свободное время делают жизнь факультета лучше и участвуют в организации мероприятий:</p>
                
                <div class="info-grid">
                    <div class="info-card">
                        <strong>Профком</strong>
                        Защита прав студентов, консультации о льготах, информирование о событиях, еженедельные мероприятия
                    </div>
                    <div class="info-card">
                        <strong>Клубы по интересам</strong>
                        Шахматный клуб, настольные игры, гитарные вечера (2 раза в месяц)
                    </div>
                    <div class="info-card">
                        <strong>Культмасс</strong>
                        Возможность реализовать творческий потенциал: пение, танцы, сценки на мероприятиях факультета
                    </div>
                    <div class="info-card">
                        <strong>День Химика 2026</strong>
                        Масштабное мероприятие в мае, вход свободный для всех желающих
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>Полезные ссылки</h2>
                <a href="https://openday.msu.ru/" class="link-button">День открытых дверей МГУ</a>
                <a href="https://do.chem.msu.ru/dl/" class="link-button">Дистанционные курсы подготовки</a>
                <a href="https://docs.google.com/spreadsheets/d/1G11XiXfp42Fm7GqaoC6Tjg3zaWWBaYDowFPQhr9b9UQ/edit?usp=sharing" class="link-button">Таблица распределения</a>
                <a href="https://docs.google.com/document/d/10Fwh4oVMwfNdII6uFMnEDthCjp_IF-olZHGr5GR8fwk/edit?usp=sharing" class="link-button">QR-коды для абитуриентов</a>
            </div>

        </div>

        <div class="footer">
            <p><strong>Желаем успешного Дня открытых дверей!</strong></p>
            <p>Химический факультет МГУ имени М.В.Ломоносова • 2026</p>
        </div>
    </div>

    <script>
        // Добавляем плавную прокрутку
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        // Анимация при появлении элементов в viewport
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.faq-item, .stream-card, .role-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'all 0.6s ease-out';
            observer.observe(el);
        });
    </script>
</body>
</html>
