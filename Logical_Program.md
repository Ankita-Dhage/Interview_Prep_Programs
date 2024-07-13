# 1.Find number is armstrong or not 

 Code

```
public class ArmstronNo {
	public static void main(String[] args) {
		int n = 153, arm = 0, rem, c;
		c = n; // store the original value of n in c
		while (n > 0) {
			rem = n % 10;
			arm = (rem * rem * rem) + arm;
			n = n / 10;
		}
		if (c == arm) // compare c with arm
			System.out.println("number is Armstrong");
		else
			System.out.println("number is not Armstrong");
	}
}
```

# 2.Write a program for finding factorial of a number

Code
```
public class FactorialNo {

	public static void main(String[] args) {

		int n = 0, fact = 1;
		System.out.println("enter any no");
		Scanner sc = new Scanner(System.in);
		n = sc.nextInt();

		for (int i = 1; i <= n; i++)

			fact = fact * i;
		System.out.println("factorial of no is:" + fact);
	}

}
```

# 3.Write a program for Fibonacci series if you enter term as 5 then output as :01123

Code
```
 public class FibonacciSeries {
	public static void main(String[] args) {
		int term, a = 0, b = 1, c;
		System.out.println("enter any term");

		Scanner sc = new Scanner(System.in);
		term = sc.nextInt();

		for (int i = 1; i <= term; i++) {

			System.out.println(a);
			c = a + b;

			a = b;
			b = c;

		}
	}
}
```

#  4.Write a program to find prime number.

```
public class PrimeNo {
	public static void main(String[] args) {
		int n = 0, count = 0;

		System.out.println("enter any no");
		Scanner sc = new Scanner(System.in);
		sc.nextInt();
		for (int i = 1; i <= n; i++) {
			if (n % i == 0) {

				count++;
			}
		}
		{
			if (count == 2) {
				System.out.println("no is prime");
			} else {
				System.out.println("no is not prime");

			} 

		}
	}
}
```

# 5.Write a program for reverse a number 123 -- 321

code
```
public class ReverseNo {
	public static void main(String[] args) {

		int n, r = 0;

		System.out.println("Enter any number");
		Scanner sc = new Scanner(System.in);
		n = sc.nextInt();

		while (n > 0) {
			r = n % 10;
			System.out.println(r);
			n = n / 10;
			System.out.println("n is :: " + n);
		}
	}
}
```

# 6. How to swap two numbers without using a third variable?

code
```
public class SwapNo {
	public static void main(String[] args) {
		int a = 10, b = 20;

		// Swap without using third variable
//		a = a + b;
//		b = a - b;
//		a = a - b;

		// swap using third variable
		int c = a;
		a = b;
		b = c;

		System.out.println("after swapping " + a + " " + b);

	}
}
```

# 7.Sum of all elements in integer array?
 
 Code
 ```
public class SumOfArray {
	public static void main(String[] args) {
		int a[] = { 40, 20, 40, 20 };
		int sum = 0;

		// for (int i = 0; i <= a.length - 1; i++) {

        //			sum = sum + a[i];
		// }

		for (int value : a) {
			sum = sum + value;

		}
		System.out.println("sum of an array is:" + sum);

	}

}
```

# 8. Find largest number in an array?
		
```
public class LargestNoInArray {

	public static void main(String[] args) {

		int a[] = { 10, 52, 65, 100, 90 };
		System.out.println("length:: " + a.length);
		int max = a[0];
		for (int i = 0; i < a.length; i++) {

			if (a[i] > max) {
				max = a[i];
			}
		}

		System.out.println("largest value in an array is:" + max);

	}
}
```

# 9.Java Program to check if number is Palindrome Check?
Code
```
public class PalindromeNum {

	public static void main(String args[]) {
		int n, rem, sum = 0, temp;
		System.out.println("enter any no");
		Scanner sc = new Scanner(System.in);
		n = sc.nextInt();
		temp = n;
		while (n > 0) {
			rem = n % 10; // getting remainder
			System.out.println("remainedr== " + rem);
			sum = (sum * 10) + rem;
			System.out.println("sum== " + sum);
			n = n / 10;
			System.out.println("n:: " + n);
		}
		if (temp == sum)
			System.out.println("palindrome number ");
		else
			System.out.println("not palindrome");
	}
}
```

# 10. Find second largest number in an array

Code
```
public class SecondLargestNoInArray {
	public static void main(String[] args) {

		int array[] = { 10, 20, 25, 57, 63, 96 };
		int size = array.length;
		Arrays.sort(array);

		System.out.println("array: " + Arrays.toString(array));// toString() return values in string

		// above we simply print array
		// now print sec largest no in an array

		int res = array[size - 2];
		System.out.println("second largest no in an array: " + res);

	}
	// output:[10, 20, 25, 57, 63, 96]
	// second largest no in an array: 63
}

```