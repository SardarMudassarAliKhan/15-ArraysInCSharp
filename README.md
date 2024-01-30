```csharp
using System;

class Program
{
    static void Main()
    {
        // Declaring and initializing an array
        int[] numbers = new int[] { 3, 1, 4, 1, 5 };

        // Accessing and printing elements of the array
        Console.WriteLine("Array elements:");
        for (int i = 0; i < numbers.Length; i++)
        {
            Console.WriteLine($"Element at index {i}: {numbers[i]}");
        }

        // Sorting the array
        Array.Sort(numbers);
        Console.WriteLine("\nArray after sorting:");
        foreach (var number in numbers)
        {
            Console.WriteLine(number);
        }

        // Finding a specific value in the array
        int searchValue = 4;
        int index = Array.BinarySearch(numbers, searchValue);
        if (index >= 0)
        {
            Console.WriteLine($"\n{searchValue} found at index {index}.");
        }
        else
        {
            Console.WriteLine($"{searchValue} not found in the array.");
        }

        // Sum of array elements
        int sum = Array.Sum(numbers);
        Console.WriteLine($"\nSum of array elements: {sum}");

        // Maximum and minimum values in the array
        int max = Array.Max(numbers);
        int min = Array.Min(numbers);
        Console.WriteLine($"Maximum value: {max}");
        Console.WriteLine($"Minimum value: {min}");
    }
}
```

This program declares, initializes, and operates on an integer array. It prints the original array, sorts it, searches for a specific value, calculates the sum, and finds the maximum and minimum values in the array.
