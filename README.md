# Alfa-x-FinU-Hack
Хакатон от Альфа-Банка и Финансового университета
https://drive.google.com/drive/folders/1FcrwPInxpXKMH6TZI6KKU4L-o0hp_23F?usp=sharing - файлы

# Проблематика
Модель CLTV позволяет определять ценность клиента для Банка на всем периоде взаимодействия клиента с Банком.
В качестве показателя ценности клиента используется операционная прибыль - сумма всех доходных и расходных операций.
Основной характеристикой клиента, влияющей на его прибыльность, является набор продуктов (продуктовый кластер), которыми клиент активно пользуется, то есть генерирует операционную прибыль.

При изменении кластера клиента, например, при открытии нового продукта или закрытии существующего, у него существенным образом меняется профиль доходности.

Поэтому ядром модели CLTV будет являться модель, которая предсказывает переход клиента из одного продуктового кластера во все возможные кластеры на некотором горизонте прогнозирования.

# Задача
Построить модель, которая будет предсказывать продуктовый кластер клиента - Юридического лица на горизонте в 12 месяцев.

Для анализа и построения модели выбран тренировочный датасет, содержащий данные о 200 000 клиентах банка и их целевых переменных за три последовательных месяца (month_1, month_2, month_3).

Для оценивания работы модели дан тестовый набор данных о 100 000 клиентах, аналогично, за 3 последовательных месяца (month_4, month_5, month_6).

Целевой переменной является продуктовый кластер, в котором клиент будет находится через год. В задаче будут рассматриваться 17 продуктовых кластеров. Нужно получить вероятности перехода клиента в продуктовые кластеры для последнего месяца (month_6).
