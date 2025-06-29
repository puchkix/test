# first program
using System
public Random Random;
{
    int num = random.randint(1, 100);
    Console.WriteLine("Guess the number from 1 to 100. DON'T type the number in LETTERS");
    int guess = Convert.ToInt32(Console.ReadLine());
    int numOfGuesses = 1;
    while (guess != num)
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
    }
    Console.WriteLine("You Win!1!!!!!!!1!111!1");
    Environment.Exit(0);
}
