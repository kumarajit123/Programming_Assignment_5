## Python Basic Programming Assignment - 5
--------------


### 1. Write a Python Program to Find LCM?


```python
def lcm(a,b):
    '''
    Function which return the LCM of two number.
    '''
    high = a if a > b else b
    
    while True:
        if (high%a==0) and (high%b==0):
            break
        else:
            high += 1
            
    return high
```


```python
a = 22
b = 7

lcm(a, b)
```




    154



---------------------
### 2. Write a Python Program to Find HCF?


```python
def hcf(a, b):
    
    low = a if a < b else b
    
    for i in range(1, low+1):
        if (a%i==0) and (b%i==0):
            hcf = i
            
    return hcf
```


```python
a = 53
b = 33

hcf(a, b)
```




    1




```python
a = 52
b = 24

hcf(a, b)
```




    4



---------------
### 3. Write a Python Program to Convert Decimal to Binary, Octal and Hexadecimal?


```python
def conversion(num):
    print("Binary:      ", bin(num))
    print("Octal:       ", oct(num))
    print("Hexadecimal: ", hex(num))
```


```python
conversion(7)
```

    Binary:       0b111
    Octal:        0o7
    Hexadecimal:  0x7
    


```python
conversion(369)
```

    Binary:       0b101110001
    Octal:        0o561
    Hexadecimal:  0x171
    

---------------------
### 4. Write a Python Program To Find ASCII value of a character?


```python
try:
    char = input("Enter a character: ")
    ASCII = ord(char)
    print("ASCII value of {} is {}".format(char, ASCII))
except Exception as e:
    print(e)
```

    Enter a character: A
    ASCII value of A is 65
    

----------------
### 5. Write a Python Program to Make a Simple Calculator with 4 basic mathematical operations?


```python
try:
    
    while True:
        num1 = int(input("Enter first number: "))
        num2 = int(input("Enter second number: "))
        
        print("\nFor addition:       +")
        print("For subtraction:    -")
        print("For multiplicaton:  *")
        print("For division:       /")
        print("For Exit:            X")
        
        ch = input("\nEnter the choice for mathematical operations: ")
        
        
        if ch == '+':
            output = num1 + num2
        elif ch == '-':
            output = num1 - num2
        elif ch == '*':
            output = num1 * num2
        elif ch == '/':
            output = num1 / num2
        
        if ch == 'X' or ch == 'x':
            break
            
        print("\nResult: ", output)
        
        
            
except Exception as e:
    print(e)
```

    Enter first number: 189
    Enter second number: 9
    
    For addition:       +
    For subtraction:    -
    For multiplicaton:  *
    For division:       /
    For Exit:            X
    
    Enter the choice for mathematical operations: /
    
    Result:  21.0
    Enter first number: 123
    Enter second number: 3
    
    For addition:       +
    For subtraction:    -
    For multiplicaton:  *
    For division:       /
    For Exit:            X
    
    Enter the choice for mathematical operations: *
    
    Result:  369
    Enter first number: 12
    Enter second number: 3
    
    For addition:       +
    For subtraction:    -
    For multiplicaton:  *
    For division:       /
    For Exit:            X
    
    Enter the choice for mathematical operations: X
    


```python

```
