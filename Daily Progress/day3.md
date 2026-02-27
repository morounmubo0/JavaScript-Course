### JavaScript Notes Summary

---

## Mutable vs Immutable Data Types

### **Mutable Data**
- Can be changed during program execution
- **Example:** Arrays
- In JavaScript, you can modify an array's element by directly assigning a new value to a specific index
- Example: `abcArray[0] = "d"` replaces the element at that index

**Example of Mutable Array:**
```javascript
let abcArray = ['a', 'b', 'c', 3];
abcArray[0] = 'd';  // Modifies the original array
```

---

### **Immutable Data**
- Cannot be modified once created
- **Primitive data types** are immutable (string, boolean, number)
- When attempting to modify an immutable type, the original value remains unchanged

**Example with Primitive (Immutable):**
```javascript
let numbers1 = [1, 2, 3];
let result1 = numbers1.push(4);  // This actually MUTATES the array
// numbers1 becomes [1, 2, 3, 4]
```

**Example with Concat (Non-mutating):**
```javascript
let numbers2 = [1, 2, 3];
let result2 = numbers2.concat([4]);  // Creates NEW array, original unchanged
// numbers2 remains [1, 2, 3]
// result2 is [1, 2, 3, 4]
```

---

### **Key Takeaway**
- Some methods **mutate** the original array (e.g., `push()`)
- Some methods return a **new array** without changing the original (e.g., `concat()`)

