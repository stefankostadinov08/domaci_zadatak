# Домаћи задатак из Техничке документације

## Задатак

Програм који на основу унете дужине **странице** једнакостраничног троугла a израчунава **полупречник уписане кружнице** r.

$r = \frac{a\sqrt{3}}{6}$

### Алгоритамска шема

![Алгоритамско решење](domaci.png)

## Решење
```cs
using System;


namespace ConsoleApp3
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Unesi duzinu stranice jednakostranicnog trougla a: ");
            double.TryParse(Console.ReadLine(), out double a);

            double r = a * Math.Sqrt(3.0) / 6.0;

            Console.WriteLine("Poluprecnik upisane kruznice r = "+r);
        }
    }
}
```
### Тест примери

Тест пример 1:
```
Unesi duzinu stranice jednakostranicnog trougla a: 2
Poluprecnik upisane kruznice r = 0,577350269189626

C:\Users\Admin\OneDrive\Desktop\ConsoleApp3\ConsoleApp3\bin\Debug\ConsoleApp3.exe (process 27404) exited with code 0 (0x0).
To automatically close the console when debugging stops, enable Tools->Options->Debugging->Automatically close the console when debugging stops.
Press any key to close this window . . .
```

Тест пример 2:
```
Unesi duzinu stranice jednakostranicnog trougla a: 4,67
Poluprecnik upisane kruznice r = 1,34811287855778

C:\Users\Admin\OneDrive\Desktop\ConsoleApp3\ConsoleApp3\bin\Debug\ConsoleApp3.exe (process 27168) exited with code 0 (0x0).
To automatically close the console when debugging stops, enable Tools->Options->Debugging->Automatically close the console when debugging stops.
Press any key to close this window . . .
```

### Објекти

| Редни број | Променљива | Тип променљиве |
| ---------- | ---------- | -------------- |
| 1.         | `a`    | `double`       |
| 2.         | `r`    | `double`       |
