# 100-days-of-c-upes-day-15-question-30-reverse-a-number-given-by-user-
#include <stdio.h>

int main() {
    int num, remainder, reversed = 0;

    
    printf("Enter an integer: ");
    scanf("%d", &num);

    
    while (num != 0) {
        remainder = num % 10;         
        reversed = reversed * 10 + remainder;
        num /= 10;                     
    }

   
    printf("Reversed number: %d\n", reversed);

    return 0;
}
