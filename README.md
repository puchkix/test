# GuessTheNumber
using System;

namespace Figure
{
    class Program
    {
        static void Main(string[] args)
        {
            Random random = new Random();
            int num = random.Next(1, 100);
            int numOfGuesses = 0;
            Console.WriteLine("Guess the number from 1 to 100. DON'T type the number in LETTERS");
            while (true)
            {
                int guess = Convert.ToInt32(Console.ReadLine());
                numOfGuesses++;
                if (guess > num)
                {
                    Console.WriteLine("Too High, Try again");
                }
                if (guess < num)
                {
                    Console.WriteLine("Too Low, Try again");
                }
                if (guess == num)
                {
                    break;
                }
            }
            Console.Write("You Win!1!!!!!!!1!111!1 ");
            Console.WriteLine($"With {numOfGuesses} guesses!!!!1!!!!");
            Environment.Exit(0);
        }
    }
}
