# Рекомендация тарифов 

### Описание проекта  
В вашем распоряжении данные о поведении клиентов, которые уже перешли на эти тарифы (из проекта курса «Статистический анализ данных»). Нужно построить модель для задачи классификации, которая выберет подходящий тариф. Предобработка данных не понадобится — вы её уже сделали.

Постройте модель с максимально большим значением *accuracy*. Чтобы сдать проект успешно, нужно довести долю правильных ответов по крайней мере до 0.75. Проверьте *accuracy* на тестовой выборке самостоятельно.

### Описание данных  
Каждый объект в наборе данных — это информация о поведении одного  
пользователя за месяц. Известно:  
`сalls` — количество звонков,  
`minutes` — суммарная длительность звонков в минутах,  
`messages` — количество sms-сообщений,  
`mb_used` — израсходованный интернет-трафик в Мб,  
`is_ultra` — каким тарифом пользовался в течение месяца ("Ультра" — 1, "Смарт" — 0).  

### В ходе исследования было выполнено:  
- разделение данных на обучающую и тестовую выборки;
- сравнение трёх моделей (критерий - `accuracy`): решающего дерева, случайного леса и логистической регрессии;
- проверка на адекватность модели.

### С точки зрения метрики `accuracy` алгоритмы расположились в следующем порядке:  
1. Случайный лес (0.81).  
2. Решающее дерево (0.8).  
3. Логистическая регрессия (менее 0.75).
