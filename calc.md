# Описание функции romanToArabic:

1. Функция принимает на вход строку roman, содержащую число в римской системе счисления.

2. Создаётся объект romanNumbers, в котором каждой римской цифре соответствует её арабское значение.

3. Создаются переменные arabic и i, равные 0.

4. Запускается цикл while, который продолжается до тех пор, пока переменная i не достигнет длины строки roman.

5. Внутри цикла извлекается текущая цифра current из объекта romanNumbers, соответствующая символу в строке roman по
   индексу i.

6. Извлекается следующая цифра next из объекта romanNumbers, соответствующая символу в строке roman по индексу i + 1.

7. Если текущее значение current меньше следующего значения next, то вычитается current из next, и результат
   прибавляется к arabic. Индекс i увеличивается на 2, чтобы пропустить обе цифры.

8. В противном случае текущее значение current прибавляется к arabic, а индекс i увеличивается на 1.

9. После того как цикл завершается, функция возвращает значение переменной arabic, которое представляет число в арабской
   системе счисления, эквивалентное введённому числу в римской системе счисления.

# Описание функции arabicToRoman:

1. Функция принимает на вход число arabic, которое нужно перевести в римскую систему счисления.

2. Создаётся объект romanNumbers, в котором каждой римской цифре соответствует её арабское значение.

3. Создаётся переменная roman, равная пустой строке.

4. Запускается цикл for..in, который перебирает все свойства объекта romanNumbers.

5. Внутри цикла извлекается значение value из объекта romanNumbers, соответствующее ключу key.

6. Вычисляется количество цифр, равных value, в числе arabic, используя деление с округлением в меньшую сторону: count =
Math.floor(arabic / value).

7. Если количество цифр больше нуля, то к строке roman добавляется key повторенное count раз. Также из arabic вычитается
значение, равное произведению value на count, чтобы уменьшить оставшееся число.

8. После того как цикл завершается, функция возвращает значение переменной roman, которая содержит число, представленное в
римской системе счисления, эквивалентное введённому числу в арабской системе счисления.
