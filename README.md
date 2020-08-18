# skillfactory_rds-module_5.-Recommender-systems

Суть кейса:
Вы работаете в крупной компании, занимающейся онлайн-ритейлом (розничными продажами в интернете).

Ваш работодатель хочет увеличить средний чек продаж. Вы знаете, что чем точнее рекомендовать нужный товар пользователю 
(в нашем случае, товар с более высоким средним чеком), тем выше вероятность покупки этого товара. Простая логика. Мы нашли золото!

В качестве входных данных - история оценок пользователя вместе с его отзывом на товар. Все оценки пользователей нормированы для бинарной классификации: 
если человек поставил оценку продукту 4 и больше, то мы считаем, что продукт ему понравился, если меньше 4, то продукт не понравился.

На выходе получаем модель, которая предсказывает рейтинг товара. Так же с помощью полученных эмбеддингов можно получить наиболее подходящие товары к указанному.
Работа с данными и построение модели в base_notebook.ipynb

Streamlit
Так же присутствует User Interface (UI), сделанный через Streamlit. (см. app.py). Результат - result_streamlit.png. 
Пользователю предлагается ввести айди товара, который указан в исходном датасете. Интерфейс выдает ссылку на даныый товар и на 5 наиболее подходящих к нему.
