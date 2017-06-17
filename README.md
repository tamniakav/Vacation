using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Exam_3
{
    class Program
    {
        static void Main(string[] args)
        {
            double budget = double.Parse(Console.ReadLine());
            string season = Console.ReadLine().ToLower();

            if (season == "summer")
            {
                if (budget <= 1000)
                {
                    budget *= 0.65;
                    Console.WriteLine("Alaska - Camp - {0:f2}", budget);
                }
                else if (budget > 1000 && budget <= 3000)
                {
                    budget *= 0.80;
                    Console.WriteLine("Alaska - Hut - {0:f2}", budget);
                }
                else
                {
                    budget *= 0.90;
                    Console.WriteLine("Alaska - Hotel - {0:f2}", budget);
                }
            }
            else if (season == "winter")
            {
                if (budget <= 1000)
                {
                    budget *= 0.45;
                    Console.WriteLine("Morocco - Camp - {0:f2}", budget);
                }
                else if (budget > 1000 && budget <= 3000)
                {
                    budget *= 0.60;
                    Console.WriteLine("Morocco - Hut - {0:f2}", budget);
                }
                else
                {
                    budget *= 0.90;
                    Console.WriteLine("Morocco - Hotel - {0:f2}", budget);
                }
            }
        }
    }
}
