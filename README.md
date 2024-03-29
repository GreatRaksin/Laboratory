# Практическая работа
## Списки и циклы

Давайте вспомним, что такое списки и циклы.
**Циклы** - управляющая конструкция, которая нужна для многократного исполнения кода.
**Cписки** - упорядоченная изменяемая последовательность данных произвольных типов.

В **Python** существует два вида циклов:
- условный цикл **while**. Цикл будет исполняться, пока верно условие, написанное после ключевого слова while.
- счетный цикл **for**. Цикл исполняется заданное количество раз. Для управления количеством итераций (повторений) цикла используется функция **range(start, stop, step)**. Например, <code>range(0, 12, 2)</code> означает последовательность чисел от 0 до 11 с шагом 2.

Чтобы создать список, нужно написать его название, затем поставить оператор присваивания (**=**) и квадратные скобочки. <code>myList = [1, 2, 'three', 4, [1.2, 2.2]]</code>
<hr>

### Задача 0.
Напишите программу, которая будет запрашивать у пользователя 7 чисел и добавлять их в список <code>numbers</code>. Программа должна вывести 3 значения:
1. Самое большое число;
2. Самое маленькое число;
3. Сумма всех чисел.

Для нахождения максимального и минимального значений используйте встроенные функции <code>max()</code> и <code>min()</code>. Для подсчета суммы чисел используйте функцию <code>sum()</code>.

### Усложнение.
Добавьте к программе из задачи 0 обработчик исключений, чтобы пользователь, вводя не числовые значения, получал сообщение "Вы ввели не число". Также сделайте так, чтобы программа запускалась заново, если пользователь ошибся с вводом.
<hr>

### Задача 1.
Заполните список случайными целыми числами.
### Усложнение.
Отсортируйте полученный список по возрастанию.
<hr>

### Задача 2.
Если функцию <code>range()</code> включить в функцию <code>list()</code>, она преобразует все случайные числа в список. Создайте программу, которая будет генерировать список с элементами от 1 до 100 с шагом 7.
<hr>

### Задача 3.
Есть список, состоящий из неопределенного количества положительных и отрицательных чисел. Необходимо посчитать количество отрицательных чисел и вывести их количество на экран пользователю.
<hr>

### Задача 4.
Напишите программу, которая будет заполнять список 8 словами. Слова вводятся пользователем. Программа должна измерить длину каждого слова (функция <code>len()</code>) и добавить количество букв в другой список. Список с введенными словами и список с количеством символов в каждом слове должны выводиться на экран.
<hr>

## Строки
### Задача 5.
Пользователь вводит строку, в которой есть и строчные и прописные буквы. Выведите эту же строку, сделав все буквы в строке прописными буквами, если в строке больше прописных или строчными буквами, если в строке больше строчных букв. 
<blockquote>
Пример:<br>
Вводится строка "ПРИвет АНДрЕй". Программа должна вывести "ПРИВЕТ АНДРЕЙ", потому что в исходной строке больших букв больше, чем маленьких.
</blockquote>
Чтобы выполнить все проверки, нужно познакомиться с новыми методами для строк:
- <code>.islower()</code> - проверяет, являются ли символы в строке маленькими. 
- <code>.isupper()</code> - проверяет, являются ли символы в строке большими. 
- <code>.lower()</code> - позволяет преобразовать все символы в строке в маленькие буквы.
- <code>.upper()</code> - позволяет преобразовать все символы в строке в большие буквы.
<hr>

### Задача 6. 
Существует метод, который позволяет проверить, являются ли все символы в строке числами - <code>.isdigit()</code>.
Напишите программу, которая получает от пользователя два числа и выводит их сумму. Если пользователь введет не числа, программа не должна завершаться с ошибкой, она должна снова запрашивать числа. 

### Усложнение.
Обработка исключений (оператор **try-except**) запрещена.
<hr>

## Кортежи
### Задача 7
Создайте функцию, которая будет заполнять кортеж случайными целыми числами от 0 до 5 включительно.
Заполните случайными числами один кортеж. Затем заполните второй кортеж случайными числами от -5 до 0.
Объедините два кортежа и сделайте из них третий. Используя метод <code>.count()</code> посчитайте количество
1 (единиц) в кортеже. Выведите на экран третий кортеж и количество единиц в нем.

<hr>

## Словари
### Задача 8
Создайте словарь **school**, и наполните данными, которые бы отражали количество учащихся в разных классах '1а, 1б, 2б, 6а, 7в и т. д.). Внесите изменения в словарь согласно следующему: 
- В одном из классов изменилось количество учащихся, 
- в школе появился новый класс,
- в школе был расформирован (удален) другой класс. Вычислите общее количество учащихся в школе.
</hr>

### Задача 9
Создайте словарь. Ключи в нем должны быть числами, а значения - строками.
Примените к нему метод <code>.items()</code>, полученный объект <code>dict_items</code> передайте в написанную вами функцию, которая создает и
возвращает новый словарь, "обратный" исходному, т. е. ключами являются строки, а значениями – числа.
 
<hr>

### Задача 10
Выведите на экран степени двойки от 0 до 20.
<hr>

### Задача 11
Напишите функцию, которая считывает с клавиатуры числа и перемножает их до тех пор, пока не будет
введен 0. Функция должна возвращать полученное произведение.
<hr>

### Задача 12.
Напишите программу, которая циклично запрашивает у пользователя номера символов по таблице
Unicode и выводит соответствующие им символы. Завершает работу при вводе нуля. Для перевода из Unicode используйте функцию <code>chr()</code>

