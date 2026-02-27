## JavaScript Notes Summary

---

## Array Methods: Mutating vs Non-Mutating

| Method | Behavior | Returns |
|--------|----------|---------|
| **push()** | Modifies original array **in-place** | New length of array |
| **concat()** | Creates a **new array** without changing original | New concatenated array |

---

## Variable Declaration: `let` vs `const`

| Keyword | Reassignment Allowed? | Example |
|---------|---------------------|---------|
| **let** | ✅ Yes | Can reassign to new values |
| **const** | ❌ No | Throws error if reassigned |

**Examples:**
```javascript
// Using let
let letVariable = "original value";  // undefined
letVariable = "new value";           // ✅ Works! 'new value'

// Using const
const constVariable = "original value";  // undefined
constVariable = "new value";             // ❌ ERROR! Cannot reassign
```

---

## Key Concept: Immutable Variables with Mutable Values

**Important distinction:** `const` prevents **reassignment of the variable**, but does NOT prevent **modification of the value** (if mutable).

**Example with Array:**
```javascript
const operands = [4, 6];
const sum = operands[0] + operands[1];  // sum = 10

// This WORKS! (modifying the array contents)
operands[0] = 5;  // ✅ Allowed - array is mutated in-place
// operands is now [5, 6]
```

---

## Summary Points

- **Some actions** change the array in-place (mutating)
- **Other actions** do not mutate the original array, but instead create a new copy
- Variables themselves can be mutable (`let`) or immutable (`const`)
- **`const`** = immutable variable binding (cannot reassign)
- **`const`** with arrays/objects = you can still mutate the contents!