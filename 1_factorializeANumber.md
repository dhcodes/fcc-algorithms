#Factorialize a Number

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
