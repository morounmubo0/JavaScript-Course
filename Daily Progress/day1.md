# JavaScript Notes Summary

## DOM Selection Methods
- **`document.getElementById("id")`** – gets the first element with that ID
- **`document.querySelector("#id")`** – same as above
- **`document.getElementsByTagName("h1")`** – gets all elements with that tag
- **`document.querySelectorAll("h1")`** – gets all matching elements
- **`document.getElementsByClassName("player")`** – gets all elements with that class
- **`document.body.children`** – gets all children inside the body tag

## Manipulating Content
- **`.textContent`** – reads or sets text inside an element
- **`.append("text")`** – adds text to existing content
- **`document.title = "My page"`** – changes the page title

---

## Values & Data Types
JS has two kinds of data: **Primitive types** and **Objects**

**Primitive types:** String, Number, Boolean, Undefined, Null
- **Booleans** → true/false values
- **Undefined** → accidentally nothing
- **Null** → deliberately nothing

---

## Strings
- Made up of **characters**, each with an **index** starting at 0
- `"ALOHA"[0]` → `"A"`
- `.length` → number of characters
- `.indexOf("L")` → returns index `1`
- `.includes("HA")` → `true`
- `.startsWith("AL")` → `true`
- `"ALOHA" + "!"` → `"ALOHA!"`
- `.toLowerCase()` → converts to lowercase
- `.toUpperCase()` → converts to uppercase

---

## Operators
**Arithmetic:** `+`, `-`, `*`, `/` (follows BODMAS/PEMDAS order)

**Comparison:** `>`, `<`, `>=`, `<=`

**Equality:**
| Strict | Loose |
|--------|-------|
| `===` | `==` |
| `!==` | `!=` |
- Strict checks **type + value**; loose only checks **value** (so `1 == "1"` is `true`)

**Expressions** → resolve/evaluate to a value (e.g. `4/2*10`, `5>4`)

---

## Variables
- **`let`** – declares a variable (reassignable), introduced in ES2015
- **`const`** – declares a constant (cannot be reassigned)
- **`var`** – older keyword, less predictable scoping

```js
let myVar = "so value, much wow";
const myConst = "Never gonna give you up";
```

- Variables are **pointers/references** to values, not containers
- When you do `let busta = scrub`, both point to the **same value**
- Reassigning `scrub` later does **not** change `busta`

---
