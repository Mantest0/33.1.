Итоговый проект по автоматизации тестирования (PJ-04)

Выполнил: Антон QAP-171

Объект тестирования: https://b2c.passport.rt.ru.

Задача тестирования: протестировать обновлённые интерфейсы авторизации и регистрации в личном кабинете в соответствии с требованиями Заказчика Ростелеком Информационные Технологии.

Окружение: Windows10 (разрешение экрана (1366x768)) + Google Chrome 123.0.6312.106 (Официальная сборка), (64 бит)

IDE: PyCharm 2023.2.5 (Community Edition) — для написания и запуска тестов на Python

Kiwi TSMC - прикладная система управления обучениями для составления тест-кейсов и проведения тестирования.

Проект содержит:

Директорию тестов, включающую в себя файлы: 1.locators.py — локаторы веб-элементов на сайте, использовавшиеся в тестах;

2.test_authorization_rt.py — последние авторизации;

3.test_registration_rt.py — регистрация регистрации.

4.Файл test_data.py — файл с информацией, которая используется при проведении тестов.

5.Файл requirements.txt — в нём находятся обязательные для установки библиотеки.

6.Файл тест_кейсы.txt - с ссылкой на гугл диск с тест кейсами.

7.Файл Требования_SSO_для_тестирования.txt - c ссылкой на гугл диск с требованиями заказчика.

Для запуска тестов из каталогов в терминале PyCharm IDE необходимо настроить команду pytesttesting/tests.

Также тест можно запустить непосредственно через опцию «Выполнить» интерфейса PyCharm.

Инструменты, применяемые в тестировании:

1.Для тестирования сайта был использован инструмент Selenium;

2.Для определения и построения локаторов использовались инструменты DevTools, ChroPath.

Техники тест дизайна, используемые в работе над проектом:

1.Анализ граничных значений (в требованиях указаны ограничения по символам в

определенных полях - мы анализировали и тестировали значения на границах различных

диапазонов, чтобы убедиться, что система правильно обрабатывает крайние ситуации)

2.Предупреждения об ошибках (при потенциальной ошибке пользователя при вводе данных)

3.Эквивалентное разбиение (мы разделяли входные данные по группам наследственных результатов,

чтобы протестировать их представителей вместо каждого отдельного значения. Это ресурс

уменьшения количества испытаний, при этом сохраняя полное покрытие)

Эти методы помогли нам провести тесты, которые расширили обширное покрытие функциональности объекта и выявили потенциальные проблемы.

Дефекты, обнаруженные в ходе тестирования, добавлены в файл тест-кейсы и баг-репорты отдельной таблицей.
