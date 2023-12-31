# Предсказание коэффициента восстановления золота из золотосодержащей руды

## Инструменты и библиотеки:
![Python](https://img.shields.io/badge/-Python-white?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/-Pandas-white?style=flat&logo=pandas&logoColor=130754)
![seaborn](https://img.shields.io/badge/-seaborn-white?style=flat&logo=seaborn)
![matplotlib](https://img.shields.io/badge/-matplotlib-white?style=flat&logo=matplotlib)
![NumPy](https://img.shields.io/badge/-NumPy-white?style=flat&logo=NumPy&logoColor=3366C5)
![scikit-learn](https://img.shields.io/badge/-scikit-white?style=flat&logo=scikit-learn)
## Описание проекта:
Компания «Цифры» разрабатывает решения для эффективной работы промышленных предприятий.

**Задача исследования** — Спрогнозировать концентрацию золота при проведении процесса очистки золота.

Строитстся модель машинного обучения для промышленной компании, разрабатывающая решения для эффективной работы промышленных предприятий. Модель должна предсказать коэффициент восстановления золота из золотосодержащей руды на основе данных с параметрами добычи и очистки. Модель поможет оптимизировать производство, чтобы не запускать предприятие с убыточными характеристиками.

## Выводы:
В результате исследования была проведена предобработка данных методом merge() недостающие колонки в тестовом и обучающем датафрейме были заполнены из полного датафрейма, методом ffill() были заполнены пропуски в данных.
Далее было проанализирована концентрация золота на каждом этапе очистики, оказалось что концентрация золота увеличивается от этапа к этапу.
После выяснилось, что распределение размеров гранул на обучающей и тестовой выборках примерно равно.
Затем была надена и обучена оптимальная модель (RandomForestRegressor(max_depth=5, n_estimators=55, random_state=12345)).
В итоге вычеслено финальное smape (8.926165595106212), что говорит о неплохом результате, также успешно проведена проверка на адекватность моделью Dummy Regressor() .
