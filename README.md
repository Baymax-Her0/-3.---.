№1
# HI! Это моя первая программа для ветеринарной клиники!!!

# Сначала спросим у пользователя про питомца:

# Какой у него вид? (собака, кошка, попугай...)
pet_type = input("Какой вид питомца у вас? ")

pet_age = input("Сколько лет вашему питомцу? ")
pet_name = input("Как зовут вашего питомца? ")


message = "Это " + pet_type + " по кличке \"" + pet_name + "\". Возраст: " + pet_age + " года."
print(message)


№2
stage1 = input("Австралопитек: ")
stage2 = input("Человек умелый: ")
stage3 = input("Человек прямоходящий: ")
stage4 = input("Неандерталец): ")
stage5 = input("Человек разумный): ")
print(stage1, stage2, stage3, stage4, stage5, sep=" => ")

Урок №4
Задание №1

# Программа считает площадь и периметр прямоугольника

# Спрашиваем стороны
side_a_str = input("Введите сторону A: ")
side_b_str = input("Введите сторону B: ")

# Превращаем текст в числа
side_a = float(side_a_str)
side_b = float(side_b_str)

# Считаем площадь и периметр
area = side_a * side_b
perimeter = 2 * (side_a + side_b)

# Выводим результаты
print("Площадь: " + str(area))
print("Периметр: " + str(perimeter))

Задание №2

# Программа для работы с пятизначным числом

# Получаем число от пользователя
number_str = input("Введите пятизначное число: ")

# Превращаем текст в число
number = int(number_str)

# Находим цифры
единицы = number % 10
десятки = (number // 10) % 10
сотни = (number // 100) % 10
тысячи = (number // 1000) % 10
дес_тыс = number // 10000

# Считаем результат
степень = десятки ** единицы
умножение = степень * сотни
деление = умножение / (дес_тыс - тысячи)

# Выводим результат
print(деление)

Урок №5
Задание №1

# Получаем число
number_str = input("Введите целое число: ")
number = int(number_str)

# Проверяем, четное ли число
if number % 2 == 0:
  # Число четное
  if number == 0:
    print("нулевое число")
  elif number > 0:
    print("положительное четное число")
  else:
    print("отрицательное четное число")
else:
  # Число нечетное
  if number > 0:
    print("положительное нечетное число")
  elif number < 0:
    print("отрицательное нечетное число")
  else:
    print("число не является четным")

Задание №2

word = input("Введите слово: ")

# Говорим, какие буквы гласные
vowels = "aeiou"

# Считаем гласные и согласные
vowel_count = 0
consonant_count = 0

# Считаем, сколько каждой гласной
a_count = 0
e_count = 0
i_count = 0
o_count = 0
u_count = 0

# Проходим по каждой букве
for letter in word:
    if letter in vowels:
        vowel_count = vowel_count + 1
        if letter == "a":
            a_count = a_count + 1
        elif letter == "e":
            e_count = e_count + 1
        elif letter == "i":
            i_count = i_count + 1
        elif letter == "o":
            o_count = o_count + 1
        elif letter == "u":
            u_count = u_count + 1
    else:
        consonant_count = consonant_count + 1

# Выводим результаты
print("Гласных:", vowel_count)
print("Согласных:", consonant_count)

# Проверяем, есть ли все гласные
if a_count > 0:
    print("a:", a_count)
else:
    print("a: False")

if e_count > 0:
    print("e:", e_count)
else:
    print("e: False")

if i_count > 0:
    print("i:", i_count)
else:
    print("i: False")

if o_count > 0:
    print("o:", o_count)
else:
    print("o: False")

if u_count > 0:
    print("u:", u_count)
else:
    print("u: False")

Задание №3

# Спрашиваем минимальную сумму
x_str = input("Минимальная сумма инвестиций: ")
x = int(x_str)

# Спрашиваем деньги Майкла
a_str = input("Сколько денег у Майкла: ")
a = int(a_str)

# Спрашиваем деньги Ивана
b_str = input("Сколько денег у Ивана: ")
b = int(b_str)

# Проверяем, кто может вложиться
if a >= x and b >= x:
    print(2)
elif a >= x:
    print("Mike")
elif b >= x:
    print("Ivan")
elif a + b >= x:
    print(1)
else:
    print(0)

