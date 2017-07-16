# Javascript
JavaScript is a programming language that is run by most modern browsers. It supports object-oriented programming and procedural programming. It can be used to control web pages on the client side of the browser, server-side programs, and even mobile applications.

## Add/Remove st, nd, rd and th (ordinal) suffix to numbers
The rules are as follows:

```HTML
st is used with numbers ending in 1 (e.g. 1st, pronounced first)
nd is used with numbers ending in 2 (e.g. 92nd, pronounced ninety-second)
rd is used with numbers ending in 3 (e.g. 33rd, pronounced thirty-third)
As an exception to the above rules, all the "teen" numbers ending with 11, 12 or 13 use -th 
    (e.g. 11th, pronounced eleventh, 112th, pronounced one hundred [and] twelfth)
th is used for all other numbers (e.g. 9th, pronounced ninth).
```
(Note: A number suffix is a letter that might come after an address if there aren't enough numbers for all the buildings on a street. (For example, if your address is 9A Main Street, the suffix would be "A".))

```Javascript

// Function to : 
//   Add Ordinal Suffix to numbers
function addOrdinalNumberSuffix(num) {
    var j = num % 10,
        k = num % 100;
    if (j == 1 && k != 11) {
        return num + "st";
    }
    if (j == 2 && k != 12) {
        return num + "nd";
    }
    if (j == 3 && k != 13) {
        return num + "rd";
    }
    return num + "th";
}

// Function to : 
//   Remove Ordinal Suffix from numbers
function removeOrdinalNumberSuffix(numStr) {
    var outputStr = numStr.replace(/(\d+)(st|nd|rd|th)/g, "$1");  
  
    return outputStr;
}
```

## Refrence 
* https://regex101.com/r/pN4oG0/1
* http://eloquentjavascript.net/09_regexp.html

<hr align="center" width="50%">
<hr align="center" width="60%">

# Session expiration


