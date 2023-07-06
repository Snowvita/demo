## C program to find the Transpose of the given matrix
```c
#include<stdio.h>
int main()
{
        int i,j,a[4][4],trans[4][4],m,n;
        printf("Enter the number of rows and columns of a matrix: ");
        scanf("%d %d",&m,&n);
        printf("Enter the values of a matrix:\n");
        for(i=0;i<m;i++)
        {
                for(j=0;j<n;j++)
                        scanf("%d",&a[i][j]);
        }
        for(i=0;i<m;i++)
        {
                for(j=0;j<n;j++)
                        trans[j][i]=a[i][j];
        }
        printf("Transpose of a matrix: \n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<m;j++)
                        printf("%d\t",trans[i][j]);
                printf("\n");
        }
        return 0;
}
```
