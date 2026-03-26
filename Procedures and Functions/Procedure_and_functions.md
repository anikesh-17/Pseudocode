## Procedure: Add Two Numbers

Pseudocode

```

PROCEDURE add(x : INTEGER, y : INTEGER)

PRINT x + y

END PROCEDURE

CALL add(12, 3)
```

## C++ Code

```cpp

#include <iostream>
using namespace std;

void add(int x, int y) {
    cout << x + y;
}

int main() {
    add(12, 3);
}
```

## Output

```
15
```

---

# Procedure: Cube of a Number

## Pseudocode

```
PROCEDURE cube(a : INTEGER)
    PRINT a * a * a
END PROCEDURE

CALL cube(3)
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

void cube(int a) {
cout<<a*a*a;
}

int main() {
    cube(3);
}
```

## Output

```
27
```

---

# Procedure: Area of Triangle

## Pseudocode

```
PROCEDURE areaTriangle(b : INTEGER, h : INTEGER)
    PRINT (b * h) / 2
END PROCEDURE

CALL areaTriangle(10, 5)
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

void areaTriangle(int b,int h) {
cout<< (b*h)/2;
}

int main() {
    areaTriangle(10,5);
}
```

## Output

```
25
```

---

# Procedure: Maximum of Two Numbers

## Pseudocode

```
PROCEDURE max(a : INTEGER, b : INTEGER)
    IF a > b THEN
        PRINT a
    ELSE
        PRINT b
    END IF
END PROCEDURE

CALL max(10, 20)
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

void maxNum(inta,intb) {
    if(a>b)
        cout<<a;
    else
        cout<<b;
}

int main() {
    maxNum(10,20);
}
```

## Output

```
20
```

---

# Function: Add Two Numbers

## Pseudocode

```
FUNCTION add(a : INTEGER, b : INTEGER) RETURN INTEGER
    RETURN a + b
END FUNCTION

PRINT add(2, 3)
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int add(int a,int b) {
return a+b;
}

int main() {
    cout<<add(2,3);
}
```

## Output

```
5
```

---

# Function: Maximum of Two Numbers

## Pseudocode

```
FUNCTION max(a : INTEGER, b : INTEGER) RETURN INTEGER
    DECLARE c : INTEGER

    IF a > b THEN
        c := a
    ELSE
        c := b
    END IF

    RETURN c
END FUNCTION

PRINT max(23, 6)
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int maxNum(int a,int b) {
    int c;

    if(a>b)
        c = a;
    else
        c =b;

    return c;
}

int main() {
    cout<<maxNum(23,6);
}
```

## Output

```
23
```

---

# Procedure: Simple Interest

## Pseudocode

```
PROCEDURE simpleInterest(pa : INTEGER, roi : REAL, noy : REAL)
    DECLARE si : REAL
    si := (pa * roi * noy) / 100
    PRINT si
END PROCEDURE

CALL simpleInterest(12, 3, 4)
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

void simpleInterest(int pa,float roi,float noy) {
    float si = (pa*roi*noy)/100;
    cout<<si;
}

int main() {
    simpleInterest(12,3,4);
}
```

## Output

```
1.44
```

---

# Function: Simple Interest

## Pseudocode

```
FUNCTION simpleInterest(pa : INTEGER, roi : REAL, noy : REAL) RETURN REAL
    DECLARE si : REAL
    si := (pa * roi * noy) / 100
    RETURN si
END FUNCTION

PRINT simpleInterest(12,3,4)
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

float simpleInterest(int pa,float roi,float noy) {
    floatsi = (pa*roi*noy)/100;
    return si;
}

int main() {
    cout<<simpleInterest(12,3,4);
}
```

## Output

```
1.44
```

---

# Function: Area of Circle

## Pseudocode

```
FUNCTION areaCircle(rad : REAL) RETURN REAL
    RETURN 3.14 * rad * rad
END FUNCTION

PRINT areaCircle(6.6)
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

float areaCircle(float rad) {
    return 3.14*rad*rad;
}

int main() {
    cout<<areaCircle(6.6);
}
```

## Output

```
136.7784
```

---

# Absolute Value Function

## Pseudocode

```
FUNCTION absValue(a : INTEGER) : INTEGER
    RETURN abs(a)
END FUNCTION

PRINT absValue(-5)
```

## C++ Code

```cpp
#include <iostream>
#include <cmath>
using namespace std;

int absValue(int a){
    return abs(a);
}

int main(){
    cout << absValue(-5);
}
```

## Output

```
5
```

---

# Absolute Value Without Built-in Function

## Pseudocode

```
FUNCTION absValue(a : INTEGER) : INTEGER
    DECLARE b : INTEGER

    IF a > 0 THEN
        b := a
    ELSE
        b := a * -1
    END IF

    RETURN b
END FUNCTION

PRINT absValue(-5)
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

int absValue(int a){
    int b;

    if(a > 0)
        b = a;
    else
        b = a * -1;

    return b;
}

int main(){
    cout << absValue(-5);
}
```

## Output

```
5
```

---

# Factorial Function

## Pseudocode

```
FUNCTION fact(n : INTEGER) : INTEGER
    DECLARE f : INTEGER
    SET f := 1

    FOR i := n TO 1 STEP -1
        f := f * i
    END FOR

    RETURN f
END FUNCTION

PRINT fact(5)
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

int fact(int n){
    int f = 1;

    for(int i = n; i >= 1; i--){
        f *= i;
    }

    return f;
}

int main(){
    cout << fact(5);
}
```

## Output

```
120
```

---

# Sum of Series (1 + 2 + 3 + ... + n)

## Pseudocode

```
FUNCTION series(n : INTEGER) : INTEGER
    DECLARE sum : INTEGER
    sum := 0

    FOR i := 1 TO n
        sum := sum + i
    END FOR

    RETURN sum
END FUNCTION

PRINT series(5)
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

int series(int n){
    int sum = 0;

    for(int i = 1; i <= n; i++){
        sum += i;
    }

    return sum;
}

int main(){
    cout << series(5);
}
```

## Output

```
15
```

---

# Harmonic Series (1 + 1/2 + 1/3 + ... + 1/n)

## Pseudocode

```
FUNCTION series(n : INTEGER) : REAL
    DECLARE sum : REAL
    sum := 0

    FOR i := 1 TO n
        sum := sum + (1 / i)
    END FOR

    RETURN sum
END FUNCTION
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

double series(int n){
    double sum = 0;

    for(int i = 1; i <= n; i++){
        sum += 1.0 / i;
    }

    return sum;
}

int main(){
    cout << series(5);
}
```

## Output

```
2.28333
```

---

# Reverse Number Function

## Pseudocode

```
FUNCTION reverse(n : INTEGER) : INTEGER
    DECLARE a : INTEGER
    DECLARE b : INTEGER

    SET b := 0

    WHILE n > 0
        a := n MOD 10
        n := n / 10
        b := b * 10 + a
    END WHILE

    RETURN b
END FUNCTION

PRINT reverse(1234)
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

int reverseNum(int n){
    int a, b = 0;

    while(n > 0){
        a = n % 10;
        n = n / 10;
        b = b * 10 + a;
    }

    return b;
}

int main(){
    cout << reverseNum(1234);
}
```

## Output

```
4321
```

---

# Palindrome Function

## Pseudocode

```
FUNCTION palindrome(n : INTEGER) : STRING
    DECLARE a,b,c : INTEGER

    SET b := 0
    SET c := n

    WHILE n > 0
        a := n MOD 10
        n := n / 10
        b := b * 10 + a
    END WHILE

    IF b == c THEN
        RETURN "PALINDROME"
    ELSE
        RETURN "NOT PALINDROME"
    END IF
END FUNCTION
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

string palindrome(int n){
    int a, b = 0, c = n;

    while(n > 0){
        a = n % 10;
        n = n / 10;
        b = b * 10 + a;
    }

    if(b == c)
        return "PALINDROME";
    else
        return "NOT PALINDROME";
}

int main(){
    cout << palindrome(121);
}
```

## Output

```
PALINDROME
```

---

# Swap Procedure (By Value)

## Pseudocode

```
PROCEDURE swap (BYVAL x : INTEGER, y : INTEGER)
    DECLARE z : INTEGER
    z = x
    x = y
    y = z
END PROCEDURE

x = 10
y = 20
CALL swap(x, y)
```

---

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

void swapValues(int x, int y) {
    int z;

    z = x;
    x = y;
    y = z;

    cout << "Inside Procedure:\\n";
    cout << "x = " << x << " y = " << y << endl;
}

int main() {

    int x = 10;
    int y = 20;

    swapValues(x, y);

    cout << "Outside Procedure:\\n";
    cout << "x = " << x << " y = " << y << endl;

    return 0;
}
```

---

## Output

```
Inside Procedure:
x = 20 y = 10

Outside Procedure:
x = 10 y = 20
```

---