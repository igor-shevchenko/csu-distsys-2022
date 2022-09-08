# Проектирование и разработка распределенных программных систем

Лекции и материалы по курсу распределенных систем в ЧелГУ, группа ПрИ-401.

## Лекции

### Лекция 1. Введение в распределенные системы

[Презентация](https://docs.google.com/presentation/d/1d2pypUKNwUruZWbsXhp2ydwMtSnNiuLSP4XickQO7UI/edit?usp=sharing)

Зачем нужны распределенные системы, какие проблемы они решают и какие проблемы в них появляются.

**Ссылки**
1. Мартин Клеппман. Высоконагруженные приложения. Программирование, масштабирование, поддержка
2. [Лекции Мартина Клеппмана по распределенным системам в Кембридже](https://martin.kleppmann.com/2020/11/18/distributed-systems-and-elliptic-curves.html)
3. [Distributed systems for fun and profit](http://book.mixu.net/distsys/)
4. [Страх и ненависть в распределённых системах](https://habr.com/ru/post/322876/)


### Лекция 2. Асинхронное программирование

[Презентация](https://docs.google.com/presentation/d/1LyIN79I1kte8UCAIXgRT97FxYXcyBP8t1zyyXFWENeE/edit?usp=sharing)

**Ссылки**
1. [Highload++ для начинающих](http://highload.guide/blog/highload-for-beginners.html)
2. [Анатомия веб-сервиса](http://highload.guide/blog/inside-webserver.html)
3. [Метафоры асинхронности в документации FastAPI](https://fastapi.tiangolo.com/async/)
4. [Асинхронщина в JS](https://habr.com/ru/company/oleg-bunin/blog/417461/)


### Лекция 3. Модели данных

[Презентация](https://docs.google.com/presentation/d/1q0-Z29QHd4PduiZTWnEQ88wT_1nT0yT4iBUcfCrDoiw/edit?usp=sharing)

Реляционные, документоориентированные, графовые, key-value и колоночные БД.

**Ссылки**
1. [NoSQL – коротко о главном](https://habr.com/ru/company/oleg-bunin/blog/319052/)
2. Мартин Клеппман. Высоконагруженные приложения. Программирование, масштабирование, поддержка. Глава 2
3. [CQRS documents](https://cqrs.files.wordpress.com/2010/11/cqrs_documents.pdf)


### Лекция 4. Коммуникация приложений

[Презентация](https://docs.google.com/presentation/d/1v1GFzivKFbnHxZFLRuftByF8O1mXzlv-zTKSVPOBA74/edit?usp=sharing)

**Ссылки**
1. Хоп Грегор, Вульф Бобби. Шаблоны интеграции корпоративных приложений
2. Сэм Ньюмен. Создание микросервисов, глава 4


### Лекция 5. Очереди сообщений

[Презентация](https://docs.google.com/presentation/d/1q7dW0Si8dbH9q910DcA7xcTA9U4dT4lb4eC_alZZFO0/edit?usp=sharing)

**Ссылки**
1. [Принципы и приёмы обработки очередей](https://habr.com/ru/company/oleg-bunin/blog/309332/)
2. [101 способ приготовления RabbitMQ и немного о pipeline архитектуре](https://habr.com/ru/company/oleg-bunin/blog/310418/)
3. [Очереди и блокировки. Теория и практика](https://habr.com/ru/company/oleg-bunin/blog/316458/)


### Лекция 6. Горизонтальное масштабирование

[Презентация](https://docs.google.com/presentation/d/1iBqPaXz9J1fr0pV8yAb-W_WCdcc9YoVxtw4r4NC4mIs/edit?usp=sharing)

**Ссылки**
1. [Общая логика масштабирования](http://highload.guide/blog/scaling-logic.html)
2. [Масштабирование бэкенда](https://xakep.ru/2012/11/30/backend-zoom/)
3. [Горизонтальное масштабирование. Что, зачем, когда и как](http://highload.guide/blog/scaling-what-why-when-and-how.html)
4. [Как мы сделали ровную балансировку нагрузки на фронтенд-кластере](http://highload.guide/blog/load-balancing-frontend-cluster.html)


### Лекция 7. Кэширование

[Презентация](https://docs.google.com/presentation/d/1T2idapTFR93Rj9joDxU07z7wXLdUOnDIBAzPKNOEWSI/edit?usp=sharing)

**Ссылки**
1. [Web, кэширование и memcached](http://highload.guide/blog/web-caching-memcached.html)
2. [Кэширование данных в web приложениях. Использование memcached](http://highload.guide/blog/caching-data-in-web-applications.html)
3. [Использование memcached и Redis в высоконагруженных проектах](http://highload.guide/blog/using-memcached-and-redis.html)


### Лекция 8. Масштабирование БД

[Презентация](https://docs.google.com/presentation/d/1ijCzq1pHHi8TDrvTigNDqTnMDJx6Rl-pp38e_Sf_Vms/edit?usp=sharing)

**Ссылки**
1. Мартин Клеппман. Высоконагруженные приложения. Программирование, масштабирование, поддержка. Главы 5, 6
2. [Шардинг: паттерны и антипаттерны](https://habr.com/ru/company/oleg-bunin/blog/313366/)


## Практика

### Практика 1. Контейнеризация и Docker

![](diagrams/lab1.png)

[Презентация](https://docs.google.com/presentation/d/1LZIROK9qOy4_B01JgWftwZYblGwm4UZ-izBq5nZacHM/edit?usp=sharing)

**Задание**
1. Написать  веб-сервер, который принимает HTTP-запрос и отдает ответ «Hello world»
2. Установить Docker
3. Написать Dockerfile и запустить веб-сервер в докер-контейнере так, чтобы к нему можно было обратиться с хост-машины

**Ссылки**
1. [Установка Docker](https://docs.docker.com/get-docker/)
2. [Документация по Docker](https://docs.docker.com/get-started/)
3. [Документация по Dockerfile](https://docs.docker.com/engine/reference/builder/)
4. [Порядок команд в Dockerfile](https://medium.com/@esotericmeans/optimizing-your-dockerfile-dc4b7b527756)
5. [Multi-stage builds для компилируемых языков](https://docs.docker.com/develop/develop-images/multistage-build/)


## Итоговая оценка
 
### Баллы за практические задачи

| Дата сдачи  | Docker | БД | RabbitMQ | nginx | Redis |
|-------------|--------|----|----------|-------|-------|
|  8 сентября |      - |  - |        - |     - |     - |
| 15 сентября |     20 |  - |        - |     - |     - |
| 22 сентября |     20 | 20 |        - |     - |     - |
| 29 сентября |     20 | 20 |       20 |     - |     - |
|   6 октября |     20 | 20 |       20 |    20 |     - |
|  13 октября |     20 | 20 |       20 |    20 |    20 |
|  20 октября |     20 | 20 |       20 |    20 |    20 |
|  27 октября |     15 | 20 |       20 |    20 |    20 |
|    3 ноября |     15 | 15 |       20 |    20 |    20 |
|   10 ноября |     10 | 15 |       15 |    20 |    20 |
|   17 ноября |     10 | 10 |       15 |    15 |    20 |
|   24 ноября |      5 | 10 |       15 |    15 |    15 |
|   1 декабря |      5 | 10 |       15 |    15 |    15 |
|   8 декабря |      5 | 10 |       10 |    15 |    15 |
|  15 декабря |      5 |  5 |       10 |    15 |    15 |
|  22 декабря |      5 |  5 |        5 |    10 |    15 |
|  29 декабря |      5 |  5 |        5 |    10 |    15 |
 
Все практики сданы: **+100**
 
### Перевод баллов в оценку
 
| От  | До  | Оценка |
|-----|-----|--------|
| 140 | 160 |  **3** |
| 165 | 180 |  **4** |
| 185 | 200 |  **5** |
