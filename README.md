#include<stdio.h>   
int fib(int n)
int isPrime(int N)

int main()    
{    
 int n1=0,n2=1,n3,i,number;    
 printf("Enter the number of elements:");    
 scanf("%d",&number);    
 printf("\n%d %d",n1,n2);//printing 0 and 1    
 for(i=2;i<number;++i)//loop starts from 2 because 0 and 1 are already printed    
 {    
  n3=n1+n2;    
  printf(" %d",n3);    
  n1=n2;    
  n2=n3;    
 }  
  return 0;  
 }  

   int isPrime(int N) {
    for (int i = 2; i < N; i++) {

        if (N % i == 0) {
            return 0;
        }
    }
    return 1;
}

int main() {
    int N = 10;
    printf("Is %d prime?\n", N);

    if (isPrime(N)) {
        printf("Yes\n");
    }
    else {
        printf("No\n");
    }

    return 0;
}
int base, exp;
    long double result = 1.0;
    printf("Enter a base number: ");
    scanf("%d", &base);
    printf("Enter an exponent: ");
    scanf("%d", &exp);

    while (exp != 0) {
        result *= base;
        --exp;
    }
    printf("Answer = %.0Lf", result);
    return 0;
}
