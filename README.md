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

## Semantic HTML

- Semantic HTML describes the meaning of elements to both the browser and developers.
- It refers to using specific tags like `<header>`, `<footer>`, `<nav>`, `<article>`, `<section>`, etc., to provide clearer structure and meaning to web content.
- Helps define the type of content it contains, which improves **accessibility**.
- Common semantic tags include:  
  `heading`, `nav`, `section`, `form`, `summary`, `article`, `details`

---

## Web Accessibility

- Web accessibility ensures that applications can be accessed by as many people as possible, including those with low vision or color blindness.
- Achieved by:
  - Using semantic HTML tags
  - Maintaining correct HTML structure
  - Using ARIA attributes like `aria-label`, `aria-role`, etc.

---

## Metadata

- Metadata describes the content of the page.
- Metadata does **not** appear visually on the page but is included in the page source.
- Helps search engines understand the content of the page for better SEO.
  
### Important SEO-related Metadata Tags:
- Meta title tag
- Meta description tag
- Headings
- Semantic tags
- Image alternative text (`alt` attribute)

---

## Iframe

- An `<iframe>` is used to display one webpage inside another webpage.

---

## HTML Elements: Block vs Inline

- **Block-level elements**  
  - Occupy full width of their parent container by default.  
  - Always start on a new line, pushing subsequent elements below.  
  - Examples: `<div>`, `<p>`, `<h1> - <h6>`, `<section>`, `<article>`

- **Inline elements**  
  - Only take up as much width as their content requires.  
  - Do not start on a new line; flow inline with text.  
  - Examples: `<span>`, `<a>`, `<strong>`, `<input>`, `<img>`, `<label>`, `<button>`, `<select>`

---

## Synthetic Events

- Synthetic Events in React are cross-browser wrappers around the browser's native events.
- They provide a consistent interface for event handling across different browsers.

