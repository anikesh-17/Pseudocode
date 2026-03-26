---

# Repeat–Until Loop (Print 1 to 10)

## Pseudocode

```
DECLARE i : INTEGER
SET i := 1

REPEAT
    PRINT i
    INCREMENT i
UNTIL i > 10
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;

    do {
        cout << i << " ";
        i++;
    } while(i <= 10);

    return 0;
}
```

---

#  Repeat–Until Loop (Print 10 to 1)

## Pseudocode

```
DECLARE i : INTEGER
SET i := 10

REPEAT
    PRINT i
    DECREMENT i
UNTIL i < 1
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 10;

    do {
        cout << i << " ";
        i--;
    } while(i >= 1);

    return 0;
}
```

---

#  While Loop (Print 1 to 10)

## Pseudocode

```
DECLARE i : INTEGER
SET i := 1

WHILE i <= 10
    PRINT i
    INCREMENT i
END WHILE
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;

    while(i <= 10) {
        cout << i << " ";
        i++;
    }

    return 0;
}
```

---

#  Multiplication Table

## Pseudocode

```
DECLARE num : INTEGER
DECLARE i : INTEGER

READ num
SET i := 1

WHILE i <= 10
    PRINT num * i
    INCREMENT i
END WHILE
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {
    int num;
    cin >> num;

    for(int i = 1; i <= 10; i++) {
        cout << num * i << endl;
    }

    return 0;
}
```

---

#  For Loop (Print 1 to 10)

## Pseudocode

```
FOR i := 1 TO 10
    PRINT i
END FOR
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {

    for(int i = 1; i <= 10; i++) {
        cout << i << " ";
    }

    return 0;
}
```

---

#  For Loop (Print 10 to 1)

## Pseudocode

```
FOR i := 10 TO 1 STEP -1
    PRINT i
END FOR
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {

    for(int i = 10; i >= 1; i--) {
        cout << i << " ";
    }

    return 0;
}
```

---

#  Sum of Series

### 1 + 2 + 3 + ... + n

## Pseudocode

```
DECLARE n : INTEGER
DECLARE sum : INTEGER

READ n
sum := 0

FOR i := 1 TO n
    sum := sum + i
END FOR

PRINT sum
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {
    int n, sum = 0;
    cin >> n;

    for(int i = 1; i <= n; i++) {
        sum += i;
    }

    cout << sum;

    return 0;
}
```

---

#  Sum of Squares Series

### 1² + 2² + 3² + ... + n²

## Pseudocode

```
DECLARE n : INTEGER
DECLARE sum : INTEGER

READ n
sum := 0

FOR i := 1 TO n
    sum := sum + i * i
END FOR

PRINT sum
```

## C++ Implementation

```cpp
#include <iostream>
using namespace std;

int main() {
    int n, sum = 0;
    cin >> n;

    for(int i = 1; i <= n; i++) {
        sum += i * i;
    }

    cout << sum;

    return 0;
}
```

---

#  Series

### 1 + 1/2 + 1/3 + ... + 1/n

## Pseudocode

```
DECLARE n : INTEGER
DECLARE sum : REAL

READ n
sum := 0

FOR i := 1 TO n
    sum := sum + 1/i
END FOR

PRINT sum
```

---

# Series

### 1 + 1/4 + 1/9 + ... + 1/n²

## Pseudocode

```
DECLARE n : INTEGER
DECLARE sum : REAL

READ n
sum := 0

FOR i := 1 TO n
    sum := sum + 1/(i*i)
END FOR

PRINT sum
```

---
# Break

FOR i := 1 TO 10

IF i == 5 THEN

BREAK

END IF

PRINT i

END FOR

## C++ Code
```cpp
#include <iostream>
using namespace std;

int main() {
    for(int i = 1; i <= 10; i++) {
        if(i == 5)
            break;
        cout << i << " ";
    }
}
```

## Output

```
1 2 3 4
```

---

# Continue Statement

## Pseudocode

```
FOR i := 1 TO 10
    IF i == 5 THEN
        CONTINUE
    END IF
    PRINT i
END FOR
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    for(inti =1;i<=10;i++) {
        if(i==5)
            continue;
        cout<<i<<" ";
    }
}
```

## Output

```
1 2 3 4 6 7 8 9 10
```

---

# Print Even Numbers

## Pseudocode

```
FOR i := 1 TO 10
    IF i MOD 2 ≠ 0 THEN
        CONTINUE
    END IF
    PRINT i
END FOR
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    for(int i =1;i<=10;i++) {
        if(i%2!=0)
            continue;
        cout<<i<<" ";
    }
}
```

## Output

```
2 4 6 8 10
```

---

# Print Odd Numbers

## Pseudocode

```
FOR i := 1 TO 10
    IF i MOD 2 == 0 THEN
        CONTINUE
    END IF
    PRINT i
END FOR
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    for(int i =1;i<=10;i++) {
        if(i%2==0)
            continue;
        cout<<i<<" ";
    }
}
```

## Output

```
1 3 5 7 9
```

---

# Reverse a Number

## Pseudocode

```cpp
DECLARE n : INTEGER
DECLARE x : INTEGER
DECLARE rev : INTEGER

rev := 0
READ n

WHILE n > 0
    x := n MOD 10
    rev := rev * 10 + x
    n := n / 10
END WHILE

PRINT rev
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
int n,x,rev =0;
cin>>n;

while(n>0) {
x =n%10;
rev =rev*10+x;
n =n/10;
    }

cout<<rev;
}
```

## Output

```
Input: 1234
Output: 4321
```

---

# Palindrome Number

## Pseudocode

```
DECLARE n, x, rev : INTEGER
SET rev := 0

READ n
SET temp := n

WHILE n > 0
    x := n MOD 10
    rev := rev * 10 + x
    n := n / 10
END WHILE

IF rev == temp THEN
    PRINT "PALINDROME"
ELSE
    PRINT "NOT PALINDROME"
END IF
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
int n,x,rev =0,temp;
cin>>n;

temp =n;

while(n>0) {
x =n%10;
rev =rev*10+x;
n/=10;
    }

if(rev==temp)
cout<<"Palindrome";
else
cout<<"Not Palindrome";
}
```

## Output

```
Input: 121
Output: Palindrome
```

---

# Sum of Digits

## Pseudocode

```
DECLARE n : INTEGER
DECLARE x : INTEGER
DECLARE sum : INTEGER

sum := 0
READ n

WHILE n > 0
    x := n MOD 10
    sum := sum + x
    n := n / 10
END WHILE

PRINT sum
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int n,x,sum =0;
    cin>>n;

    while(n>0) {
        x =n%10;
        sum+=x;
        n/=10;
    }

    cout<<sum;
}
```

## Output

```
Input: 1234
Output: 10
```

---

# Count Digits

## Pseudocode

```
DECLARE n : INTEGER
DECLARE count : INTEGER

count := 0
READ n

WHILE n > 0
    n := n / 10
    count := count + 1
END WHILE

PRINT count
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int n,count =0;
    cin>>n;

    while(n>0) {
        n/=10;
        count++;
    }

    cout<<count;
}
```

## Output

```
Input: 45678
Output: 5
```

---

# Armstrong Number

## Pseudocode

```
DECLARE n, x, sum : INTEGER
sum := 0

READ n
SET temp := n

WHILE n > 0
    x := n MOD 10
    sum := sum + x*x*x
    n := n / 10
END WHILE

IF sum == temp THEN
    PRINT "ARMSTRONG"
ELSE
    PRINT "NOT ARMSTRONG"
END IF
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int n,x,sum =0,temp;
    cin>>n;

    temp =n;

    while(n>0) {
        x =n%10;
        sum+=x*x*x;
        n/=10;
    }

    if(sum==temp)
        cout<<"Armstrong";
    else
        cout<<"Not Armstrong";
}
```

## Output

```
Input: 153
Output: Armstrong
```

---

# Check if Digit is Present

## Pseudocode

```
DECLARE num, digit, x : INTEGER
DECLARE found : BOOLEAN

SET found := FALSE

READ num
READ digit

WHILE num > 0
    x := num MOD 10
    num := num / 10

    IF x == digit THEN
        found := TRUE
        BREAK
    END IF
END WHILE

IF found THEN
    PRINT "Digit Found"
ELSE
    PRINT "Digit Not Found"
END IF
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int num,digit,x;
    bool found =false;

    cin>>num>>digit;

    while(num>0) {
        x =num%10;
        num/=10;

    if(x==digit) {
        found =true;
        break;
    }
}

if(found)
    cout<<"Digit Found";
else
    cout<<"Digit Not Found";
}
```

## Output

```
Input:
12345
3

Output:
Digit Found
```
---

```
DECLARE num : INTEGER
DECLARE d : INTEGER
DECLARE cnt : INTEGER

SET cnt := 0

READ num

READ d

WHILE num > 0

x := num MOD 10

num := num / 10
IF x == d THEN
    cnt := cnt + 1
END IF
END WHILE

PRINT cnt
```

### C++ Code

```cpp

#include <iostream>
using namespace std;

int main() {
    int num, d, cnt = 0;

    cin >> num >> d;

    while(num > 0) {
        int x = num % 10;
        if(x == d)
            cnt++;
        num /= 10;
    }

    cout << cnt;
}
```

## Example Output

```
Input:
122334
3

Output:
2
```

---

# Prime Number

## Pseudocode

```
DECLARE n : INTEGER
DECLARE i : INTEGER

READ n

FOR i := 2 TO n-1
    IF n MOD i == 0 THEN
        PRINT "Not Prime"
        BREAK
    END IF
END FOR

IF i == n THEN
    PRINT "Prime"
END IF
```

## C++ Code

```cpp
#include<iostream>
usingnamespacestd;

int main() {
    int n;
    cin>>n;

    bool prime = true;

    for(int i = 2;i<n;i++) {
        if(n % i == 0) {
            prime = false;
            break;
    }
}

if(prime)
    cout<<"Prime";
else
    cout<<"Not Prime";
}
```

## Output

```
Input: 7
Output: Prime
```

---

# Fibonacci Series

## Pseudocode

```
DECLARE n : INTEGER
DECLARE prev : INTEGER
DECLARE next : INTEGER
DECLARE sum : INTEGER

SET prev := 0
SET next := 1

READ n

PRINT prev
PRINT next

WHILE sum <= n
    sum := prev + next
    PRINT sum
    prev := next
    next := sum
END WHILE
```

## C++ Code

```cpp
#include <iostream>
using namespace std;

int main() {
int n;
cin>>n;

int prev = 0, next = 1;

cout << prev <<" "<<next<<" ";

while(true) {
    int sum = prev+next;

    if(sum>n)
        break;

    cout<<sum<<" ";

    prev =next;
    next =sum;
    }
}
```

## Output

```
Input: 20
Output:
0 1 1 2 3 5 8 13
```

---

# Largest Power of 2 Using Bit Shift

## Pseudocode

```
DECLARE value : INTEGER
DECLARE n : INTEGER

SET value := 1
SET n := 45

WHILE value <= n
    value := value << 1
END WHILE

PRINT value
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int value =1;
    int n =45;

    while(value<=n) {
        value = value << 1;
    }

    cout<<value;
}
```

## Output

```
64
```

---

# Digital Root Logic

## Pseudocode

```
DECLARE x : INTEGER
SET x := 259

IF x == 0 THEN
    PRINT 0
ELSE
    IF x MOD 9 == 0 THEN
        PRINT 9
    ELSE
        PRINT x MOD 9
    END IF
END IF
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int x =259;

    if(x==0)
        cout<<0;
    elseif(x%9==0)
        cout<<9;
    else
        cout<<x%9;
}
```

## Output

```
Input: 259
Output: 7
```

---

# Loop Expression Problem

## Pseudocode

```
SET a := 2
SET b := 5
SET c := 10

FOR each c from 3 to 9
    a := (a + a) + a
    a := (a ^ 1) + c
END FOR

b := (9 + 7) + a

PRINT a + b
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
    int a =2,b =5,c =10;

    for(c =3;c<=9;c++) {
        a = (a+a)+a;
        a = (a^1)+c;
    }

    b = (9+7)+a;

    cout<<a+b;
}
```

---

# Expression Loop Example

## Pseudocode

```
DECLARE x, y

SET x := 15
SET y := 12

y := x - 1

DO
    PRINT x
    x := y + (x - 2)
WHILE x < 40
```

## C++ Code

```cpp
#include<iostream>
using namespace std;

int main() {
int x =15,y =12;

y = x-1;

do {
    cout<<x<<" ";
    x =y+ (x-2);
    }while(x<40);
}
```

## Output

```
15 27 39
```