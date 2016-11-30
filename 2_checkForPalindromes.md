#Check for Palindromes

```
function palindrome(str) {
  // Good luck!
  //Remember the oldstring
  let newStr = str.replace(/\W|\s|_|\./g,'').toLowerCase();
  let revStr = str.replace(/\W|\s|_|\./g,'').split('').reverse().join('').toLowerCase();

  return newStr === revStr;
}
palindrome("A man, a plan, a canal. Panama");
```
