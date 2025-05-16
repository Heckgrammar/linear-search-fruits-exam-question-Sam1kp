
            string[] fruits = { "banana", "apple", "orange", "pear", "grape", "pineapple" };

            // Your program should:
            // Ask the user what word they would like to find
            // Output the message True if the word is found
            // Output the message False if the word is not found

            // You must write your own linear search routine and not use any built-in fuctions available in C#
            // You should use meaningful variable names
            Console.WriteLine("what fruit would you like to find ?");
            var fruitToFind = Console.ReadLine();
            bool found = false;
            if (fruitToFind != null)
            {
                for (int i = 0; i < fruits.Length; i++)
                {
                    if (fruits[i] == fruitToFind)
                    {
                        found = true;
                        break;
                    }
                }
                if (found)
                {
                    Console.WriteLine("True");
                }
                else
                {
                    Console.WriteLine("False");
                }
            }
            else
            {
                Console.WriteLine("Please enter a valid fruit name.");

            }
        }
    }
}
