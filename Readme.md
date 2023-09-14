Вритуальная стажировка PDEV-25 Требуется разработать методы запроса и создания обьектов. 
Краткий пересказ. ФСТР — организация, занимающаяся развитием и популяризацией спортивного
туризма в России и руководящая проведением всероссийских соревнований в этом виде спорта. 
На сайте https://pereval.online/ ФСТР ведёт базу горных перевалов, которая пополняется туристами. 
После преодоления очередного перевала, турист заполняет отчёт в формате PDF и отправляет
его на электронную почту федерации. Экспертная группа ФСТР получает эту информацию, верифицирует,
а затем вносит её в базу, которая ведётся в Google-таблице. ФСТР заказала разработать мобильное
приложение для Android и IOS, которое упростило бы туристам задачу по отправке данных о перевале
и сократило время обработки запроса до трёх дней. Пользоваться мобильным приложением будут туристы.
В горах они будут вносить данные о перевале в приложение и отправлять их в ФСТР, как только появится
доступ в Интернет. Модератор из федерации будет верифицировать и вносить в базу данных информацию,
полученную от пользователей, а те в свою очередь смогут увидеть в мобильном приложении статус
модерации и просматривать базу с объектами, внесёнными другими.

Пользователь с помощью мобильного приложения будет передавать в ФСТР следующие данные о перевале:

o координаты перевала и его высота;

o имя пользователя;

o почта и телефон пользователя;

o название перевала;

o несколько фотографий перевала.

Были реализованы методы REST APi в Django. Созданы модели Climber(скалолазы), PerevalAdded(перевалы), 
Category(категории перевалов применяемые во всём мире для градации горной местности в зависимости от времени года).
Это основные модели которые созданы для работы всего сайта. Иммено на них завязаны методы: Создания: - Новых пользователей
- Новых перевалов Поиск: - По Индивидуальному номеру(Id) - Поиск по почте добавившего перевал Также создан фаил
- для спецификации RESTful API. Swagger UI. База данных PostgerSQL все данные и пароли сохранены в файле ".env"