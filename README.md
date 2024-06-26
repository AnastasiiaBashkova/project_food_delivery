### Анализ продуктовых метрик (доставка продуктов на дом)

Задачи:

1. Проанализировать поведение пользователей в конце квартала
2. Оценить эффективность каналов привлечения пользователей

<hr>

Работа выполнена на Python с использованием Jupyter Notebook

<hr>

Реализация проекта:
1. Предобработала имеющиеся данные
2. Вычислила месячную аудиторию (MAU)
3. Определила количество установок приложения
4. Присвоила пользователям когорты по дню установки приложения и посчитала для них конверсию (CR) из установки в покупку в течение 7 дней. Определила для какой когорты конверсия была наибольшей. (Примечание: считаем пользователя сконвертировавшимся, если с момента установки до совершения первой покупки прошло не более 7 дней)
5. Определила с какого платного маркетингового канала пришло больше всего новых пользователей
6. Выделила группу тех, кому нужно и не нужно регистрироваться (если дата регистрации < даты совершения события, то пользователь уже зарегистрирован)
7. Проанализировала на каком этапе воронки отваливается бОльшая часть клиентов
8. Так же проанализровала на каком этапе отваливается больше всего зарегистрированных пользователей
9. Определила канал, с которого пользователи показали самую низкую конверсию в первую покупку
10. Определила канал, с которого пользователи имеют медианный первый чек выше (учитывала только первые покупки пользователей)
11. Рассчитала ROMI для каждого платного канала привлечения (для рассчета использовала дополнительные данные о затратах на рекламу)
    Данные по затратам на рекламу:
    Яндекс – 10 491 707 руб.
    Гугл – 10 534 878 руб.
    Фейсбук – 8 590 498 руб.
    Инстаграм – 8 561626 руб.
    ВК – 9 553 531руб.
    Расходы на реферальную программу: если пользователь приведет друга и последний совершит первую покупку, то оба получат по 100 рублей.
<hr>

Дополнительная информация:

1. В выгрузке только уникальные действия пользователей за каждый день 
2. Можно миновать стадию установки приложения, если оно было установлено ранее
3. Можно миновать стадию регистрации, если пользователь был уже залогинен на момент сессии. Однако незарегистрированные пользователи не могут оформить покупку
