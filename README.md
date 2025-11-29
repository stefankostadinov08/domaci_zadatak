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
