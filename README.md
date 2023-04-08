# assignment-2
# The sum of the first n odd numbers is always equal to n^2. Write a 
#C program to verify this fact 
#using a "for" loop

#include <stdio.h>

int main() {
    int n, sum = 0;

    printf("Enter a value for n: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        sum += 2*i - 1;
    }

    printf("The sum of the first %d odd numbers is %d\n", n, sum);

    if (sum == n*n) {
        printf("The formula n^2 = %d is verified for n = %d", n*n, n);
    }
    else {
        printf("The formula n^2 = %d is NOT verified for n = %d", n*n, n);
    }

    return 0;
}
