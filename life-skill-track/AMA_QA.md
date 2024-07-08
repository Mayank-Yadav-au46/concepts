---

**Q.1 What is the difference between (==) and (===) operator ?**    
**Ans:** The `==` operator compares the data only without comparing datatypes, but `===` operator compares datatype as well along with the value. Flaws of `==`:
```javascript
0 == false       // true
5 == "5"         // true
null == undefined // true
0 == ""          // true
```
---

**Q.2 Console.log(typeof []) is equals to 'object' why?**    
**Ans:** `typeof []` returns 'object' because arrays are a specialized type of object in JavaScript.



---

**Q.3) What are the disadvantages of using closure?**    
**Ans:** Closures can use more memory because they keep variables around even after the outer function finishes. They can also make your code harder to debug and understand.

---

**Q.4) Why using global variables are bad in JavaScript?**    
**Ans:** Using global variables in JavaScript is bad because they can be changed from anywhere in the code, leading to bugs and conflicts that are hard to track.

---

**Q.5)How to extract certain properties from an array of objects to create a new array?**  
**Ans:** Use the map method to create a new array by extracting the desired properties from each object.
Difference between charAt() and at() method in JS?

---

**Q.6)Difference between charAt() and at() method in js ?**  
**Ans:**charAt() returns the character at a specified index, while at() allows for negative indexing to access characters from the end of the string.

---

**Q.8)**How to reset the initial or 1st commit in Git, if possible?  
**Ans:** You can use git rebase -i --root to interactively edit the first commit, or git reset --hard to reset the repository to a specific commit.

---

**Q.9)**Why does console.log(typeof []) return 'object', yet we can't use the . operator on arrays like objects?  
**Ans:** Arrays are a type of object, but they use numerical indexing instead of named properties, so array elements are accessed with square brackets.

---

**Q.10)**Why does forEach loop skip undefined values whereas for loop does not?  
**Ans:** forEach skips holes in sparse arrays (elements that haven't been explicitly assigned), while for loops iterate over all indices.

---

**Q.11)**How can we mimic the action of Array.splice and Array.slice on objects?  
**Ans:** Use Object.keys and Object.values with methods like slice and splice to work with objects as if they were arrays.

---

**Q.12)**What is the "Callback Hell" problem and how to avoid it?  
**Ans:** "Callback Hell" is the difficulty in reading and maintaining code with many nested callbacks; it can be avoided using Promises or async/await.

---

**Q.13)**
let ar = [1,2,3];
console.log("Hello");
module.exports.ar = ar;

//file2.js
const {ar} = require('file1.js');
let print = ar;
console.log(print);

Output: "Hello" 
                [1,2,3]
why "Hello" is also printing ? when we have exported array('ar') only!  
**Ans:** When you require file1.js in file2.js, Node.js runs all the top-level code in file1.js, including the console.log("Hello"); statement. This is why "Hello" is printed. The module.exports.ar = ar; then makes the array available to file2.js, which prints [1, 2, 3].

---

