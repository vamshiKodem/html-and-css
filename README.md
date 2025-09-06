# html-and-css

## Important Topics
- Why use **Axios** rather than **fetch** internally, features it provides
- Redux middleware internally
- Why use `useReducer` vs `useState` internally; can we use `useReducer` in component vs why `useState` is slow with complex state
- How **React Context** works internally
- Features of **Next.js**

---

## Namaste React Links
- [Link 1](https://mega.nz/folder/9jxU1DAA#-wIk88IWNsQ8mifA-6ijXg)
- [Link 2](https://mega.nz/folder/nYRRSIIL#Xn_v-8h7d4QUAWX0nV9oFg)

## Code with Mosh
- [Code with Mosh](https://mega.nz/folder/8stDDQ7J#_mPKY8XOQ4UbaUJ5rV0WBw)

---

## Important Notes
- These features allow you to manage multiple packages within a single repository, often referred to as a **monorepo**. This setup is particularly useful for large projects that consist of multiple interdependent packages.
- The dependencies section includes packages with the `"workspace:*"` protocol. This indicates these packages are part of the workspace and should be linked locally rather than fetched from npm.

**Note:**
- `interface` gives the shape of the object or state.
- `type` is similar to interface.
- We can have union and intersection types in `type`.

---

# HTML

- `DOCTYPE` represents the type of document.
- HTML5 is more sophisticated compared to HTML4, including features like:
  - Local storage
  - Semantic elements
  - Web workers
  - Geolocation
  - Canvas
  - Drag and drop
  - WebSocket
- HTML structure:
  - `<html>` element contains `<head>`, `<body>`, and `<script>`
  - `<head>` contains metadata, title, styles, etc.
  - `<body>` contains the actual content.
- Different types of inputs: text, button, checkbox, color picker, date, file, email, etc.

### Custom Attributes in React JSX
```jsx
<div data-status="active">Active Item</div>
<div data-status="inactive">Inactive Item</div>

/* CSS targeting */
div[data-status="active"] {
  background-color: green;
  color: white;
}

div[data-status="inactive"] {
  background-color: gray;
  color: white;
}



