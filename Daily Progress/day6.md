## JavaScript Notes Summary


### 1. **Creating Objects with Properties**

You learned to create objects representing people with various property types:

| Property Type | Example |
|-------------|---------|
| **Strings** | `name: "Anjana"`, `home: "San Francisco"` |
| **Arrays** | `languages: ["English", "German", "French"]` |
| **Null** | `pet: null` |
| **Nested objects** | Complex structures with multiple levels |

**Two example objects created:**
- `anjana` — from San Francisco, speaks 3 languages, rides a Vespa, enjoys travel/climbing/gaming/Lindy hop
- `aoishah` — from Lagos, Nigeria, speaks English/Arabic/Yoruba, has a cat, hobbies include reading/motivating/coding/exploring

---

### 2. **Object Methods & The `this` Keyword**

- **Methods** = functions stored as object properties
- **`this`** = refers to the object the method belongs to

```javascript
// Example: Dog object with speak method
const dog = {
    name: "Fin",
    breed: "corgi",
    speak: function() {
        console.log("woof woof");
    }
};

// Using 'this' to access other properties
anjana.speak = function() {
    console.log("Hi my name is " + this.name);
};
```

---

### 3. **Nested Objects**

Objects containing other objects:

```javascript
const menu = {
    lunch: {
        appetizer: "salad",
        main: "spaghetti",
        dessert: "tiramisu"
    },
    dinner: {
        appetizer: "samosa",
        main: "saag paneer",
        dessert: "gulab jamun"
    }
};

// Access nested properties: menu.lunch.dessert
```

---

### 4. **Arrays of Objects**

```javascript
const spices = [
    {name: "Emma", nickname: "Baby"},
    {name: "Geri", nickname: "Ginger"},
    {name: "Mel B", nickname: "Scary"},
    {name: "Mel C", nickname: "Sporty"},
    {name: "Victoria", nickname: "Posh"}
];
```

---

### 5. **Spice Girls Object Exercise**

Complex object combining arrays and nested data:

```javascript
const spiceGirls = {
    albums: ["Spice", "Spiceworld", "Forever"],
    motto: "Girl power",
    members: spices  // array from above
};
```

**Practice questions you solved:**
- Get motto: `spiceGirls.motto`
- Get "Ginger" object: `spiceGirls.members[1]`
- Get "Spiceworld" album: `spiceGirls.albums[1]`
- Get "Victoria": `spiceGirls.members[4].name`

---

### 6. **Console Methods**

| Method | Purpose |
|--------|---------|
| `console.log()` | General output |
| `console.log(document.querySelector("h1").textContent)` | Display element content |
| `console.warn()` | Warning messages |
| `console.error()` | Error messages |
| `console.clear()` | Clear console |

---

### 7. **Math Object**

```javascript
let randomNumber = Math.random();      // 0 to 1
const pi = Math.PI;                    // 3.14159...
const five = Math.abs(-5);             // 5 (absolute value)
```

---

### 8. **Strings & Wrapper Objects**

- Strings are **primitive values** (not objects)
- JavaScript **auto-wraps** them in temporary String objects when using methods

```javascript
const hello = "hello";
console.log(hello.length);           // 5
const yello = hello.toUpperCase();   // "HELLO"
```

---

### 9. **DOM Manipulation (Tic-Tac-Toe Project)**

```javascript
// Selecting elements
document.getElementById("p1-name").textContent    // get content
document.getElementsByClassName("square")         // by class
document.querySelectorAll(".square")              // CSS selector

// Modifying content
squares[4].textContent = "X";
squares[6].textContent = player[1].symbol;
```

---

### 10. **Key Concepts Highlighted**

| Concept | Explanation |
|---------|-------------|
| `Object.freeze()` | Makes object immutable (no changes/additions) |
| Spread syntax `...` | For copying/expanding objects |
| Dot notation | `object.property` to access values |
| Bracket notation | `object["property"]` alternative access |

---

**Overall:** These notes progress from basic object creation → methods → nesting → arrays → practical DOM manipulation, building toward a Tic-Tac-Toe game project. Well-structured learning path! 🎯