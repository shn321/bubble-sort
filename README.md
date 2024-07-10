# bubble-sort
#include <stdio.h>
#include <conio.h>

void main()
{
  int arr[20],i,n;
  void bubblesort(int[],int);
  printf("\n enter how many elements to enter?");
  scanf("%d",&n);
  printf("\n enter %d elements",n);
  for(i=0;i<n;i++)
    scanf("%d",&arr[i]);
  printf("\n before sorting elements are:");
  for(i=0;i<n;i++)
    printf("%d",arr[i]);
  bubblesort(arr,n);
  printf("\n after sorting elements are:");
  for(i=0;i<n;i++)
  printf("%d",arr[i]);
  getch();
}
void bubblesort(int arr[],int n)
{
    int temp,i,j;
     for(i=0;i<n;i++)
     {
          for(j=0;j<n-1-i;j++)
          {
              if(arr[j]>arr[j+1])
              {
                  temp=arr[j];
                  arr[j]=arr[j+1];
                  arr[j+1]=temp;
              }
}
}
}
