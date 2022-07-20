# 1. Цель проекта

Цель проекта - разработать игровую систему для игры в "ЧТО? ГДЕ? КОГДА?" (далее Игра).
Команда до 8 человек может сразиться со зрительсим набором вопросов по правилам телепередачи.

# 2. Описание игры

Игра состоит из следующих основных компонентов: 

1. Аутентификация пользователя
2. Функционал для ведущего
3. Функционал для знатока
4. Функционал для зрителя
5. Функционал для капитана
6. Функционал игрового стола

# 2.1. Типы пользователей

Игра предусматривает особый функционал для каждого типа пользователя: 
ведущий (хост) зачитывает вопросы, крутит волчок и отвечает за настройку игры и принятие ответов; игроки (в том числе капитан) отвечают на вопросы ведущего; зрители не могут взаимодействовать с игрой и только наблюдают. При настройке комнаты пользователи могут меняться ролями (кроме ведущего).

# 2.2 Аутентификация

Процесс аутентификации выглядит слеюущим образом:
1. При первом посещении сайта пользователю предлагают ввести его Имя.
2. При последующем посещении сайта вводить Имя не требуется.

# 2.4. Функционал для ведущего

1. Изменение состояния стола
2. Выбор пака вопросов
3. Пуск кручения волчка
4. Запуск таймера ответа на вопрос
5. Запуск процедуры досрочного ответа
6. Приниятие и непринятие ответа
7. Взаимодействие со знатоками

# 2.4.1 Состояние стола

У стола существует 2 состояния:

* Открытый
* Закрытый

При открытом столе пользователи (кроме ведущего) могут менять свою роль
При закрытом столе все новые пользователи получают роль зрителя

# 2.4.2 Выбор пака вопросов

В настройках стола Ведущему предоставляется поле, в которое он может вписать id пака вопросов, взятое с сайта https://db.chgk.info/

# 2.4.3 Волчок

На игровом поле находится кнопка, которая запускает волчок, под окончание вращения которого Ведущему будет предоставлен сам вопрос в модальном окне

# 2.4.4 Таймер ответа

Ведущий после прочтения вопроса запускает таймер, по истечению которого команда должна выбрать игрока, который выдаст ответ на вопрос. 
