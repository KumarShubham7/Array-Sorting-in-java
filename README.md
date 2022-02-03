# Array-Sorting-in-java
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner op = new Scanner(System.in);
	    
	    System.out.println("Enter the size of array:- ");
	    int n = op.nextInt();
	    int temp;
	    
	    int A[] = new int[n];
	    
	    
	    System.out.println("Enter all the elements :- ");
	    for(int i=0;i<n;i++)
	    {
	        A[i]=op.nextInt();
	    }
	    
	    for(int i=0;i<n-1;i++)
	    {
	        for(int j=i+1;j<n;j++)
	        {
	            if(A[j]<A[i])
	            {
	                temp = A[i];
	                A[i]=A[j];
	                A[j]=temp;
	            }
	        }
	    }
	    
	    System.out.println("");
	    System.out.println("Elements after sorting are:- ");
	    for(int i=0;i<n;i++)
	    {
	        System.out.print(A[i]+" ");
	    }
		
	}
}
