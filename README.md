using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace SENG8040_Assignment2
{

    public class Triangle
    {
        public static string Analyze(int SIDE1, int SIDE2, int SIDE3)
        {

            if ((SIDE1 + SIDE2 > SIDE3) && (SIDE2 + SIDE3 > SIDE1) && (SIDE1 + SIDE3 > SIDE2))
            {

                if (SIDE1 == SIDE2 && SIDE2 == SIDE3)
                {
                    return ("This is an Equilateral Triangle");
                }

                else if (SIDE1 == SIDE2 || SIDE1 == SIDE2 || SIDE3 == SIDE1)
                {
                    return ("This is an Isosceles Triangle");
                }

                else if (SIDE1 != SIDE2 || SIDE1 != SIDE2 || SIDE3 != SIDE1)
                {
                    return ("This is a Scalene Triangle");
                }

            }

            else
            {
                return ("Triangle cannot be created");
            }
            return ("");
        }
    }
}   

