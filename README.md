
# Задание
[Описание задания](https://netology.ru/profile/program/job-tz-prog-pd-4/lessons/401964/lesson_items/2175029)



Условие

Необходимо реализовать Python-библиотеку, которая осуществляет получение квадратной матрицы (NxN) с удалённого сервера и возвращает её пользователю в виде List[int]. 

Этот список должен содержать результат обхода полученной матрицы по спирали: против часовой стрелки, начиная с левого верхнего угла (см. test case ниже).

Пример исходной матрицы:

![image](https://github.com/user-attachments/assets/970a6634-ef58-4c0b-b13b-803b79397dfc)


Матрица гарантированно содержит целые неотрицательные числа. Форматирование границ иными символами не предполагается.

# Требования к выполнению и оформлению

Библиотека содержит функцию со следующим интерфейсом:

async def get_matrix(url: str) -> List[int]:

● …
● Функция единственным аргументом получает URL для загрузки матрицы с сервера по протоколу HTTP(S)

● Функция возвращает список, содержащий результат обхода полученной матрицы по спирали: против часовой стрелки, начиная с левого верхнего угла

● Взаимодействие с сервером должно быть реализовано асинхронно - посредством aiohttp, httpx или другого компонента на asyncio

● Библиотека должна корректно обрабатывать ошибки сервера и сетевые ошибки (5xx, Connection Timeout, Connection Refused, …)

● В дальнейшем размерность матрицы может быть изменена с сохранением форматирования. Библиотека должна сохранить свою работоспособность на квадратных матрицах другой размерности

● Решение задачи необходимо разместить на одном из публичных git-хостингов (GitHub, GitLab, Bitbucket). Можно также выслать решение в виде архива (zip, tar). Загружать библиотеку в PyPi или другие репозитории не требуется

# Проверка решения


![image](https://github.com/user-attachments/assets/01651cca-27ca-4b72-be42-30e8e02f4f05)


При проверке мы также будем обращать внимание на тесты, type hints, структуру решения и общее качество кода.
Удачи в выполнении задачи и не забывайте о The Zen of Python! :)
