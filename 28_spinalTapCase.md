# Spinal Tap Case

Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.

```

function spinalCase(str) {

  return str.replace(/\B[A-Z]/g, '-' + '$&').replace(/\s|_/g, "-").replace(/--/g, "-").toLowerCase();;
}

spinalCase("thisIsSpinalTap");

```
