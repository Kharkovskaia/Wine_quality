Структура проекта:
1. README.md – общее описание проекта;
2. sturktura.md – информация о структуре проекта;
3. data – содержит данные:
- external – исходные данные, взяты с https://www.kaggle.com/rajyellow46/wine-quality; 
- intermid – промежуточные результаты (указаны в порядке получения):   
data_categ.csv – преобразованы категориальные признаки в числовые переменные;   
no_passes.csv – заполнены пропуски;   
new_values.csv – с новыми признаками;   
- processe – финальные датасеты для обучения модели;
4. models – содержит используемые модели:
- LogisticRegression.pkl – модель логистической регрессии;
- DecisionTreeClassifier.pkl – дерево решений;
- stacking_model.pkl – стекинг моделей Decision Tree Classifier, Linear SVC, KNeighbors Classifier. Для объединения базовых оценок использована модель Logistic Regression;
5. reports – содержит отчёт по проведённому исследованию;
6. scripts – содержит вспомогательные Python-скрипты:
- plot_script – содержит функции для визуализации данных:   
def plot_distribution( df , var , target , **kwargs ) – функция для рассмотрения взаимосвязи между признаками и качеством вина;   
def plot_correlation_map( df ) – функция для построения тепловой карты корреляции;   
def plot_variable_importance( X , y )- функция для определения важности признаков;   
7. notebooks - содержит JupyterNotebook.
