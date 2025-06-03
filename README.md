# pattern-wuth-which-rows-can-be-changed.c
//  C program to print pattern with given rows // example enter no. of rows=11  ABCDEFGHIJKKJIHGFEDCBA ABCDEFGHIJ  JIHGFEDCBA ABCDEFGHI    IHGFEDCBA ABCDEFGH      HGFEDCBA ABCDEFG        GFEDCBA ABCDEF          FEDCBA ABCDE            EDCBA ABCD              DCBA ABC                CBA AB                  BA A                    A 
//  C program to print pattern with given rows
// example enter no. of rows=11

ABCDEFGHIJKKJIHGFEDCBA
ABCDEFGHIJ  JIHGFEDCBA
ABCDEFGHI    IHGFEDCBA
ABCDEFGH      HGFEDCBA
ABCDEFG        GFEDCBA
ABCDEF          FEDCBA
ABCDE            EDCBA
ABCD              DCBA
ABC                CBA
AB                  BA
A                    A

#include <stdio.h>
int main() {
    int i,j,n;
    printf("enter rows=");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        for(j=0;j<=n-1-i;j++)
         printf("%c",65+j);
        for(j=0;j<=i-1;j++)
         printf(" ");
         for(j=0;j<=i-1;j++)
         printf(" ");
        for(j=n-1-i;j>=0;j--)
         printf("%c",65+j);
        printf("\n");
    }
    return 0;
}
