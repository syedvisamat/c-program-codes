# c-program-codes#include <stdio.h>
/*int main() // program to print 2d array and sum
{
    int  a[4][6];

    int i,j ,sum = 0;
    printf("enter the numbers in rows and columns:\n");
    for (i = 0; i < 4; i++)
    {
        for (j = 0; j < 6; j++)
        {
            scanf("%d", &a[i][j]);
        }
    }
    printf("matrix is:\n");
    for (i = 0; i < 4; i++)
    {
        for (j = 0; j < 6; j++)
        {
            printf("%d\t", a[i][j]);
            sum = sum + a[i][j];
        }
       printf("\n");
    }
    printf("\nsum=%d", sum);
    return 0;*/
int main()//to print transpose of a matrix
{int a[2][3],i,j,sumr,sumc;
printf("enter the elements of the matrix:\n");
for ( i = 0; i < 2; i++)
{
    for ( j = 0; j < 3; j++)
    {
        scanf("%d",&a[i][j]);
    }  
}printf("the matrix is:\n");
for ( i = 0; i < 2; i++)
{sumr=0,sumc=0;
    for ( j= 0; j < 3; j++)
    {
        printf("%d ",a[i][j]);}
        sumr=sumr+a[i][j];
        sumc=sumc+a[j][i];
    
    printf("\n");
} printf("the transpose of matrix is:\n");
for ( i = 0; i < 3; i++)
{
    for ( j = 0; j < 2; j++)
    {
        printf("%d ",a[j][i]);
    }
    printf("\n");
}
printf("the sum of row is %d\n",sumc);
printf("the sum of column is %d\n",sumr);
return 0;

}
