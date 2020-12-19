# CF_732A---Buy-a-Shovel
using System;

namespace Shovel
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] text = (Console.ReadLine()).Split(' ');
            int k = int.Parse(text[0]);
            int r = int.Parse(text[1]);
            int i;
            for (i = 1; ; i++)
            {
                if (((k * i) - r) % 10 == 0 || (k * i) % 10 == 0)
                {
                    break;
                }
            }
            Console.WriteLine(i);
        }
    }
}
