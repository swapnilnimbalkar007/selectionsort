
public class SelectionSort1 {

	public static void main(String[] args) {
		
		int arr[] = {1,8,7,9,2,6};
		int length = arr.length;
		
		for(int i=0;i<length-1;i++)
		{
			int min_index=i;
			for(int j=i+1;j<length;j++)
			{
				if(arr[min_index] > arr[j])
				{
					min_index=j;
				}
			}
			
			int temp = arr[min_index];
			arr[min_index] = arr[i];
			arr[i] = temp;
		}
		
		for(int arr1: arr)
		{
			System.out.println(arr1);
		}

	}

}
