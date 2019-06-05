# TestMethods_Assignment_2
2nd Assignment


                    using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp18
{
     public static class TriangleSolver
    {
        public static string Analaysis(int a, int b, int c)
        {
            if (((a + b) > c) && ((b + c) > a) && ((c + a) > b))
            {
                if (a == b && b == c)
                {
                    return ("Equilateral triangle");
                }
                else if (a == b || b == c || c == a)
                {
                    return ("Isosceles triangle");
                }
                else
                {
                    return ("Scalene triangle");
                }
            }
            else
            {
                Console.Write("The given sides does not form a triangle, try again.\n");
                return ("No triangle");
            }
        }

    }
}





