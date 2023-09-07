### Прогноз заказов такси
####  Цель проекта: Сокращение времени подачи и простоя такси.
####  Задача проекта: Требуется спрогнозировать количество заказов такси на следующий час в аэропорт, чтобы привлекать необходимое количество водителей в периоды пиковой нагрузки.

*Инструменты:* 
- *python*
- *pandas*
- *numpy*
- *statsmodels.tsa.seasonal.seasonal_decompose*
- *sklearn.model_selection.TimeSeriesSplit*
- *sklearn.model_selection.GridSearchCV*
- *sklearn.metrics.mean_squared_error*
- *sklearn.metrics.make_scorer*
- *sklearn.linear_model.LinearRegression*
- *sklearn.ensemble.RandomForestRegressor*
- *catboost.CatBoostRegressor*
- *matplotlib*

#### Описание проекта
Разработанная модель предсказывает коэффициент восстановления золота из золотосодержащей руды. Для расчётов использовались данные АСУТП за 2.5 года работы золоторудного комбината. В данном проекте протестированы четыре типовые модели с кросс-валидацией:
> - `RandomForestRegressor`,
> - `DecisionTreeRegressor`,
> - `LinearRegression` и
> - `CatBoostRegressor`

#### Общий вывод
Проведено исследование временного ряда на предмет трендовых и сезонных закономерностей, случайной составляющей. Проведено исследование трёх типов моделей, выбрана линейная регрессия.
