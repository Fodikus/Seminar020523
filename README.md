# Seminar020523
Домашняя работа №4 к семинару "Знакомство с языками программирования"

# Задача 25: Напишите цикл, который принимает на вход два числа (A и B) и возводит число A в натуральную степень B.
Нельзя использовать Math.Pow();
```
Console.Clear();
Console.Write("Введите число A: ");
int a = Convert.ToInt32(Console.ReadLine());
Console.Write("Введите степень B: ");
int b = Convert.ToInt32(Console.ReadLine());

int result = 1;
for (int i = 1; i <= b; i++)
    result = result * a;
Console.WriteLine($"{a},{b} -> {result} ({a}^{b})");
```

# Задача 27: Напишите программу, которая принимает на вход число и выдаёт сумму цифр в числе.
```
Console.Clear();
Console.Write("Введите число N: ");
int n = Convert.ToInt32(Console.ReadLine());

int result = 0;
while (n != 0)
{
    result = result + n % 10;
    n = n / 10;
}

Console.WriteLine($"Сумма цифр в числе N -> {result}");
```

# Задача 29: https://acmp.ru/asp/do/index.asp?main=task&id_course=1&id_section=5&id_topic=114&id_problem=699
```
Console.Clear();
Console.Write("Введите число учеников: ");
int n1 = Convert.ToInt32(Console.ReadLine());

while (n1 > 100)
{
    Console.WriteLine($"Вы ошиблись! Максимальное число учеников не должно превышать 100! \nВведите количество учеников: ");
    n1 = Convert.ToInt32(Console.ReadLine());
}

Console.Write("Введите рост Пети: ");
int n2 = Convert.ToInt32(Console.ReadLine());
while (n2 > 200)
{
    Console.WriteLine($"Вы ошиблись! Рост Пети не должен превышать 200! \nВведите рост Пети: ");
    n2 = Convert.ToInt32(Console.ReadLine());
}

int[] array = new int[n1];
for (int i = 0; i < n1; i++)
{
    array[i] = new Random().Next(100, 200); 
}

int result = 0;
for (int i = 0; i < n1; i++)
{
    if (array[i] > n2)
    {
        result = result + 1;
    }
}

Console.WriteLine($"Рост учеников: [{string.Join(", ", array)}] ");
Console.WriteLine($"Количество учеников выше Пети: {result} ");
```

# Суперсдвиг(https://acmp.ru/asp/do/index.asp?main=task&id_course=1&id_section=5&id_topic=114&id_problem=702)
```

```

# Гипотеза Гольдбаха(https://acmp.ru/asp/do/index.asp?main=task&id_course=1&id_section=6&id_topic=117&id_problem=723)
```

```
