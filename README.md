# Day-21-Generics
Generic Koleksiyonlar ve List app.patika.dev





<img width="951" alt="Ekran Resmi 2022-05-23 16 21 12" src="https://user-images.githubusercontent.com/105243448/169828998-f1241da7-9d95-4a8d-b940-d5846e045821.png">


```


using System;

class Printer
{

	/**
	*    Name: PrintArray
	*    Print each element of the generic array on a new line. Do not return anything.
	*    @param A generic array
	**/
    // Write your code here
    
    public static void PrintArray<T>(T[] arr) {
        
       foreach(var a in arr){
           Console.WriteLine(a);
       }
    }


    static void Main(string[] args)
	{
		int n = Convert.ToInt32(Console.ReadLine());
		int[] intArray = new int[n];
		for (int i = 0; i < n; i++)
		{
			intArray[i] = Convert.ToInt32(Console.ReadLine());
		}
		
		n = Convert.ToInt32(Console.ReadLine());
		string[] stringArray = new string[n];
		for (int i = 0; i < n; i++)
		{
			stringArray[i] = Console.ReadLine();
		}
		
		PrintArray<Int32>(intArray);
		PrintArray<String>(stringArray);
	}
}


```

