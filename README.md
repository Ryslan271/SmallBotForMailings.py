# Бот для отправки сообщений выбранным пользователям 
Бот сохраняет отправленные сообщения и ники пользователей 
Сохранение происходит в локальном файле SQLite, пока что стоит задача отправить сообщение пользователям по никам, но данная проблема довольно серьзно меняшает доделать проект

Проблема с отправкой данных 
--------
По идеи отправка сообщений должна производиться по chat_id но достать его нельзя, если пользователь сам ранее не вошел в систему и придется сохранять все id всех пользователей, что уже негативно сказывается на безопастности проекта и данных пользователей 
Данная проблема возникает из за политики телеграмма, он запрещает отправку сообщений по никам или как пишется в коде username, каждый диалог использует chat_id, для отправки сообщений нужному пользователю, данный id можно получить только в прямой переписки с пользователем, из за чего и возникает проблема

Решение
-------

Решение есть, но смутное, https://github.com/vysheng/tg/ библиотека позволяет работать с терминалом телеграмма на прямую, но сама библиотека уже не поддерживается и придется дорабатывать её для своих целей 
