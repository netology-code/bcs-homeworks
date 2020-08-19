# Задача 2. Возведение в степень

## Описание

Дана заготовка программы с функцией:

```cs
using System;

class Program
{
    /// <summary>
    /// Функция возведения в степень. По умолчанию возводит в квадрат.
    /// </summary>
    /// <param name="x">основание</param>
    /// <param name="pow">показатель</param>
    /// <returns>степень</returns>
    static double Pow(double x, int pow = 2)
    {
        double y = 1;
        for (int i = 0; i < pow; ++i)
        {
            y *= x;
        }
        return y;
    }

    static void Main(string[] args)
    {
        // здесь ваш код
    }
}
```

Необходимо вывести квадраты чисел от 3 до 6, а затем кубы чисел от 7 до 9.

Пример вывода:

```
Квадраты от 3 до 6:
9
16
25
36
Кубы от 7 до 9:
343
512
729
```
