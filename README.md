using System.Diagnostics;

namespace Dymchenko
{
    class Program
    {
        static int Euklides(int a, int b)
        {
            while (b != 0)
            {
                Console.WriteLine($"a = {a}, b = {b}");
                int dzielenie = a % b;
                a = b;
                b = dzielenie;
            }
            Console.WriteLine($"NWD = {a}");
            return a;
        }
        static void Main()
        {

            Console.Write("Podaj pierwszą liczbę całkowitą: ");
            int c = int.Parse(Console.ReadLine());
            Console.Write("Podaj drugą liczbę całkowitą: ");
            int z = int.Parse(Console.ReadLine());
            int nwd = Euklides(c, z);
          
            Console.ReadKey(true);

        }
