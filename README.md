# TaskControl

# Задача :
Написать программу, которая из имеющегося массива строк формирует массив из строк,
длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры,
либо задать на старте выполнения алгоритма. При решение не рекомендуется пользоваться коллекциями,
лучше обойтись исключительно массивами.

# Описание алгоритма решения:

- Объявляем 2 массива- начальный и второй равный длине начального массива.
- Затем создаем метод в котором есть переменная temp и 2 цикла(цикл в цикле):
В 1м цикле перебираем всю длину массива(все элементы)
В 2м цикле проверяем условие(если длина элемента массива <=3 символов), то элемент  
изначального массива записывается в temp элемент 2го массива.
Переменная temp нужна,чтобы по очереди из начального массива переписывать элементы
(подходящие под условие <=3) во второй массив.
После temp увеличиваем на 1 и возвращаемся к 1му циклу,где i увеличиваем на 1
(т.е. проверяем следующий элемент массива).
Если условие( <=3 ) 2го цикла не соблюдается, то возвращаемся к 1му циклу и увеличиваем i на 1.
И так пока не пройдем всю длину массива(array.Length).
- Выводим на печать массив.

- Графическая блок-схема метода в файле Scheme.jpg
- Реализация алгоритма по пути TaskControl/Program.cs