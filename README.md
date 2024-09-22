<h1>WhatsApp</h1>

<h2>ДЗ1</h2>

<h3>Целевая аудитория</h3>
<p>Более 2.9 млрд по всему миру, более 2 млрд MAU за 2024 год, 1.66 млрд DAU [1]. Самое большое количество пользователей - в Индии (535.8 млн), далее идут Бразилия (139.3 млн),
США (91.3 млн). В РФ активных пользователей WhatsApp 66.7 млн. [2]</p>

<h3>Ключевые продуктовые решения</h3>
<ol>
    <li>Сервис максимально ориентирован под мобилки, изначально WhatsApp был задуман как замена SMS [3]</li>
    <li>После подтвержденного получения сообщения сервер стирает отправленное сообщение из памяти, оно хранится на клиенте [4]</li>
</ol>

<h3>Ключевой функционал</h3>
<ol>
    <li>Зарегистрироваться/войти по номеру телефона</li>
    <li>CRUD сообщений (read - читать диалог)</li>
    <li>CRUD групповых чатов</li>
    <li>Просмотреть список диалогов</li>
    <li>Найти пользователя по номеру телефона</li>
    <li>Отправить вложение (фото/видео/аудио/файл/голосовое сообщение)</li>
    <li>Аватарки пользователей (статические картинки)</li>
    <li>Аудиозвонки</li>
</ol>

<h3>Список использованных источников</h3>
<ol>
    <li>https://analyzify.com/statsup/whatsapp</li>
    <li>https://worldpopulationreview.com/country-rankings/whatsapp-users-by-country</li>
    <li>https://www.whatsapp.com/about</li>
    <li>https://highscalability.com/the-whatsapp-architecture-facebook-bought-for-19-billion/</li>
</ol>

<h2>ДЗ2</h2>

<h3>Продуктовые метрики</h3>

<h5>MAU - 2 млрд</h5>

<h5>DAU - 1.66 млрд</h5>

<h5>Средний размер пользовательских хранилищ</h5>

<table>
    <thead>
        <th>Тип хранилища</th>
        <th>Средний объем на 1 пользователя</th>
    </thead>
    <tbody>
        <tr>
            <td>Текстовые сообщения</td>
            <td>90 bil (approximately) / 3 bil = 30 messages a day per user, about 15 Kb a day per user, *365 a year (by 2024), 0.41 of that a year avg since 2010 (average MAU since 2010 is 0,41 of that in 2024), * 15 years passed = * 6.27 a year avg, total = 15 * 365 * 6.27 * 15 Kb per user = 21900 Kb per user = <b>4.19 MB</b> per user</td>
        </tr>
        <tr>
            <td>Голосовые сообщения</td>
            <td>150 mil a day / 3 bil, 0.05 per user a day, 20 sec avg [1], 1 sec per user per day avg, 365 * 6.27 secs per user total, WhatsApp typically uses the Opus codec for voice messages, which has a bitrate of around 16 kbps (kilobits per second), so 16 * 365 * 6.27 Kb per user total = <b>4.47 MB</b> per user</td>
        </tr>
        <tr>
            <td>Медиа-файлы</td>
            <td>10 bil total media a day,  / 3 bil users, max img size = 5 MB, let avg be 1 MB, 10 / 3 MB per user per day, (10/3) * 365 * 6.27 MB per user total = <b>7.45 GB</b></td>
        </tr>
    </tbody>
</table>

<h5>Среднее кол-во действий пользователя по типам в день</h5>

<table>
    <thead>
        <th>Тип действия</th>
        <th>Среднее кол-во действий в день</th>
    </thead>
    <tbody>
        <tr>
            <td>Просмотр списков диалогов</td>
            <td>34.19 billion total annual visits in 2021, 2.13b users in 2021, 2.9b in 2024, 34.19 * 6.27 billion total annual visits in 2024, * 1/365 [3] = 34.19 * 2.9 / 365 / 2.13 bil = <b>127 mil</b></td>
        </tr>
        <tr>
            <td>Поиск чата по номеру телефона</td>
            <td>Let 1 in 200 messages is to new user, 100 bil / 150 = <b>500 mil</b></td>
        </tr>
        <tr>
            <td>Отправка сообщений</td>
            <td><b>100 bil</b>[2]</td>
        </tr>
        <tr>
            <td>Отправка сообщений с вложениями</td>
            <td> 6.9 billion images are shared on WhatsApp chat each day [3], <b>10 bil total attachments</b>
            </td>
        </tr>
        <tr>
            <td>Отправка голосовых сообщений</td>
            <td><b>150 mil</b> a day [1]</td>
        </tr>
        <tr>
            <td>Отправка сообщений в групповых чатах</td>
            <td>57.5% of all messages are sent in groups with more than two participants https://analyzify.com/statsup/whatsapp. 100 bil * 57.5% = <b>57.5 bil</b></td>
        </tr>
        <tr>
            <td>Аудиозвонки</td>
            <td>Almost 2 billion minutes are spent each day on WhatsApp calls [3] 120 bil secs / 182 secs avg voice call = <b>659 mil</b> voice calls avg</td>
        </tr>
    </tbody>
</table>

<h3>Технические метрики</h3>

<h5>Размер хранения в разбивке по типам данных</h5>
<table>
    <thead>
        <th>Тип хранилища</th>
        <th>Объем хранилища по типам данных, Тб</th>
    </thead>
    <tbody>
        <tr>
            <td>Текстовые сообщения</td>
            <td>11 973 TB</td>
        </tr>
        <tr>
            <td>Голосовые сообщения</td>
            <td>12 789 TB</td>
        </tr>
        <tr>
            <td>Медиа-файлы</td>
            <td>21 826 172 TB</td>
        </tr>
    </tbody>
</table>

<h5>Сетевые метрики</h5>
<table>
    <thead>
        <th>Тип запроса</th>
        <th>RPS средний</th>
        <th>RPS пиковый</th>
        <th>Пиковое потребление в течение суток (в Гбит/с)</th>
        <th>Суммарный суточный (Гбайт/сутки)</th>
    </thead>
    <tbody>
        <tr>
            <td>Отправка сообщения</td>
            <td>1 157 400</td>
            <td>2 000 000</td>
            <td>2 mil * 0.5 Kb = 10 mil Kb = <b>1 Gb/sec</b></td>
            <td>1 * (1157400/2000000) / 8 * 24 * 3600 = <b>5 956 GB/day</b></td>
        </tr>
        <tr>
            <td>Просмотр списка диалогов</td>
            <td>1471</td>
            <td>5000</td>
            <td>5000 * 1 Kb (w/out avatars) * 0.1 (client caches are hit in 90% of the requests) = 500 Kb = <b>0.00047 Gb/sec</b></td>
            <td>0.00047 * (1471/5000) / 8 * 24 * 3600 = <b>0.1493 GB/day</b></td>
        </tr>
        <tr>
            <td>Сохранение вложения</td>
            <td>110 000</td>
            <td>200 000</td>
            <td>1 MB avg attach, 200 000 * 1 * 8 / 1024 = <b>790 Gb/sec</b></td>
            <td>790 * (110000 / 200000) / 8 * 24 * 3600 = <b>4 640 328 GB/day</b></td>
        </tr>
        <tr>
            <td>Аудиозвонок</td>
            <td>7 627</td>
            <td>20 000</td>
            <td>2 billion minutes a day * 60 sec * 16 Kbps / (24 * 3600) = <b>21.19 Gb/sec</b></td>
            <td>21.19 * (7 627 / 20 000) / 8 * 3600 * 24 = <b>87 272 GB/day</b></td>
        </tr>
        <tr>
            <td>Голосовое сообщение</td>
            <td>150 mil / (24 * 3600) = <b>1787</b></td>
            <td>5000</td>
            <td>5000 * 16 Kbps * 20 sec avg length = 1 600 000 Kbps = <b>1.52 Gb/s</b></td>
            <td>1.52 * (1787 / 5000) / 8 * 3600 * 24 = <b>5 867 GB/day</b></td>
        </tr>
        <tr>
            <td>Поиск по телефону</td>
            <td>150 mil / (24 * 3600) = <b>1736</b></td>
            <td>5000</td>
            <td>12000 * 10 Kb = 120000 Kbps = <b>0.11 Gb/s</b></td>
            <td>0.11 * (5787 / 12000) / 8 * 3600 * 24 = <b>573 GB/day</b></td>
        </tr>
        <tr>
            <td>Логин</td>
            <td>Let once in 180 days 1 user is logged out. 1.66 bil DAU / 180 = 9 220 000 logins a day = <b>106 RPS</b></td>
            <td>400</td>
            <td>400 * 1 Kb = 400 Kbps = <b>0.0004 Gb/s</b></td>
            <td>0.0004 * (106/400) / 8 * 3600 * 24 = <b>1 GB/day</b></td>
        </tr>
        <tr>
            <td>Создание группового чата</td>
            <td>Let it happen once in 5 searches by phone: 1736 / 5 = <b>340 RPS</b></td>
            <td>1000</td>
            <td>1000 * 5 Kb = 5000 Kbps = <b>0.004 Gb/s</b></td>
            <td>0.004 * (340/1000) / 8 * 3600 * 24 = <b>17.5 GB/day</b></td>
        </tr>
    </tbody>
</table>

<h3>Список использованных источников</h3>
<ol>
    <li>https://soundbran.ch/2023/03/06/the-rise-of-voice-notes-20-statistics/</li>
    <li>https://verloop.io/blog/whatsapp-statistics-2024</li>
    <li>https://www.cooby.co/en/post/whatsapp-statistics</li>
</ol>

<h2>ДЗ3</h2>

<h3>Функциональное разбиение по доменам</h3>

<ul>
    <li>auth - авторизация и аутентификация</li>
    <li>chat - чаты</li>
    <li>call - звонки</li>
</ul>

<h3>Обоснование расположения ДЦ</h3>
<p>Сервис имеет огромную аудиторию по всему миру, поэтому следует распределить ДЦ так, чтобы они покрывали все континенты, с фокусом на те страны, в которых находится наибольшее число пользователей. Для Северной Америки это США, для Южной Америки - Бразилия, для Европы - Германия (с высокой концентрацией и в других странах), для Азии - Индия (550 млн, наибольшая аудитория), для Африки - Нигерия. Также часть пользователей присутствует в Австралии и Океании. Если не иметь хотя бы одного ДЦ в каждом из этих регионов, то задержка для местных пользователей будет увеличена на десятки мс (вплоть до 100-150 мс) только из-за географического положения.</p>

<table>
    <thead>
        <th>Регион</th>
        <th>Города расположения ДЦ</th>
        <th>Обоснование</th>
    </thead>
    <tbody>
        <tr>
            <td>Европа</td>
            <td>Франкфурт, Лондон, Стокгольм, Варшава</td>
            <td>ДЦ в UK будет обслуживать западную Европу (включая Францию), ДЦ в Германии - Центральную Европу, Варшава - европейская часть РФ и Восточная Европа, Стокгольм - Скандинавия</td>
        </tr>
        <tr>
            <td>Азия</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Африка</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Северная Америка</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Южная Америка</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Австралия и Океания</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>

<h3>Расчет распределения запросов по типам запросов по датацентрам</h3>
<h3>Схема DNS балансировки</h3>

<p>Разумно будет использовать <b>GEO-based DNS</b> для определения IP балансировщика по регионам. Например, если есть 2 ДЦ, в Нью-Дели и в Мумбаи, то DNS определяет IP-адрес Anycast-балансировщика для региона Азия, который распределяет нагрузку по соответствующим ДЦ.</p>

<h3>Схема Anycast балансировки</h3>

<p>Используем Latency-based Anycast. После определения IP регионального балансировщика DNS балансировщик определяет ДЦ, до которого задержка минимальна, и роутит запрос в этот ДЦ.</p>
