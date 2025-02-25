# Математические формулы
## Площадь
- Круга: S = πR²
- Прямоугольника: S = ab
- Квадрата: S = a²
- Треугольника: S = 1/2ah

## Периметр
- Круга: P = 2πR
- Прямоугольник: P = 2a + 2b
- Квадрата: P = 4a
- Треугольника: P = a + b + c
  
# Назначение проекта
Проект предназначен для вычисления периметров и площадей нескольких классов плоских геометрических фигур (многоугольников), таких как круг, квадрат, прямоугольник и треугольник, в декартовой системе координат.

# Механизм решения

## Привлечение сторонних материалов
Для реализации поставленной задачи были использованы формулы из элементарной геометрии для двумерных фигур, основанные на Евклидовой геометрии.

## Формат входных данных
Для обеспечения большей точности вычислений и возможности работы с нецелыми значениями каждая программа из данного проекта принимает на вход с консоли значения типа переменных с плавающей точкой (тип float) (при необходимости работы с целыми числами пользователю предлагается ввести натуральное число x в формате x, которое будет неявно преобразовано в int)

## Формат выходных данных
По окончании выполнения вычислений каждая программа возвращает результат также в виде чисел с плавающей точкой (в случае работы с целыми числами результат выводится в формате x.0)

# Описание каждой функции с примерами вызова

## Описание процесса работы программы circle.py
Содержимое программы circle.py выглядит следующим образом
```
import math


def area(r):
    '''
    Возвращает произведение математической константы и двух чисел с плавающей точкой в десятичной системе счисления.

        Параметры:
            r (float) : число с плавающей точкой в десятичной системе счисления

        Возвращаемое значение:
            (math.pi * r * r) (float) : число с плавающей точкой в десятичной системе счисления

            Пример вызова функции:
                area(10.5) = 346.36059005827474
    '''
    return math.pi * r * r


def perimeter(r):
    '''
        Возвращает произведение десятичной константы, математической константы и числа с плавающей точкой в десятичной системе счисления.

            Параметры:
                r (float) : число с плавающей точкой в десятичной системе счисления

            Возвращаемое значение:
                (2 * math.pi * r) (float) : число с плавающей точкой в десятичной системе счисления

                    Пример вызова функции:
                        perimeter(10.5) = 65.97344572538566

    '''
    return 2 * math.pi * r


print(
    'Введите значение радиуса круга в формате x, если это натуральное число, либо в формате x.y, где x — показатель целой части, y — показатель дробной части',
    '\n')
r = float(input())
print('Площадь круга равна', area(r), '\n')
print('Периметр круга равен', perimeter(r), '\n')
```

### Функция area(r)
* **Назначение:**
Возвращает произведение математической константы и двух чисел с плавающей точкой в десятичной системе счисления.

* **Параметры:**
r (float) : число с плавающей точкой в десятичной системе счисления.

* **Возвращаемое значение:**
(math.pi * r * r) (float) : число с плавающей точкой в десятичной системе счисления.

* **Пример вызова функции area(r):**
area(10.5) = 346.36059005827474


### Функция perimeter(r)
* **Назначение:**
* Возвращает произведение десятичной константы, математической константы и числа с плавающей точкой в десятичной системе счисления.

* **Параметры:**
* r (float) : число с плавающей точкой в десятичной системе счисления.

* **Возвращаемое значение:**
(2 * math.pi * r) (float) : число с плавающей точкой в десятичной системе счисления.

* **Пример вызова функции perimeter(r):**
perimeter(10.5) = 65.97344572538566


Программа хранит в памяти 1 переменную типа float — радиус круга.

Данная программа предназначена для вычисления площади и периметра круга по заданному пользователем радиусу.

Для успешного достижения поставленной задачи в программу circle.py был импортирован стандартный встроенный модуль math для получения значения π. 

Первый фрагмент программы — декларирование (объявление) функции area(r), которая получает на вход в качестве аргумента 1 число с плавающей точкой — значение радиуса круга, хранящееся в переменной r, отвечает за вычисление площади круга по формуле 
**$S = πr^2$**, где r — радиус круга, 
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции. 

Следующий фрагмент программы — декларирование (объявление) функции perimeter(r), которая получает на вход в качестве аргумента 1 число с плавающей точкой — значение радиуса круга, хранящееся в переменной r, отвечает за вычисление площади круга по формуле 
**$P = 2πr$**, где r — радиус круга,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции. 

В целях получения программой входных данных в консоль с помощью оператора print() выводится комментарий 'Введите значение радиуса круга в формате x, если это натуральное число, либо в формате x.y, где x — показатель целой части, y — показатель дробной части.'. Таким образом, пользователю предлагается ввести значение радиуса круга по указанным в инструкции правилам, которые преобразуются в тип float. Далее в коде программы следует инициализация переменной r, хранящей в себе числовой показатель радиуса, считывание посредством конструкции float(input()) и присваивание переменной соответствующего считанного значения.

Для отображения результатов вычисления программы в консоль с помощью оператора print() выводится комментарий 'Площадь круга равна', далее вызывается функция area(r), выводится результат этой функции, со следующей строки с помощью оператора print() выводится комментарий 'Периметр круга равен', далее вызывается функция perimeter(r), выводится результат этой функции, и программа завершает работу.


## Описание процесса работы программы square.py
Содержимое программы square.py выглядит следующим образом
```
def area(a):
    '''Принимает на вход число a (число с плавающей точкой в десятичной системе счисления), возвращает квадрат числа a.

        Пример вызова функции:
            area(196) = 38416.0
    '''
    return a * a


def perimeter(a):
    '''
        Возвращает произведение десятичной константы и числа с плавающей точкой в десятичной системе счисления.

            Параметры:
                a (float) : число с плавающей точкой в десятичной системе счисления

                Возвращаемое значение:
                (4 * a) (float) : число с плавающей точкой в десятичной системе счисления

                Пример вызова функции:
                    perimeter(196) = 784.0
        '''
    return 4 * a


print(
    'Введите значение стороны квадрата в формате x, если сторона квадрата выражена натуральным числом, либо в формате x.y, где x — показатель целой части, y — показатель дробной части.',
    '\n')
a = float(input())
print('Площадь квадрата равна', area(a), '\n')
print('Периметр квадрата равен', perimeter(a), '\n')
```
### Функция area(a)

* **Назначение:**
Принимает на вход число a (число с плавающей точкой в десятичной системе счисления), возвращает квадрат числа a — площадь квадрата.

* **Пример вызова функции:**
area(196) = 38416.0


### Функция perimeter(a):
* **Назначение:**
Возвращает произведение десятичной константы и числа с плавающей точкой в десятичной системе счисления.

* **Параметры:**
a (float) : число с плавающей точкой в десятичной системе счисления.

* **Возвращаемое значение:**
(4 * a) (float) : число с плавающей точкой в десятичной системе счисления.

* **Пример вызова функции:**
perimeter(196) = 784.0


Программа хранит в памяти 1 переменную типа float — сторону квадрата.

Данная программа предназначена для вычисления площади и периметра квадрата по заданной пользователем стороне квадрата.

Так как достижение поставленной задачи может быть реализовано посредством элементарных вычислений без привлечения посторонних констант, никакие из встроенных стандартных модулей импортированы не были.

Первый фрагмент программы — декларирование (объявление) функции area(a), которая получает на вход в качестве аргумента значение стороны квадрата, содержащейся в переменной a, отвечает за вычисление площади квадрата по формуле
**$S = a^2$**, где a — сторона квадрата,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции.

Следующий фрагмент программы — декларирование (объявление) функции perimeter(a), которая получает на вход в качестве аргумента значение стороны квадрата, содержащейся в переменной a, отвечает за вычисление периметра квадрата по формуле
**$P = 4a$**, где a — сторона квадрата,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции.

В целях получения программой входных данных в консоль с помощью оператора print() выводится комментарий 'Введите значение стороны квадрата в формате x, если сторона квадрата выражена натуральным числом, либо в формате x.y, где x — показатель целой части, y — показатель дробной части.'. Таким образом, пользователю предлагается ввести значение стороны квадрата по указанным в инструкции правилам, которое преобразуется в тип float. Далее в коде программы следует инициализация переменной a, хранящей в себе числовой показатель стороны квадрата, считывание данных при выполнении оператора float(input()), обработка и присваивание переменной a полученных входных данных. 

Для отображения результатов вычисления программы в консоль с помощью оператора print() выводится комментарий 'Площадь квадрата равна', далее вызывается функция area(a), выводится результат этой функции, со следующей строки с помощью оператора print() выводится комментарий 'Периметр квадрата равен', далее вызывается функция perimeter(a), выводится результат этой функции, и программа завершает работу.


## Описание процесса работы программы rectangle.py
Содержимое программы rectangle.py выглядит следующим образом
```
def area(a, b):
    '''
    Возвращает произведение двух чисел с плавающей точкой в десятичной системе счисления.

        Параметры:
            a (float) : первое число с плавающей точкой в десятичной системе счисления
            b (float) : второе число с плавающей точкой в десятичной системе счисления

            Возвращаемое значение:
            (a * b) (float) : число с плавающей точкой в десятичной системе счисления

                Пример вызова функции:
                    area(27.1, 18.9) = 512.1899999999999
    '''
    return a * b


def perimeter(a, b):
    '''
        Возвращает произведение десятичной константы и суммы двух чисел с плавающей точкой в десятичной системе счисления.

            Параметры:
                a (float) : первое число с плавающей точкой в десятичной системе счисления
                b (float) : второе число с плавающей точкой в десятичной системе счисления

                Возвращаемое значение:
                (2 * (a + b)) (float) : число с плавающей точкой в десятичной системе счисления

                    Пример вызова функции:
                        perimeter(27.1, 18.9) = 92.0
    '''
    return 2 * (a + b)


print(
    'Введите значения смежных сторон прямоугольника, каждое из которых с новой строки в формате x, если соответствующая сторона выражена натуральным числом, либо в формате x.y, где x — показатель целой части, y — показатель дробной части.',
    '\n')
a = float(input())
b = float(input())
print('Площадь прямоугольника равна', area(a, b), '\n')
print('Периметр прямоугольника равен', perimeter(a, b), '\n')
```
### Функция area(a, b)

* **Назначение:**
Возвращает произведение двух чисел с плавающей точкой в десятичной системе счисления.

* **Параметры:**
a (float) : первое число с плавающей точкой в десятичной системе счисления
b (float) : второе число с плавающей точкой в десятичной системе счисления

* **Возвращаемое значение:**
(a * b) (float) : число с плавающей точкой в десятичной системе счисления

* **Пример вызова функции:**
area(27.1, 18.9) = 512.1899999999999


### Функция perimeter(a, b)

* **Назначение:**
Возвращает произведение десятичной константы и суммы двух чисел с плавающей точкой в десятичной системе счисления.

* **Параметры:**
a (float) : первое число с плавающей точкой в десятичной системе счисления
b (float) : второе число с плавающей точкой в десятичной системе счисления

* **Возвращаемое значение:**
(2 * (a + b)) (float) : число с плавающей точкой в десятичной системе счисления

* **Пример вызова функции:**
perimeter(27.1, 18.9) = 92.0


Программа хранит в памяти 2 переменных типа float — 2 смежные стороны прямоугольника.

Данная программа предназначена для вычисления площади и периметра прямоугольника по заданным пользователем смежным сторонам.

Так как достижение поставленной задачи может быть реализовано посредством элементарных вычислений без привлечения посторонних констант, никакие из встроенных стандартных модулей импортированы не были.

Первый фрагмент программы — декларирование (объявление) функции area(a, b), которая получает на вход в качестве аргументов значения смежных сторон прямоугольника, хранящихся в переменных a и b, отвечает за вычисление площади прямоугольника по формуле
**$S = ab$**, где a, b — смежные стороны прямоугольника,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции.

Следующий фрагмент программы — декларирование (объявление) функции perimeter(a, b), которая получает на вход в качестве аргумента значения смежных сторон прямоугольника, хранящихся в переменных a и b, отвечает за вычисление периметра прямоугольника по формуле
**$S = 2 * (a + b)$**, где a, b — смежные стороны прямоугольника,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции.

В целях получения программой входных данных в консоль с помощью оператора print() выводится комментарий 'Введите значения смежных сторон прямоугольника, каждое из которых с новой строки в формате x, если соответствующая сторона выражена натуральным числом, либо в формате x.y, где x — показатель целой части, y — показатель дробной части'. Таким образом, пользователю предлагается ввести значения смежных сторон прямоугольника по указанным в инструкции правилам, которые преобразуются в тип float. Далее в коде программы следует инициализация переменных a и b, хранящих в себе числовые показатели смежных сторон прямоугольника, считывание посредством последовательных конструкций float(input()) и присваивание переменным соответствующих значений.

Для отображения результатов вычисления программы в консоль с помощью оператора print() выводится комментарий 'Площадь прямоугольника равна', далее вызывается функция area(a, b), выводится результат этой функции, со следующей строки с помощью оператора print() выводится комментарий 'Периметр прямоугольника равен', далее вызывается функция perimeter(a, b), выводится результат этой функции, и программа завершает работу.


## Описание процесса работы программы triangle.py
Содержимое программы rectangle.py выглядит следующим образом
```
def area(a, h):
    '''
        Возвращает частное произведения двух чисел с плавающей точкой в десятичной системе счисления и десятичной константы.

            Параметры:
                a (float) : первое число с плавающей точкой в десятичной системе счисления
                h (float) : второе число с плавающей точкой в десятичной системе счисления

                Возвращаемое значение:
                (a * h / 2) (float) : число с плавающей точкой в десятичной системе счисления

                    Пример вызова функции:
                        area(60, 74) = 2220.0
    '''
    return a * h / 2


def perimeter(a, b, c):
    '''
            Возвращает сумму трех чисел с плавающей точкой в десятичной системе счисления и десятичной константы.

                Параметры:
                    a (float) : первое число с плавающей точкой в десятичной системе счисления
                    b (float) : второе число с плавающей точкой в десятичной системе счисления
                    c (float) : третье число с плавающей точкой в десятичной системе счисления

                    Возвращаемое значение:
                    (a + b + c) (float) : число с плавающей точкой в десятичной системе счисления

                        Пример вызова функции:
                            perimeter(60, 80, 100) = 240.0
    '''
    return a + b + c


print(
    'Введите значения трех сторон треугольника и высоты, проведенной к первой введенной стороне, каждое из которых с новой строки в формате x, если соответствующая сторона выражена натуральным числом, либо в формате x.y, где x — показатель целой части, y — показатель дробной части.',
    '\n')
a = float(input())
b = float(input())
c = float(input())
h = float(input())
print('Площадь треугольника равна', area(a, h), '\n')
print('Периметр треугольника равен', perimeter(a, b, c), '\n')
```

### Функция area(a, h)

* **Назначение:**
Возвращает частное произведения двух чисел с плавающей точкой в десятичной системе счисления и десятичной константы.

* **Параметры:**
a (float) : первое число с плавающей точкой в десятичной системе счисления
h (float) : второе число с плавающей точкой в десятичной системе счисления

* **Возвращаемое значение:**
(a * h / 2) (float) : число с плавающей точкой в десятичной системе счисления

* **Пример вызова функции:**
area(60, 74) = 2220.0


### Функция perimeter(a, b, c)
* **Назначение:**
Возвращает сумму трех чисел с плавающей точкой в десятичной системе счисления и десятичной константы.

* **Параметры:**
a (float) : первое число с плавающей точкой в десятичной системе счисления
b (float) : второе число с плавающей точкой в десятичной системе счисления
c (float) : третье число с плавающей точкой в десятичной системе счисления

* **Возвращаемое значение:**
(a + b + c) (float) : число с плавающей точкой в десятичной системе счисления

* **Пример вызова функции:**
perimeter(60, 80, 100) = 240.0


Программа хранит в памяти 4 переменных типа float — 3 стороны треугольника и высоту данного треугольника.

Данная программа предназначена для вычисления площади и периметра треугольника по заданным пользователем трем сторонам и высоте.

Так как достижение поставленной задачи может быть реализовано посредством элементарных вычислений без привлечения посторонних констант, никакие из встроенных стандартных модулей импортированы не были.

Первый фрагмент программы — декларация (объявление) функции area(a, h), которая получает на вход в качестве аргументов 2 числа с плавающей точкой — значение стороны треугольника и высоты, падающей на данную сторону, хранящихся в переменных a и h соответственно, отвечает за вычисление площади треугольника по формуле
**$S = 1/2 (a * h)$**, где a — сторона треугольника, h — высота, опущенная на данную сторону,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции.

Следующий фрагмент программы — декларация (объявление) функции perimeter(a, b, c), которая получает на вход в качестве аргументов 3 числа с плавающей точкой — значения сторон треугольника, хранящихся в переменных a, b, c, отвечает за вычисление периметра треугольника по формуле
**$P = a + b + c$**, где a, b и c — стороны треугольника,
и возвращает найденное значение при выполнении оператора return в случае вызова данной функции.

В целях получения программой входных данных в консоль с помощью оператора print() выводится комментарий 'Введите значения трех сторон треугольника и его высоты, каждое из которых с новой строки в формате x, если соответствующая сторона выражена натуральным числом, либо в формате x.y, где x — показатель целой части, y — показатель дробной части.'. Таким образом, пользователю предлагается ввести значения смежных сторон треугольника по указанным в инструкции правилам, которые преобразуются в тип float. Далее в коде программы следует инициализация переменных a, b, c и h, хранящих в себе числовые показатели трех сторон треугольника, считывание посредством последовательных конструкций float(input()) и присваивание переменным соответствующих считанных значений.

Для отображения результатов вычисления программы в консоль с помощью оператора print() выводится комментарий 'Площадь треугольника равна', далее вызывается функция area(a, h), выводится результат этой функции, и со следующей строки с помощью оператора print() выводится комментарий 'Периметр треугольника равен', далее вызывается функция perimeter(a, b, c), выводится результат этой функции, и программа завершает работу.

# История изменения проекта с хешами коммитов (кроме последней записи)

**04.03.2021**

commit 8ba9aeb3cea847b63a91ac378a2a6db758682460

Добавлены новые файлы circle.py и square.py для вычисления площадей и периметров круга и квадрата.

commit d078c8d9ee6155f3cb0e577d28d337b791de28e2

В файл README.md внесены формулы для вычисления площадей и периметров круга, прямоугольника и квадрата.


**25.09.2023**

commit bcb6fd8466add79afbd66ba348a0934b7eb7d8fa

Добавлен новый файл rectangle.py для вычисления площади и периметра прямоугольника.

commit 2cbafb51dfa4c1eb03e682c5ba2088ad5a577318

Добавлен новый файл triangle.py для вычисления площади треугольника по высоте и стороне, падающей на эту сторону, и периметра по заданным сторонам.

commit 57d02e8247ad321e1cbd52f2983f4ab05bf63149

Исправлена ошибка в вычислении периметра прямоугольника.


**07.10.2023**

commit 5fbc244bf7a908ff5b4ab7f91836471433ca22c6

В функции, расположенные в файлах triangle.py, square.py, rectangle.py, circle.py внесены комментарии о назначениях данных функций, типах входных параметров и возвращаемых значений, код оснащен операторами считывания входных данных и выводом возвращаемых функциями значений, расширился функционал проекта.

commit 23bcf9e069168122a34ef6731a6ecd103c52208d

Внесены дополнительные корректировки в комментарии для разработчика, касающиеся типов возвращаемых данных, а также для пользователя в рамках указаний формата ввода данных. Исправлены опечатки в названиях функций в примерах вызова.


**08.10.2023**

commit d37341471e18d84cb22aec4cef0455e44bac10d6

В проект внесена документация в файле documentation.md.

**09.10.2023**

Документация внесена в файл README.md, находящийся в каталоге docs.


# Написание Unittest

## Описание тестов

### Тестирование модуля circle.py

| Название теста | Входные данные | Ожидаемый результат | Результат (true/false) |
| -------------- | -------------- | ------------------- | ---------------------- |
| test_zero_mul | data = [0] | 0 | true |
| test_area_mul | data = [254] | 202682.99163899910057265590051566 | true |
| test_perimeter_mul | data = [198] | 1244.0706908215581224312067797787 | true |
| test_perimeter_negative | data = [-8329] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_area_negative | data = [-18.301] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_perimeter_inf | data = [1.7976931348623157e+308] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_area_inf | data = [1.7976931348623157e+308] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_perimeter_str | data = ['bibaboba'] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_area_str | data = ['bambam'] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_perimeter_value | data = [10, 62819] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |
| test_area_value | data = [5932, 3, 1, 6, 9] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |

### Тестирование модуля rectangle.py
| Название теста | Входные данные | Ожидаемый результат | Результат (true/false) |
| -------------- | -------------- | ------------------- | ---------------------- |
| test_zero_mul | data = [0, 9] | 0 | true |
| test_area_mul | data = [613, 463] | 283819 | true
| test_perimeter_mul | data = [1983, 8348292] | 16700550 | true |
| test_perimeter_negative | data = [-8329, 7929] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_area_negative | data = [-18.301, 0] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_perimeter_inf | data = [1.7976931348623157e+308, 1] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_area_inf | data = [9, 1.7976931348623157e+308] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_perimeter_str | data = ['bibaboba', 'www'] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_area_str | data = ['bambam', 373021] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_perimeter_value | data = [10, 62819, 1] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |
| test_area_value | data = [5932] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |

### Тестирование модуля triangle.py
| Название теста | Входные данные | Ожидаемый результат | Результат (true/false) |
| -------------- | -------------- | ------------------- | ---------------------- |
| test_zero_mul | data = [0, 9, 2, 7] | 0 | true |
| test_area_mul | data = [51, 32, 78, 381.84578733521687] | 9737.06757704803 | true
| test_perimeter_mul | data = [52, 45, 82, 467.4964275406964] | 179 | true |
| test_perimeter_negative | data = [-8329, 7929, 23920, 1289382] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_area_negative | data = [-18.301, 0, 1, 1] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_perimeter_inf | data = [1.7976931348623157e+308, 1, 4, 8] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_area_inf | data = [1.7976931348623157e+308, 193, 821923, 1] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_perimeter_str | data = ['bibaboba', 'www', 'ac/dc', 'apdjbqw'] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_area_str | data = ['bambam', 373021, "2102", -7] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_perimeter_value | data = [53, 19, 49, 207.4209427473755, 53, 60, 37, 324.58698460221365] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |
| test_area_value | data = [3, 79, 94] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |

### Тестирование модуля square.py
| Название теста | Входные данные | Ожидаемый результат | Результат (true/false) |
| -------------- | -------------- | ------------------- | ---------------------- |
| test_zero_mul | data = [0] | 0 | true |
| test_area_mul | data = [542] | 293764 | true |
| test_perimeter_mul | data = [78358252] | 313433008 | true |
| test_perimeter_negative | data = [-8329] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_area_negative | data = [-18.301] | 'Значение элемента геометрической фигуры не может быть отрицательным, введите корректные данные.' | true |
| test_perimeter_inf | data = [1.7976931348623157e+308] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_area_inf | data = [1.7976931348623157e+308] | 'Ошибка: Переполнение в результате выполнения арифметической операции.' | true |
| test_perimeter_str | data = ['bibaboba'] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_area_str | data = ['bambam'] | 'Входные данные являются строковыми значениями, а не численными. Попробуйте еще раз и введите корректные данные.' | true |
| test_perimeter_value | data = [10, 62819] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |
| test_area_value | data = [5932, 3, 1, 6, 9] | 'Перечитайте условие и введите необходимое количество входных данных.' | true |
