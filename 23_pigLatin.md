# Pig Latin

Translate the provided string to pig latin.

Pig Latin takes the first consonant (or consonant cluster) of an English word, moves it to the end of the word and suffixes an "ay".

If a word begins with a vowel you just add "way" to the end.

Input strings are guaranteed to be English words in all lowercase.

```
function translatePigLatin(str) {
  if (/a|e|i|o|u/.exec(str[0])) {
    return str + 'way';
  }
  let clip = (/a|e|i|o|u/.exec(str).index);
  return str.substr(clip, str.length) + str.substr(0, clip) + 'ay';
}

translatePigLatin("glove");
```
