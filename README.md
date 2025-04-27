# Embedded_CPP_Training
Embedded C++ Training with yocto linux
## Reverse the String
```cpp 
#include <iostream>
std::string strrev(std::string a)
{
    int len =a.length();
    for (int i=0; i<len/2; i++)
    {
        char temp = a[i];
        a[i]=a[len-i-1];
        a[len-i-1]= temp;
    }
    return a;
}
int main() {
    std::string let = "Helloworld";
    std::cout << strrev(let) << std::endl;
    return 0;
}
```
