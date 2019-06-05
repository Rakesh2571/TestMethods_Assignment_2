# TestMethods_Assignment_2
2nd Assignment

                              using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp18
{
    class Program
    {
        static void Main(string[] args)
        {
            Program p = new Program();
            p.Run();

            Console.ReadKey();
        }
        public void Run()
        {
            string datast = string.Empty;
            string sta = string.Empty;
            string stb = string.Empty;
            string stc = string.Empty;
            string result = string.Empty;
            int dataint = 0;
            int a = 0;
            int b = 0;
            int c = 0;
            do
            {
                Console.Write("\n1.Enter triangle dimension  \n2.Exit \nEnter your option: ");
                datast = Console.ReadLine();
                if (int.TryParse(datast, out dataint))
                {
                    switch (dataint)
                    {
                        case 1:
                            Console.Write("Enter the first side of the triangle: ");
                            sta = Console.ReadLine();
                            if (!int.TryParse(sta, out a))
                            {
                                Console.WriteLine("Invalid entry,enter integer values only !!");
                                goto case 1;
                            }
                            Console.Write("Enter the second side of the triangle: ");
                            stb = Console.ReadLine();
                            if (!int.TryParse(stb, out b))
                            {
                                Console.WriteLine("Invalid entry,enter integer values only !!");
                                goto case 1;
                            }

                            Console.Write("Enter the third side of the triangle: ");
                            stc = Console.ReadLine();
                            if (!int.TryParse(stc, out c))
                            {
                                Console.WriteLine("Invalid entry, enter integer values only !!");
                                goto case 1;
                            }

                            result = TriangleSolver.Analaysis(a, b, c);
                            Console.Write("{0} is formed.", result);
                            break;
                        case 2:
                            Environment.Exit(0);
                            break;
                    }
                }
                else
                {
                    Console.WriteLine("Not a valid input, try agian !!");
                }

            } while (datast != "1" || datast != "2");

        }

    }
}
