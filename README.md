# specific-word-count


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp8
{
    class Program
    {
        static void Main(string[] args)

        {
            Console.WriteLine("Enter  a string:");
            string s = Console.ReadLine();
            string[] arr = s.Split();
                Console.WriteLine("Enter  a string to count specific word:");
                string fs = Console.ReadLine();
                int Count = 0;
                for (int i = 0; i < arr.Length; i++)
                {
                    if (arr[i].ToLower() == fs.ToLower())
                    {
                        Count++;
                    }                  
                }
            Console.WriteLine($"{fs} find:{Count} Count");        
        }
    } 
}
