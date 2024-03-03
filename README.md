#include <stdio.h>
 #define SIZE 100
 int main()
{
    int A[SIZE][SIZE];  
    int B[SIZE][SIZE];  
    int C[SIZE][SIZE];  

    int i, j,n;

     printf("enter size of array");
     scanf("%d",&n);
    printf("Enter elements in matrix A of size 3x3: \n");
    for(i=0; i<n; i++)
    {
        for(j=0; j<n; j++)
        {
            scanf("%d", &A[i][j]);

    }
}
    
    printf("\nEnter elements in matrix B of size 3x3: \n");
    for(i=0; i<n; i++)
    {
        for(j=0; j<n; j++)
        {
            scanf("%d", &B[i][j]);
        }
    }

    
    for(i=0; i<n; i++)
    {
        for(j=0; j<n; j++)
        {
             
            C[i][j] = A[i][j] + B[i][j];
        }
    }


     
    printf("\nSum of matrices A+B = \n");
    for(i=0; j<n; i++)
    {
        for(j=0; j<n; j++)
        {
            printf("%d ", C[i][j]);
        }
        printf("\n");
    }

    return 0;
}
