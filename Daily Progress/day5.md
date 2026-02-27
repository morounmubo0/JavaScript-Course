# JavaScript Notes Summary

---

## What are Objects?

Objects collect multiple values together to describe more complex data. They let us point at related values using **properties**.

---

## Creating Objects

Objects use curly braces `{}` with **key-value pairs** separated by colons, and different properties separated by commas.

**Example:**
```javascript
const js = {
  name: "JavaScript",
  abbreviation: "JS",
  isAwesome: true,
  officialSpec: "ECMAScript",
  birthYear: 1995,
  creator: "Brendan Eich"
};
```

---

## Accessing Property Values (Dot Notation)

Use **dot notation** to access values collected as properties of an object.

```javascript
js.name        // "JavaScript"
js.isAwesome   // true
```

**Using property values in expressions:**
```javascript
js.name.startsWith("Java")     // true
let age = 2022 - js.birthYear; // 27
```

---

## Setting/Modifying Property Values

Object properties in JavaScript are **mutable** — you can modify and reassign them.

```javascript
const indecisive = {
  lunch: "Sandwich"
};

// Modify existing property
indecisive.lunch = "tacos";

// Add new property
indecisive.snack = "chips";
```

---

## Key Points

| Concept | Description |
|---------|-------------|
| **Syntax** | `{}` with `key: value` pairs |
| **Access** | Dot notation: `object.property` |
| **Mutability** | Object properties are mutable |
| **Modification** | Change existing values or add new properties using dot notation |
| **String methods** | Can call string methods directly on object properties that contain strings (e.g., `js.name.startsWith()`) |

---

## Reference vs Value (Diagram Explanation)

The notes include a diagram showing that when you assign one array to another variable, both variables **point to the same memory location**. Modifying one affects both:

```javascript
// Both array1 and array2 point to [1, 2, 3]
array1[1] = 4;  // Changes the shared array
// Now both see [1, 4, 3]
```
