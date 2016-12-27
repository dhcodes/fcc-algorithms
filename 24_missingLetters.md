# Missing Letters

Find the missing letter in the passed letter range and return it.

If all letters are present in the range, return undefined.

```
function fearNotLetter(str) {

  let numArr = str.split('').map((item)=>{
    return item.charCodeAt();
    });     
  for (let i = 0; i<numArr.length-1; i++) {
    if (numArr[i]+1 !== numArr[i+1]) {
      return String.fromCharCode(numArr[i]+1);
    }

  }
};

fearNotLetter("bcd");
```
