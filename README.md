import java.util.Scanner;

class Large {
 
	public void find() {
		Scanner input = new Scanner(System.in);
		System.out.println("Enter elements of array");
		int arr[]= new int[5];
		for(int i=0;i<arr.length;i++)
		{
			arr[i]= input.nextInt();
		}
		int largest = arr[0];
		int secondLargest = arr[0];
		
		System.out.println("The given array is:" );
		for (int i = 0; i < arr.length; i++) {
			System.out.print(arr[i]);
		}
		for (int i = 0; i < arr.length; i++) {
 
			if (arr[i] > largest) {
				secondLargest = largest;
				largest = arr[i];
 
			} else if (arr[i] > secondLargest) {
				secondLargest = arr[i];
 
			}
		}
 
		System.out.println("\nSecond largest number is:" + secondLargest);
 
	}
}
public class Jala {
public static void main(String[] args) 
	{
		Large obj = new Large();
		obj.find();
    }
}
