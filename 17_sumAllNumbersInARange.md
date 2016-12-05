# Sum All Numbers in a Range

We'll pass you an array of two numbers. Return the sum of those two numbers and all numbers between them.

The lowest number will not always come first.

```
function sumAll(arr) {
  let newArr= [];
  for (let i = Math.min(...arr); i<=Math.max(...arr); i++) {
    newArr.push(i);
  }
  return newArr.reduce((curr, next) => {
    return curr + next;
  });

}
sumAll([1, 4]);

```
