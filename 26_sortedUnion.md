# Sorted Union

Write a function that takes two or more arrays and returns a new array of unique values in the order of the original provided arrays.

In other words, all values present from all arrays should be included in their original order, but with no duplicates in the final array.

The unique numbers should be sorted by their original order, but the final array should not be sorted in numerical order.

```

function uniteUnique(arr) {

  let args = Array.from(arguments);
  let joinedArr = args.reduce((a, b)=> {
    return a.concat(b);
  });
  let newArr = [];
  for (let i = 0; i<joinedArr.length; i++) {
    if (newArr.indexOf(joinedArr[i])== -1) {
      newArr.push(joinedArr[i]);
    }
  }
  return newArr;
}

uniteUnique([1, 3, 2], [1, [5]], [2, [4]]);

```
