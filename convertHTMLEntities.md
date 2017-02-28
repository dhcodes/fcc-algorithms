# Convert HTML Entities

Convert the characters &, <, >, " (double quote), and ' (apostrophe), in a string to their corresponding HTML entities.

```
function convertHTML(str) {
  // &colon;&rpar;
 return str.split("").map((item)=> {
   switch(item) {
     case "&":
       item = "&amp;";
       break;
     case "<":
       item = "&lt;";
       break;
     case ">":
       item = "&gt;";
       break;
     case '"':
       item = "&quot;";
       break;
     case "'":
       item = "&apos;";
       break;
  }
   return item;
 }).join("");
}
convertHTML("Dolce & Gabbana");
```
