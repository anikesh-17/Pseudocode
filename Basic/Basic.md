Pseudocode → Combination of natural language and elements of programming language.

- Keywords
- Identifiers
- Literals
- Constants
- Data Types : Valued + allowed operations
    - Set of values and allowed operations on that value
    - INTEGER, REAL, CHAR, STRING, BOOLEAN, DATE
- Variable

---

### Add 2 Numbers

> DECLARE x : INTEGER
DECLARE y : INTEGER
DECLARE z : INTEGER
READ x
READ y
z := x + y
PRINT z
> 

```cpp
# include <bits/stdc++.h>
using namespace std;
int main(){
    int x;
    int y;
    int z;
    cin >>x;
    cin>>y;
    z = x + y;
    cout << z << endl;
    return 0;
}
```

### Read a number and print square and cube

> DECLARE x : INTEGER
DECLARE y : INTEGER
DECLARE z : INTEGER
READ x
y := x * x
z := x * x * x
PRINT y
PRINT z
> 

```cpp
# include <bits/stdc++.h>
using namespace std;
int main(){
    int x;
    int y;
    int z;
    cin >>x;
    y = x * x;
    z = x * x * x;
    cout << y << endl;
    cout << z << endl;
    return 0;
}
```

### Area and Perimeter of Rectangle

> 
> 
> 
> DECLARE length : REAL
> DECLARE breadth : REAL
> DECLARE area : REAL
> DECLARE peri : REAL
> 
> READ length
> READ breadth
> 
> area := length * breadth
> peri := 2 * (length + breadth)
> 
> PRINT area
> PRINT peri
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    float length, breadth, area, peri;

    cout << "Enter length: ";
    cin >> length;

    cout << "Enter breadth: ";
    cin >> breadth;

    area = length * breadth;
    peri = 2 * (length + breadth);

    cout << "Area = " << area << endl;
    cout << "Perimeter = " << peri << endl;

    return 0;
}
```

### **Volume of Sphere**

> 
> 
> 
> DECLARE radius : REAL
> DECLARE volume : REAL
> CONSTANT PI = 3.14
> 
> READ radius
> 
> volume := (4/3) * PI * radius * radius * radius
> 
> PRINT volume
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    float radius, volume;
    const float PI = 3.14;

    cout << "Enter radius: ";
    cin >> radius;

    volume = (4.0/3.0) * PI * radius * radius * radius;

    cout << "Volume of sphere = " << volume << endl;

    return 0;
}
```

### Set / Initialize Integer

> 
> 
> 
> DECLARE x : INTEGER
> 
> SET x := 5
> 
> x := x + 5
> 
> PRINT x
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int x;

    x = 5;
    x = x + 5;

    cout << "Value of x = " << x << endl;

    return 0;
}
```

### Increment and Decrement

Increment

> 
> 
> 
> SET x := 10
> INCREMENT x
> PRINT x
> 

Decrement

> 
> 
> 
> SET x := 10
> DECREMENT x
> PRINT x
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 10;

    // Increment
    x++;
    cout << "After increment: " << x << endl;

    // Decrement
    x--;
    cout << "After decrement: " << x << endl;

    return 0;
}
```

### Write a pseudocode to find Remainder and Division of Two Numbers

> 
> 
> 
> DECLARE a : INTEGER
> DECLARE b : INTEGER
> DECLARE rem : INTEGER
> DECLARE div : INTEGER
> 
> READ a
> READ b
> 
> rem := MOD(a, b)
> div := a / b
> 
> PRINT rem
> PRINT div
> 

```cpp
#include <iostream>
using namespace std;

int main()
{
    int a, b;
    int rem, div;

    cout << "Enter first number: ";
    cin >> a;

    cout << "Enter second number: ";
    cin >> b;

    rem = a % b;   
    div = a / b;     

    cout << "Remainder = " << rem << endl;
    cout << "Division = " << div << endl;

    return 0;
}
```