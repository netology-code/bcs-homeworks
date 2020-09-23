# Задача 4. Оптимизация

Дан код:

```cs
using System;

class Program
{
  static void Main(string[] args)
  {
    Console.Write("Введите x: ");
    double x = Convert.ToDouble(Console.ReadLine());

    Console.Write("Введите y: ");
    double y = Convert.ToDouble(Console.ReadLine());

    double result = (x + y) * (y + 1) - y * (x + 1);

    Console.Write("Результат: ");
    Console.WriteLine(result);
  }
}

```

Попробуйте упростить формулу так, чтобы результат был такой же, но количество операций уменьшилось.
