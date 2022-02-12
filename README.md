## Welcome to `return0.io`

This is going to be a website contains mainly educational resources.

### Why the name of `return0`

In Linux/Unix environment, when a program exits with a return code `0`, it indicates the program successfully exits.

### What to expect?

`Return0` will provide both fundamental computer science concept, in format of crash course and detailed explaination, programming challenges and more.

Sample leetcode question: Given two integers a and b, return the sum of the two integers without using the operators + and -.

```
def getSum(self, a: int, b: int) -> int:
    x, y = abs(a), abs(b)
    
    if x < y:
        return self.getSum(b, a)  
    sign = 1 if a > 0 else -1

    if a * b >= 0:
        while y:
            x, y = x ^ y, (x & y) << 1
    else:
        while y:
            x, y = x ^ y, ((~x) & y) << 1

    return x * sign
```

### Support or Contact

maxim[dot]sl[dot]mai[at]gmail[dot]com
