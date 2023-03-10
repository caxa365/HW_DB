Домашнее задание к лекции «Проектирование БД. Связи. 3НФ»
Задание 1
Обязательная часть

Будем развивать схему для музыкального сервиса.

Ранее было ограничение, что каждый исполнитель поет строго в одном жанре - пора убрать это ограничение. Исполнители могут петь в разных жанрах, как и одному жанру могут принадлежать несколько исполнителей.

Аналогичное ограничение было и с альбомами у исполнителей (альбом мог выпустить только один исполнитель). Теперь альбом могут выпустить несколько исполнителей вместе. Как и исполнитель может принимать участие во множестве альбомов.

С треками ничего не меняем, все так же трек принадлежит строго одному альбому.

Но появилась новая сущность - сборник. Сборник имеет название и год выпуска. В него входят различные треки из разных альбомов.

Обратите внимание: один и тот же трек может присутствовать в разных сборниках.

Задание состоит из двух частей:

Спроектировать и нарисовать схему (как в первой домашней работе. Прислать изображение со схемой.
Написать SQL-запросы, создающие спроектированную БД как во второй домашней работе. Прислать ссылку на файл, содержащий SQL-запросы.
Примечание: можно прислать сначала схему, получить подтверждение, что схема верная и после этого браться за написание запросов.

Домашнее задание к лекции «Select-запросы, выборки из одной таблицы»
Задание 1
Заполните базу данных из предыдущего домашнего задания. В ней должно быть:

не менее 8 исполнителей;
не менее 5 жанров;
не менее 8 альбомов;
не менее 15 треков;
не менее 8 сборников.
Внимание! Должны быть заполнены все поля каждой таблицы, в т.ч. таблицы связей (исполнителей с жанрами, исполнителей с альбомами, сборников с треками).

Задание 2
Написать SELECT-запросы, которые выведут информацию согласно инструкциям ниже. Внимание! Результаты запросов не должны быть пустыми (учтите при заполнении таблиц).

название и год выхода альбомов, вышедших в 2018 году;
название и продолжительность самого длительного трека;
название треков, продолжительность которых не менее 3,5 минуты;
названия сборников, вышедших в период с 2018 по 2020 год включительно;
исполнители, чье имя состоит из 1 слова;
название треков, которые содержат слово "мой"/"my".
Результатом работы будет 3 файла (с INSERT, SELECT запросами и CREATE запросами из предыдущего задания) в формате .sql (или .py/.ipynb, если вы будете писать запросы с использованием SQLAlchemy).

Домашнее задание к лекции «Группировки, выборки из нескольких таблиц»
Задание 1
Написать SELECT-запросы, которые выведут информацию согласно инструкциям ниже. Внимание! Результаты запросов не должны быть пустыми (при необходимости добавьте данные в таблицы).

количество исполнителей в каждом жанре;
количество треков, вошедших в альбомы 2019-2020 годов;
средняя продолжительность треков по каждому альбому;
все исполнители, которые не выпустили альбомы в 2020 году;
названия сборников, в которых присутствует конкретный исполнитель (выберите сами);
название альбомов, в которых присутствуют исполнители более 1 жанра;
наименование треков, которые не входят в сборники;
исполнителя(-ей), написавшего самый короткий по продолжительности трек (теоретически таких треков может быть несколько);
название альбомов, содержащих наименьшее количество треков.
Результатом работы будет 3 файла (с INSERT, SELECT запросами и CREATE запросами из предыдущего задания) в формате .sql (или .py/.ipynb, если вы будете писать запросы с использованием SQLAlchemy). В случае если INSERT- и CREATE-запросы остались без изменений, приложите файлы c ними из предыдущих домашних заданий.
