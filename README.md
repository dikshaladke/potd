# potd
#Given an array arr[] of n positive integers. Push all the zeros of the given array to the right end of the array while maintaining the order of non-zero elements. Do the mentioned change in the array in-place.
void pushZerosToEnd(int arr[], int n) 
	{
	    int count=0;
	    for(int i=0;i<n;i++)
	    {
	        if(arr[i]!=0)
            {
                int temp=arr[i];
                arr[i]=arr[count];
                arr[count]=temp;
                count++;
            }
	    }
	   
	    // code here
	}
