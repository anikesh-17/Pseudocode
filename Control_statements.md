# Control Statements
1. Selection
    1. If
    2. Case
2. Loop Iteration
    1. While
    2. Repeat Until
    3. For
3. Jump
    1. Break
    2. GOTO
    3. Continue
    4. Return

---

# Selection Statement

### Simple IF

> 
> 
> 
> DECLARE x : INTEGER
> READ x
> 
> IF x >= 5 THEN
> PRINT "x is greater than or equal to 5"
> END IF
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int x;
    cin >> x;

    if (x >= 5) {
        cout << "x is greater than or equal to 5";
    }

    return 0;
}
```

### IF–ELSE

> 
> 
> 
> DECLARE num : INTEGER
> READ num
> 
> IF num MOD 2 == 0 THEN
> PRINT "EVEN"
> ELSE
> PRINT "ODD"
> END IF
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int num;
    cin >> num;

    if (num % 2 == 0)
        cout << "EVEN";
    else
        cout << "ODD";

    return 0;
}
```

### Find Greater Number

> 
> 
> 
> DECLARE a : INTEGER
> DECLARE b : INTEGER
> 
> READ a
> READ b
> 
> IF a > b THEN
> PRINT "a is greater"
> ELSE
> PRINT "b is greater"
> END IF
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;

    if (a > b)
        cout << "a is greater";
    else
        cout << "b is greater";

    return 0;
}
```

### Nested IF

> 
> 
> 
> DECLARE uid : STRING
> DECLARE pass : STRING
> 
> READ uid
> READ pass
> 
> IF uid == "PIP" THEN
> IF pass == "PPP" THEN
> PRINT "WELCOME"
> ELSE
> PRINT "INVALID PASS"
> END IF
> ELSE
> PRINT "INVALID UID"
> END IF
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    string uid, pass;

    cin >> uid;
    cin >> pass;

    if (uid == "PIP") {
        if (pass == "PPP")
            cout << "WELCOME";
        else
            cout << "INVALID PASSWORD";
    }
    else {
        cout << "INVALID USER ID";
    }

    return 0;
}
```

### IF–ELSE–IF Ladder

> 
> 
> 
> DECLARE x : INTEGER
> DECLARE y : INTEGER
> 
> READ x
> READ y
> 
> IF x > 0 AND y > 0 THEN
> PRINT "1st Quadrant"
> 
> ELSE IF x < 0 AND y > 0 THEN
> PRINT "2nd Quadrant"
> 
> ELSE IF x < 0 AND y < 0 THEN
> PRINT "3rd Quadrant"
> 
> ELSE IF x > 0 AND y < 0 THEN
> PRINT "4th Quadrant"
> 
> ELSE
> PRINT "Origin"
> END IF
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int x, y;
    cin >> x >> y;

    if (x > 0 && y > 0)
        cout << "1st Quadrant";
    else if (x < 0 && y > 0)
        cout << "2nd Quadrant";
    else if (x < 0 && y < 0)
        cout << "3rd Quadrant";
    else if (x > 0 && y < 0)
        cout << "4th Quadrant";
    else
        cout << "Origin";

    return 0;
}
```

### CASE / SWITCH

> 
> 
> 
> DECLARE value : INTEGER
> READ value
> 
> CASE value OF
> 1 : PRINT "ONE"
> 2 : PRINT "TWO"
> 3 : PRINT "THREE"
> 4 : PRINT "FOUR"
> 5 : PRINT "FIVE"
> OTHERWISE PRINT "WRONG"
> END CASE
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int value;
    cin >> value;

    switch(value) {
        case 1: cout << "ONE"; break;
        case 2: cout << "TWO"; break;
        case 3: cout << "THREE"; break;
        case 4: cout << "FOUR"; break;
        case 5: cout << "FIVE"; break;
        default: cout << "WRONG";
    }

    return 0;
}
```