# TestMethods_Assignment_2
2nd Assignment



                        using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using ConsoleApp18;
using NUnit.Framework;

namespace Assignment2_Unit_test
{

    [TestFixture]
    public class Class1
    {

        [Test]
        public void Analysis_Input1andInput1andInput1_expectedEquilateraltriangle()
        {

            //Arrange

            int a = 1;
            int b = 1;
            int c = 1;
            string expectedResult = "Equilateral triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input2andInput2andInput2_expectedEquilateraltriangle()
        {

            //Arrange

            int a = 2;
            int b = 2;
            int c = 2;
            string expectedResult = "Equilateral triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input2andInput2andInput3_expectedIsocelestriangle()
        {

            //Arrange

            int a = 2;
            int b = 2;
            int c = 3;
            string expectedResult = "Isosceles triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input3andInput3andInput4_expectedIsoscelestriangle()
        {

            //Arrange

            int a = 3;
            int b = 3;
            int c = 4;
            string expectedResult = "Isosceles triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input2andInput3andInput4_expectedScalenetriangle()
        {

            //Arrange

            int a = 2;
            int b = 3;
            int c = 4;
            string expectedResult = "Scalene triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input5andInput6andInput7_expectedScalenetriangle()
        {

            //Arrange

            int a = 5;
            int b = 6;
            int c = 7;
            string expectedResult = "Scalene triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input0andInput0andInput0_expectedNotriangle()
        {

            //Arrange

            int a = 0;
            int b = 0;
            int c = 0;
            string expectedResult = "No triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Analysis_Input1andInput2andInput3_expectedNotriangle()
        {

            //Arrange

            int a = 1;
            int b = 2;
            int c = 3;
            string expectedResult = "No triangle";

            //Act

            string actualResult = TriangleSolver.Analaysis(a, b, c);

            //Assert

            Assert.AreEqual(expectedResult, actualResult);
        }
    }
}
