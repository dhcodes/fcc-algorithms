#Factorialize a Number

Return the factorial of the provided integer.

If the integer is represented with the letter n, a factorial is the product of all positive integers less than or equal to n.

Factorials are often represented with the shorthand notation <code>n!</code>

For example: <code>5! = 1 * 2 * 3 * 4 * 5 = 120</code>

```
function factorialize(num) {
  let val = 1;
  for (let i=1; i<=num; i++) {
    val*=i;
  }
  return val;
}

factorialize(5);
```
