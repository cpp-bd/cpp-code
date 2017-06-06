### Swap Two Variables by Pointer
```c
#include <stdio.h>

void swap(char* a, char* b)
{
    int temp;
    temp = *a;
    *a = *b;
    *b = temp;
}

int main(void)
{
    char a = 'x';
    char b = 'y';
    
    printf("a is now %c and b is now %c\n", a, b); 
    
    swap(&a, &b);

    printf("a is now %c and b is now %c\n", a, b); 

    return 0;
}
```
