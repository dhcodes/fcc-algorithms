# Chunky Monkey

Write a function that splits an array (first argument) into groups the length of size (second argument) and returns them as a two-dimensional array.

```
function chunkArrayInGroups(arr, size) {
  let chunkedArr = [];
  while (arr.length > size) {
    chunkedArr.push(arr.splice(0, size));
  }
  chunkedArr.push(arr);
  return chunkedArr;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);
```
