# Python Operators
In Python programming, Operators in general are used to perform operations on values and variables.

----------------------

## Types of Operators in Python

|  Type | Operators |
|----------|----------|
| Arithmetic Operators | + , - , * , / , // , ** , %  | 
| Relational Operators | < , > , <= , >= , == , !=  | 
| Logical Operators | AND , OR , NOT  | 
| Bitwise Operators | & , \| , ^ , ~ , << , >> | 
| Assignment Operators |  += , -= , *= , %= , = | 
| Unaru Operators | +x, -x, ~x |
----------------------

## Arithmatic Operators
They perform basic mathematical operations
| Arithematic Operator | Code | Output |
|----------------------|-------------------------------|-------------------------------|
| + | `a,b = 10,5`<br>`print("Addition :",a+b`) | Addition = 15 |
| - | `a,b = 10,5`<br>`print("Substraction :",a-b`) | Substraction = 5 |
| * | `a,b = 10,5`<br>`print("Multiplication :",a*b`) | Multiplication = 50 |
| / | `a,b = 9,5`<br>`print("Division :",a/b`) | Division = 1.8 |
| // | `a,b = 9,5`<br>`print("Floor Division :",a//b`) | Floor Division = 1 |
| % | `a,b = 6,5`<br>`print("Modulus :",a%b`) | Modulus = 1 |
| ** | `a,b = 2,3`<br>`print("Exponentiation :",a**b`) | Exponentiation = 8 |

----------------------

## Relational Operators
They are used to **compare two values** and return `True` or `False`.

| Relational Operator | Meaning | Code | Output |
|--------------------|---------|-------------------------------|----------------|
| `==` | Equal to | `a,b = 10,5`<br>`print(a == b)` | False |
| `!=` | Not equal to | `a,b = 10,5`<br>`print(a != b)` | True |
| `>` | Greater than | `a,b = 10,5`<br>`print(a > b)` | True |
| `<` | Less than | `a,b = 10,5`<br>`print(a < b)` | False |
| `>=` | Greater than or equal to | `a,b = 10,10`<br>`print(a >= b)` | True |
| `<=` | Less than or equal to | `a,b = 5,10`<br>`print(a <= b)` | True |

----------------------

## Logical Operators
They are used to combine conditional statements

| Logical Operator | Code | Output |
|------------------|-------------------------------|-------------------------------|
| and | `a,b = True, False`<br>`print("AND :", a and b)` | AND : False |
| or | `a,b = True, False`<br>`print("OR :", a or b)` | OR : True |
| not | `a = True`<br>`print("NOT :", not a)` | NOT : False |

----------------------

## Bitwise Operators
They perform operations on **binary representations (bits)** of numbers.

### Binary Representation
| Decimal | Binary |
|--------|--------|
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |

### Bitwise AND (`&`)
Returns `1` if **both bits are 1**

| Operator | Code | Output |
|---------|-------------------------------|----------------|
| & | `a,b = 5,3`<br>`print("AND :", a & b)` | AND : 1 |

**Bit Computation:**
```text
5 → 0101

3 → 0011

--------

    0001
    
--------

0001 ----> 1
```

### Bitwise OR (`|`)

Returns `1` if **any one bit is 1**

| Operator | Code | Output |
|---------|-------------------------------|----------------|
| \| | `a,b = 5,3`<br>`print("OR :", a | b)` | OR : 7 |

**Bit Computation:**
```text
5 → 0101
3 → 0011
--------
    0111
--------

0111 ----> 7
```

### Bitwise XOR (`^`)

Returns `1` if **bits are different**

| Operator | Code | Output |
|---------|-------------------------------|----------------|
| ^ | `a,b = 5,3`<br>`print("XOR :", a ^ b)` | XOR : 6 |

**Bit Computation:**
```text
5 → 0101
3 → 0011
--------
    0110
--------

0110 ----> 6
```

### Bitwise NOT (`~`)

Inverts all bits (0 → 1, 1 → 0)

| Operator | Code | Output |
|---------|-------------------------------|----------------|
| ~ | `a = 5`<br>`print("NOT :", ~a)` | NOT : -6 |

**Bit Computation:**
```text
5 → 00000101
~5 → 11111010
```

Formula:

~n = -(n + 1)

### Left Shift (`<<`)

Shifts bits to the **left** 

| Operator | Code | Output |
|---------|-------------------------------|----------------|
| << | `a = 5`<br>`print("Left Shift :", a << 1)` | Left Shift : 10 |

**Bit Computation:**

#### 5 << 1

1) Original number
   
   5 --> 0101
   
3) Shift left by 1 position
   
   0101 << 1
   
   0101 --> 1010
   
5) Convert back to decimal

   1010 --> 10

#### 5 << 2

1) Original number
   
   5 --> 0101
   
3) Shift left by 2 position
   
   0101 << 2
   
   0101 --> 10100
   
5) Convert back to decimal
   
   10100 --> 20

#### Formula

a << n = a × (2ⁿ)

So:

-5 << 1 = 5 × 2 = 10

-5 << 2 = 5 × 4 = 20

### Right Shift (`>>`)

Shifts bits to the **right**

| Operator | Code | Output |
|---------|-------------------------------|----------------|
| >> | `a = 5`<br>`print("Right Shift :", a >> 1)` | Right Shift : 2 |

**Bit Computation:**

#### 5 >> 1

1) Original number
   
   5 --> 0101
   
3) Shift Right by 1 position
   
   0101 << 1
   
   0101 --> 0010
   
5) Convert back to decimal
   
   0010 --> 2

#### 5 >> 2

1) Original number
   
   5 --> 0101
   
3) Shift left by 2 position
   
   0101 << 2
   
   0101 --> 0001
   
5) Convert back to decimal
   
   10100 --> 1

#### Formula

a >> n = a // (2ⁿ)

So:

- 5 >> 1 = 5 // 2 = 2

- 5 >> 2 = 5 // 4 = 1

----------------------

## Assignment Operators
They are used to **assign values to variables**.

| Assignment Operator | Meaning | Code | Output |
|--------------------|---------|-------------------------------|----------------|
| `=` | Assign | `a = 5`<br>`print(a)` | 5 |
| `+=` | Add and assign | `a = 5`<br>`a += 3`<br>`print(a)` | 8 |
| `-=` | Subtract and assign | `a = 5`<br>`a -= 2`<br>`print(a)` | 3 |
| `*=` | Multiply and assign | `a = 5`<br>`a *= 2`<br>`print(a)` | 10 |
| `/=` | Divide and assign | `a = 10`<br>`a /= 2`<br>`print(a)` | 5.0 |
| `//=` | Floor divide and assign | `a = 10`<br>`a //= 3`<br>`print(a)` | 3 |
| `%=` | Modulus and assign | `a = 10`<br>`a %= 3`<br>`print(a)` | 1 |
| `**=` | Exponent and assign | `a = 2`<br>`a **= 3`<br>`print(a)` | 8 |

----------------------

## Unary Operators
Unary operators operate on **a single operand**.

| Unary Operator | Meaning | Code | Output |
|---------------|---------|-------------------------------|----------------|
| `+` | Unary plus (returns the value as it is) | `a = 5`<br>`print(+a)` | 5 |
| `-` | Unary minus (negates the value) | `a = 5`<br>`print(-a)` | -5 |
| `~` | Bitwise NOT (inverts bits) | `a = 5`<br>`print(~a)` | -6 |
| `not` | Logical NOT (negates boolean value) | `a = True`<br>`print(not a)` | False |


## Precedence and Associativity of Operators

### Operator Precedence
Operator precedence determines **which operator is evaluated first** in an expression.

### Operator Associativity
Operator associativity determines **the order of evaluation when operators have the same precedence**.

---

### Precedence and Associativity Table

| Operator | Description | Associativity |
|---------|-------------|---------------|
| `()` | Parentheses | Left to Right |
| `**` | Exponentiation | Right to Left |
| `+x`, `-x`, `~x` | Unary plus, minus, bitwise NOT | Right to Left |
| `*`, `/`, `//`, `%` | Multiplication, Division, Floor Division, Modulus | Left to Right |
| `+`, `-` | Addition, Subtraction | Left to Right |
| `<<`, `>>` | Bitwise shift | Left to Right |
| `&` | Bitwise AND | Left to Right |
| `^` | Bitwise XOR | Left to Right |
| `|` | Bitwise OR | Left to Right |
| `==`, `!=`, `<`, `>`, `<=`, `>=` | Relational operators | Left to Right |
| `is`, `is not` | Identity operators | Left to Right |
| `in`, `not in` | Membership operators | Left to Right |
| `not` | Logical NOT | Right to Left |
| `and` | Logical AND | Left to Right |
| `or` | Logical OR | Left to Right |
| `=` , `+=`, `-=`, `*=`, `/=` | Assignment operators | Right to Left |
