# bubble_sort
package elclipse;
import java.util.*;
public class bubblesort {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {4,9,5,8,6,2,78,564,};
		int n=a.length;
		int end=a.length-1;
		int search=14;
		bubble(a,n); ///calling function


	}
	public static void bubble(int a[],int n) {
		int temp=0;
		for(int i=0;i<n;i++) {
			for(int j=0;j<n-i-1;j++) {
				if(a[j+1]<a[j]) {     //swapping two element at a time
					temp=a[j+1];
					a[j+1]=a[j];
					a[j]=temp;
				}
			}
		}
		System.out.print(Arrays.toString(a)); ///convert array to string
	}

} 

//time complexity of this solution is o(n^2);
