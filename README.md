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
## C++ Standard Template Library (STL)
### The C++ Standard Template Library (STL) is a set of template classes and functions that provides the implementation of common data structures and algorithms such as lists, stacks, arrays, sorting, searching, etc. It also provides the iterators and functors which makes it easier to work with algorithms and containers.

``` bash 
Components of STL
The components of STL are the features provided by Standard Template Library (STL) in C++ that can be classified into 4 types:

1. Containers
    a. Sequence Containers
        i.Arrays
        ii. Vector
        iii. Deque
        iv. Lists
        v. Forward Lists
    b. Container Adaptors
        i. Stack
        ii. Queue
        iii. Priority Queue
    c. Associative Containers
        i. Sets
        ii. Maps
        iii. Multisets
        iv. Multimaps
    d. Unordered Associated Containers
        i. Unordered Set
        ii. Unordered Multiset
        iii. Unordered Map
        iv. Unordered Multimap
2. Algorithms
    a. Manipulative Algorithms
        i.copy
        ii. fill
        iii. transform
        iv. replace
        v. swap
        vi. reverse
        vii. rotate
        viii. remove
        ix. unique
    b. Non-Manipulative Algorithms
        i. max_element
        ii. min_element
        iii.accumulate
        iv.count
        v. find
        vi.is_permutation
        vii, is_sorted
        viii. partial_sum
3. Iterators
    a.Input Iterators
    b. Output Iterators
    c. Forward Iterators
    d. Bidirectional Iterators
    e. Random Access Iterators
4. Functors
    a. Arithmetic Functors
        i. plus – Returns the sum of two parameters.
        ii. minus – Returns the difference of two parameters.
        iii. multiplies – Returns the product of two parameters.
        iv. divides – Returns the result after dividing two parameters.
        v. modulus – Returns the remainder after dividing two parameters.
        vi. negate – Returns the negated value of a parameter.
    b. Relational Functors
        i. equal_to – Returns true if the two parameters are equal.
        ii. not_equal_to – Returns true if the two parameters are not equal.
        iii. greater – Returns true if the first parameter is greater than the second.
        iv. greater_equal – Returns true if the first parameter is greater than or equal to the second.
        v. less – Returns true if the first parameter is less than the second.
        vi. less_equal – Returns true if the first parameter is less than or equal to the second.
    c. Logical Functors
        i. logical_and – Returns the result of Logical AND operation of two parameters.
        ii. logical_or – Returns the result of Logical OR operation of two parameters.
        iii. logical_not – Returns the result of Logical NOT operation of the parameters.
    d. Bitwise Functors

        i. bit_and – Returns the result of Bitwise AND operation of two parameters.
        ii. bit_or – Returns the result of Bitwise OR operation of two parameters.
        iii. bit_xor – Returns the result of Bitwise XOR operation of two parameters.
```
## Using [STL Cheat sheet ] https://www.geeksforgeeks.org/cpp-stl-cheat-sheet/
