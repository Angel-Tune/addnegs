using System;

namespace Calculator
{
    class Program
    {
        static double Add(double x, double y) => x + y;
        static double Subtract(double x, double y) => x - y;
        static double Multiply(double x, double y) => x * y;
        static double deleni(double x, double y) => x / y;

        static void Main()
        {
            Console.Write("Напиши 2 числа: ");
            var input = Console.ReadLine().Split();
            double a = double.Parse(input[0]), b = double.Parse(input[1]);

            Console.WriteLine($"{a} + {b} = {Add(a, b)}");
            Console.WriteLine($"{a} - {b} = {Subtract(a, b)}");
            Console.WriteLine($"{a} * {b} = {Multiply(a, b)}");
            Console.WriteLine($"{a} / {b} = {deleni(a, b)}");
        }
    }
}
