# Простое тестовое задание

### Введение
Предположим, есть данные, а именно собранная хроматограмма, которая хранится в CSV-файле (файл в репозитории scout_ph_7.75.csv)
Устроена она следующим образом: столбцы, имеющие постфикс "_time" -- это временная ось, а столбцы, имеющие другой постфикс -- это амплитуда сигнала. 
Время и амплитуду объединяет общий корень, название метрики. 
Например: 
* UV1 (215 nm)_time -- время для метрики UV-датчика UV1 (215 nm)
* UV1 (215 nm)_mAU -- амплитуда сигнала метрики UV-датчика UV1 (215 nm)

### Задание
Необходимо собрать страницу, содержащую график этих метрик и легенду для этого графика.

В легенде нужно будет вывести:
- названия метрик
- минимумы и максимумы амплитуд метрик

В легенде нужно реализовать следующие функции:
- реализовать возможность задавать цвет (меняю цвет в легенде, соответствующая метрика на графике тоже меняет цвет)
- и включать/выключать видимость (нажимаю на иконку видимости в легенде, соответствущая метрика на графике исчезает/появялется)

В графике:
- при наведении мыши мы видим значения амплитуд метрик
- в качестве подписей и шкал к осям данных можно вывести любую метрику, например первую

### Ограничения
Реализовать необходимо в следующем стеке:
- TypeScript
- Feature Sliced
- Effector
- написать хотя бы пару unit-тестов в любом удобном фреймворке
