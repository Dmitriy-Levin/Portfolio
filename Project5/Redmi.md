### Анализ текстов
####  Цель проекта:   Дать возможность пользователям редактировать и дополнять описания товаров, как в вики-сообществах.
####  Задача проекта:   Требуется создать программу, которая будет искать токсичные комментарии и отправлять их на модерацию.

#### *Инструменты:* 
|  |  |
| :---         |     :---     |
|*python*|*sklearn.linear_model.LinearRegression*|
|*pandas*|*sklearn.model_selection.cross_val_score*|
|*numpy*|*sklearn.model_selection.train_test_split*|
|*torch*|*sklearn.metrics.accuracy_score*|
|*torch.LongTensor*|*transformers.BertTokenizer*|
|*tqdm*|*transformers.BertModel*|

#### Описание проекта

1. Интернет-магазин запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Необходимо обучить модель классифицировать комментарии на позитивные и негативные. В нашем распоряжении набор данных с разметкой о токсичности правок. Требуется разработать модель со значением метрики качества F1 не меньше 0.75.

2. Был проделан следующий объём работ:
    - Данные:
        - загружены,
        - исследованы и
        - оптимизированы.

    - Провели предобучение - модель `DeepPavlov/rubert-base-cased`;

    - Выполнили токенизацию инструментом `BertTokenizer()` и;

    - Эмбеддинг.

3. Полученная модель показала существенно лучший результат `f1 = 0.95`, чем заданное заказчиком значение 0,75.
4. Для производства выбрана модель `LinearRegression`.

