## JavaScript Notes Summary

### Statements vs Expressions
- An **expression** "asks" JS for a value (e.g., `myAssignedVariable`, `6 + 4`, `document.getElementById("susan")`)
- A **statement** "tells" JS to do something (e.g., declare/assign a variable)
  - Examples: `let ten = 6 + 4;` and `myDeclaredVariable = "new value";`

---

### Statements include:
- Variable declarations (`let`, `var`, `const`)
- Variable assignments, `console.log()`, return statements, conditional statements (`if/else`), and loop statements (`for`)

---

### Arrays
- Arrays let us keep **multiple values together** in a single collection
- Example: `let synonyms = ["plethora", "array", "cornucopia"];`
- Like strings, arrays have a **length** → `synonyms.length`
- Each value has an **index** → `synonyms[1]`
- You can check if an array contains a value using `.includes()`
- **Unlike strings, arrays are mutable** → `synonyms[2] = "variety";`

### Key Array Methods:
- `.pop()` → removes the last element
- `.push()` → adds an element to the end
- `.sort()` → re-arranges elements alphabetically
- `.join(" ")` → joins elements into a string with a separator
- `.concat()` → combines two arrays — e.g., `[1,2,3].concat([4,5,6])` → `[1,2,3,4,5,6]`
- `.indexOf()` → finds the position of a value
- `.includes()` → returns a boolean (true/false)
- `.length` → returns the number of elements
