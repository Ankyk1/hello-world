using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using NUnit.Framework;
using AwesomeCalculator;


namespace AwesomeCalcTest
{
    public class CalcTest1
    {
        [TestFixture]
        class CalcTests
        {
            [Test]
            public void GetAddition_Input4point5and6point9_Returns11point4()
            {
                //Arrange
                double number1 = 4.5; double number2 = 5.9;
                double expectedResult = number1 + number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetAddition();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

            [Test]
            public void GetAddition_Input99and66_Returns165()
            {
                //Arrange
                double number1 = 99; double number2 = 66;
                double expectedResult = number1 + number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetAddition();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

            [Test]
            public void GetAddition_Input9point9and6point5_Returns16point4()
            {
                //Arrange
                double number1 = 9.9; double number2 = 6.5;
                double expectedResult = number1 + number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetAddition();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

            [Test]
            public void GetSubtraction_Input9and6_Returns3()
            {
                //Arrange
                double number1 = 9; double number2 = 6;
                double expectedResult = number1 - number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetSubtraction();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

            [Test]
            public void GetSubtraction_Input9point5and6point5_Returns2()
            {
                //Arrange
                double number1 = 9.5; double number2 = 6.5;
                double expectedResult = number1 - number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetSubtraction();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

            [Test]
            public void GetSubtraction_Input11point4and6point4_Returns5()
            {
                //Arrange
                double number1 = 11.4; double number2 = 6.4;
                double expectedResult = number1 - number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetSubtraction();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

            [Test]
            public void GetMultiplication_Input11point4and6_Returns68point4()
            {
                //Arrange
                double number1 = 11.4; double number2 = 6;
                double expectedResult = number1 * number2;
                Calc testCalc = new Calc(number1, number2);
                //Act 
                double actualResult = testCalc.GetMultiplication();
                //Assert 
                Assert.AreEqual(expectedResult, actualResult);
            }

        }
    }
}
