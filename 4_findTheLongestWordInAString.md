#Find the Longest Word in a String

Return the length of the longest word in the provided sentence.

Your response should be a number.

```
function findLongestWord(str) {
  let arr=str.split(' ');
  let numArr = arr.map((item) => {
    return item.length;

  });
  return numArr.sort((a,b)=>{
  return b - a;
  }).shift();
}
findLongestWord("May the force be with you.");
```
