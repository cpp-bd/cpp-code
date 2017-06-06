### Pointer Basic
```cpp
#include <iostream>
using namespace std; 
 
int main()
{
 
    int a = 10;
    int *p;
    int **pp;
    int ***ppp;
    
    p = &a;
    pp = &p;
    ppp = &pp;
    
    cout << *p << endl;    // 10
    cout << **pp << endl;  // 10
    cout << ***ppp << endl;// 10
    
    *p = 20;
    
    cout << a << endl;     // 20
    cout << **pp << endl;  // 20
    cout << ***ppp << endl;// 20
    
    return 0;
}
```
