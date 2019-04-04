# DPR-QUIZ-ALGOS
Algorithm Quiz 1
 
<h4>Please answer the following questions by forking this project. Respond within the README file by editing it. Then submit your Github URL on Canvas</h4>
<ol>
 <li>What does sheevpalpatine.java do? You can copy the code from above and use a browser ide here... https://www.compilejava.net/</li>
 
 This java program will take a String and decide whether or not it s a palindrome. A palindrome is a word or sentence (string) that is identicle whether read forwards or backwards, such as the name "Hannah". If the string entered is a palindrome, the program will return tru. If not it will return false. 
 
 
 
  <li>Submit a binary search example by adding a file to this project after forking it. Be sure to explain how the example functions using comments or in this README.</li>
  
  I found this example on geeksforgeeks.org

// Java implementation of recursive Binary Search 
class BinarySearch { 
	// Returns index of x if it is present in arr[], else return -1 
	int binarySearch(int arr[], int l, int r, int x) 
	{ 
		if (r >= l) { 
			int mid = l + (r - l) / 2; 

			// If the element is present at the 
			// middle itself 
			if (arr[mid] == x) 
				return mid; 

			// If element is smaller than mid, then 
			// it can only be present in left subarray 
			if (arr[mid] > x) 
				return binarySearch(arr, l, mid - 1, x); 

			// Else the element can only be present 
			// in right subarray 
			return binarySearch(arr, mid + 1, r, x); 
		} 

		// We reach here when element is not present 
		// in array 
		return -1; 
	} 

	// Driver method to test above 
	public static void main(String args[]) 
	{ 
		BinarySearch ob = new BinarySearch(); 
		int arr[] = { 2, 3, 4, 10, 40 }; 
		int n = arr.length; 
		int x = 10; 
		int result = ob.binarySearch(arr, 0, n - 1, x); 
		if (result == -1) 
			System.out.println("Element not present"); 
		else
			System.out.println("Element found at index " + result); 
	} 
} 
/* This code is contributed by Rajat Mishra */
  
  
  
  
  
  <li>Is a selection sort or a bubble sort faster?</li>
 </ol>

Selection sort is faster and more efficient than bubble sort, however it is less stable.

For bubble sort, adjacent elements in an array are compared and swapped.
For selection sort, the largest element is selected and swapped with the last element (in case of ascending order). This results in typically less iterations.

