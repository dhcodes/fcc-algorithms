# Caesar's Cipher

One of the simplest and most widely known ciphers is a Caesar cipher, also known as a shift cipher. In a shift cipher the meanings of the letters are shifted by some set amount.

A common modern use is the ROT13 cipher, where the values of the letters are shifted by 13 places. Thus 'A' ↔ 'N', 'B' ↔ 'O' and so on.

Write a function which takes a ROT13 encoded string as input and returns a decoded string.

All letters will be uppercase. Do not transform any non-alphabetic character (i.e. spaces, punctuation), but do pass them on.

```

function rot13(str) { // LBH QVQ VG!
  let strArr = str.split('');
  let decodedArr = strArr.map((letter) => {
    if (letter.charCodeAt() < 65 || letter.charCodeAt() >90) {
      return letter;
    }
    else {
    let newLetter = letter.charCodeAt() + 13 > 90 ?  letter.charCodeAt() - 13 : letter.charCodeAt() + 13;  
    return String.fromCharCode(newLetter);
    }
  });
  return decodedArr.join('');
}

// Change the inputs below to test
rot13("SERR CVMMN!");

```
