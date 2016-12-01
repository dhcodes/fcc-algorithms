#Title Case a Sentence

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.

For the purpose of this exercise, you should also capitalize connecting words like "the" and "of".

```
function titleCase(str) {
  let strArr = str.toLowerCase().split(' ').map((item)=>{
    return item.replace(item.charAt(0), item.charAt(0).toUpperCase());
  });

  return strArr.join(' ');

}

titleCase("I'm a little tea pot");
```
