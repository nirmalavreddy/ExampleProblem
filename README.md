# ExampleProblemForSelectionSort

public class SortAnArray {

	public static void main(String[] args) {
		
		int[]arr=new int[] {21, 86, -1, 11, 64};
		
		//array elements before sorting
		System.out.println("array elements before sorting are:");
		for(int i=0;i<arr.length;i++)
		{
			System.out.println(arr[i]);
		}
		
		//array elements after sorting
		System.out.println("array elements after sorting are:");
		for(int i=0;i<arr.length;i++)
		{
			for(int j=i+1;j<arr.length;j++)
			{
				int tmp=0;
				if(arr[i]>arr[j])
				{
					tmp=arr[i];
					arr[i]=arr[j];
					arr[j]=tmp;
				}
			}
			System.out.println(arr[i]);
		}
		}
}
