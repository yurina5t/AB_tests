# AA и AB тесты
Проведены A/A и A/B тесты по новым алгоритмам рекомендации постов

__[1.Проведен А/А тест с 23 июля 2023 по 29 июля 2023 года.](https://github.com/yurina5t/AB_tests/blob/main/AA_test_CTR.ipynb)__   
У нас есть данные А/А-теста с '2023-07-23' по '2023-07-29'. Нам нужно сделать симуляцию, как будто мы провели 10000 А/А-тестов. На каждой итерации нужно сформировать подвыборки без повторения в 500 юзеров из 2 и 3 экспериментальной группы. Провести сравнение этих подвыборок t-testом.

1. Построить гистограмму распределения получившихся 10000 p-values.   
2. Посчитать, какой процент p values оказался меньше либо равен 0.05.   
3. Написать вывод по проведенному А/А-тесту, корректно ли работает наша система сплитования.   

__[2. Проведен А/В тест на данных с 30 июля 2023 по 5 августа 2023 года по метрике CTR](https://github.com/yurina5t/AB_tests/blob/main/AB_test_CTR.ipynb)__   
Задача — проанализировать данные А/B-теста.

1. Выбрать метод анализа и сравнить CTR в двух группах (мы разбирали t-тест, Пуассоновский бутстреп, тест Манна-Уитни, t-тест на сглаженном ctr (α=5) а также t-тест и тест Манна-Уитни поверхного преобразования).   
2. Сравнить данные этими тестами. А еще посмотреть на распределения глазами. Почему тесты сработали именно так?    
3. Описать потенциальную ситуацию, когда такое изменение могло произойти. Тут нет идеального ответа.   
4. Написать рекомендацию, будем ли мы раскатывать новый алгоритм на всех новых пользователей или все-таки не стоит.   

__[3. Выполнен А/В тест с 30 июля 2023 по 5 августа 2023 года по метрике линеаризованных лайков](https://github.com/yurina5t/AB_tests/blob/main/AB_test_linearized_likes.ipynb)__   

1. Проанализировать тест между группами 0 и 3 по метрике линеаризованных лайков. Видно ли отличие? Стало ли 𝑝−𝑣𝑎𝑙𝑢𝑒 меньше?   
2. Проанализировать тест между группами 1 и 2 по метрике линеаризованных лайков. Видно ли отличие? Стало ли 𝑝−𝑣𝑎𝑙𝑢𝑒 меньше?



Данные для анализа предоставлены @lab.karpov.courses
