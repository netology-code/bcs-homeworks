# Задача 1. Устранение дублирования

## Описание

Дана программа:

```cs
using System;

class Program
{
    static void Main(string[] args)
    {
        for (int w = 0; w < 10; ++w)
        {
            Console.Write('w');
        }
        Console.WriteLine();

        for (int w = 0; w < 10; ++w)
        {
            Console.Write('b');
        }
        Console.WriteLine();

        for (int w = 0; w < 10; ++w)
        {
            Console.Write('r');
        }
        Console.WriteLine();
    }
}
```

Необходимо определить общий участок кода и выделить его в функцию (имя функции - произвольное).

В функци `Main` должны быть вызовы написанной функции.

Результат работы программы не должен измениться.
