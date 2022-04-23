# Calculate-Discount-on-shoping
Printing discounted amount and rest amount 
using System;
using System.Collections.Generic;
using System.Text;

namespace smallest_number_find
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("***** WELCOME TO SHOP MARKET *****");
            
            Console.WriteLine(" Please Enter Your Shopping Amount ");
            int amt = int.Parse(Console.ReadLine()); //Amount enter by user
            int actamt = amt; // Stored amount in actual amount
            int disc; // discount amount variable
            if (amt >= 30000)
            {
                disc = amt * 30 / 100; // 30% discount on amount 
                amt = amt - disc; // Rest amount after discount

                Console.WriteLine("Your  Discount is 30% :" + disc);
                Console.WriteLine("Your Original Amount is :" +actamt);
                Console.WriteLine("Your Payable Amount is :" + amt);
                Console.WriteLine("***** THANK YOU, PLEASE VISIT AGAIN *****");
            }
            else if (amt >= 20000)
            {
                disc = amt * 20 / 100;
                amt = amt - disc;

                Console.WriteLine("Your  Discount is 20% :" + disc);
                Console.WriteLine("Your Original Amount is :" + actamt);
                Console.WriteLine("Your Payable Amount is :" + amt);
                Console.WriteLine("***** THANK YOU, PLEASE VISIT AGAIN *****");
            }
            else if (amt >= 10000)
            {
                disc = amt * 15 / 100;
                amt = amt - disc;

                Console.WriteLine("Your  Discount is 15%:" + disc);
                Console.WriteLine("Your Original Amount is :" + actamt);
                Console.WriteLine("Your Payable Amount is :" + amt);
                Console.WriteLine("***** THANK YOU, PLEASE VISIT AGAIN *****");
            }
            else
            {
                disc = amt * 6 / 100;
                amt = amt - disc;

                Console.WriteLine("Your  Discount is 6%:" + disc);
                Console.WriteLine("Your Original Amount is :" + actamt);
                Console.WriteLine("Your Payable Amount is :" + amt);
                Console.WriteLine("***** THANK YOU, PLEASE VISIT AGAIN *****");
            }

        }
    }
}

