[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&vCenter=true&width=435&lines=Breast+Cancer+Wisconsin+(Diagnostic))](https://git.io/typing-svg)
![](https://storage.googleapis.com/kaggle-datasets-images/180/384/3da2510581f9d3b902307ff8d06fe327/dataset-cover.jpg)

# О наборе данных
Характеристики рассчитываются по оцифрованному изображению тонкоигольной аспирации (ТАБ) массы молочной железы. Они описывают характеристики ядер клеток, присутствующих на изображении.
n трехмерное пространство описано в: [К.П. Беннетт и О.Л. Мангасарян: "Надежное линейное программирование различения двух линейно неразделимых множеств", Методы оптимизации и программное обеспечение, 1, 1992, 23-34].

Эта база данных также доступна через ftp-сервер UW CS:
ftp ftp.cs.wisc.edu
cd math-prog/cpo-dataset/machine-learn/WDBC/

Также можно найти в репозитории машинного обучения UCI: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

##  Информация об атрибутах:

- Идентификационный номер
- Диагноз (М = злокачественное, В = доброкачественное)


##### Для каждого клеточного ядра вычисляются десять вещественных признаков:

- радиус (среднее значение расстояний от центра до точек на периметре)
- текстура (стандартное отклонение значений шкалы серого)
- периметр
- площадь
- гладкость (локальное изменение длины радиуса)
- компактность (периметр^2 / площадь - 1,0)
- вогнутость (выраженность вогнутых участков контура)
- вогнутость точек (количество вогнутых участков контура)
- симметричность и фрактальная размерность ("приближение береговой линии" - 1)

Среднее значение, стандартная ошибка и «наихудшее» или наибольшее (среднее значение трех
самых больших значений) этих признаков были вычислены для каждого изображения,
в результате чего было получено 30 признаков. Например, поле 3 — это средний радиус, поле
13 — юго-восточный радиус, поле 23 — наихудший радиус.

Все значения признаков перекодируются четырьмя значащими цифрами.
Отсутствующие значения атрибута: none
Распределение по классам: 357 доброкачественных, 212 злокачественных

## Работу выполнили:
- Пантюхин Роман, группа 11-008
- Капралов Александр, группа 11-008

## Ссылка на датасет:
[Breast Cancer Wisconsin](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

## Используемые алгоритмы:
- Logistic Regression
- Hist Gradient Boosting
- Random Forest
- Ada Boost
- XGBoost
- LightGBM
- Decision Tree
- KNeighbors
- СatBoost

## Результаты:
![](https://sun9-46.userapi.com/impg/4U3a6tpjXTV4tdX3k1jmMOa_wlQpvhy-004jIQ/0m6a2KI08T8.jpg?size=1027x575&quality=96&sign=8ac0246fc11e58c0d109526baa014f7d&type=album)
#### Как видим - CatBoost, LightGBM, AdaBoost показали лучший результат
