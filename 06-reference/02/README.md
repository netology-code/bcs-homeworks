# Задача 2. Краткость - сестра таланта

## Описание

Дана программа:

```cs
using System;

class Program
{
   static int Sum(int x, int y)
   {
       return x + y;
   }
   static int Sub(int x, int y)
   {
       return x - y;
   }
   static int Mult(int x, int y)
   {
       return x * y;
   }
   static int Div(int x, int y)
   {
       if (y == 0) return 0;
       return x / y;
   }

   static void Calc(int x, int y, Func<int, int, int> f)
   {
       int result = f(x, y);
       Console.WriteLine(result);
   }

   static void Main(string[] args)
   {
       Calc(7, 8, Sum);
       Calc(15, 8, Sub);
       Calc(6, 7, Mult);
       Calc(4, 0, Div);
   }
}
```

Необходимо все функции, по возможности, переписать в сокращенном виде. Если какую-то функцию невозможно переписать в сокращенном виде - оставить как есть.

---

### Подсказки

> Не читайте этот раздел сразу, попытайтесь сначала решить задачу самостоятельно :)

<details>

<summary>Подсказка 1</summary>

Все функции, кроме `Main`, можно переписать в сокращенной форме.

</details>

<details>

<summary>Подсказка 2</summary>

Чтобы записать функцию `Div` в сокращенной форме - стоит вспомнить [тернарный оператор](https://docs.microsoft.com/ru-ru/dotnet/csharp/language-reference/operators/conditional-operator).

</details>
