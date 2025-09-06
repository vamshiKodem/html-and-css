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
```

**Semantic HTML**

- Semantic HTML describes its meaning to both the browser and developer.
- refers to the use of specific tags like ` <header>, <footer>, <nav>, <article>, <section>,` etc., to provide clearer structure and meaning to web content
- It will give the type of content it will have which is also good for accessibility
- Heading, nav, section, form, summary, article, details

**Web Accessibility**

- Web accessibility will give the power to access the application to as many people as possible for example people with low vision, and color blindness.
- Using semantic tags, correct structure of HTML, using aria labels, aria type, and so on.

**Metadata**

- Metadata will describe the content of the page. Metadata won’t appear on the page but it will be in the source
- With metadata search engines will know the content of the page
  Search engine optimization using tags
  Tags that improve the SEO are

  - Meta title tag
  - Meta description tag
  - Heading
  - Semantic tags
  - Image alternative text
    Iframe
  - Iframe is used to display a webpage inside another webpage

- In HTML, a block-level element is an element that occupies the full width of its parent container (by default) and starts on a new line, pushing other elements below it (div, p, h1 - h6, section, article...)

- Inline elements in HTML are elements that do not start on a new line and only take up as much width as their content requires. (span, link, a, strong, input, img, label, button, select....)
- SyntheticEvents are a cross-browser wrapper around the browser's native event.

# CSS

- Inline styles have the highest priority, overriding any styles defined in internal or external style sheets.
- **Margin** creates space _around_ elements.
- **Padding** creates space _inside_ elements, between the content and the border.

---

## Difference between `class` and `id`

- Both are used to select and manipulate elements for styling, text update, or value access.
- **Class** can be used on multiple elements.
- **ID** should be unique per page.
- **Transition** is a CSS property that animates changes in CSS properties smoothly over time.

---

## Box Model

- CSS treats every element as a box consisting of:
  - **Content**
  - **Padding**
  - **Border**
  - **Margin**
- The box model defines the layout and design of elements like text and images.

---

## Flexbox

- Flexbox is a CSS layout module designed to arrange elements in a responsive way.
- It eliminates the need for float or positioning for layout.
- Works in **one dimension** (row or column).

---

## Grid

- CSS Grid is a layout system using rows and columns.
- Helps create two-dimensional layouts.
- Grid is for **two-dimensional** layout (both rows and columns).
- Note: Flexbox = 1D layout; Grid = 2D layout.

---

## Pseudo-class vs Pseudo-element

- **Pseudo-class** represents a state of an element (e.g., `:hover`, `:visited`, `:checked`).  
  Syntax uses a **single colon**.  
  Example:
  ```css
  a:visited {
    color: red;
  }
  ```

# Web Fundamentals

- **Local Storage**  
  Stores data as key-value pairs in the browser. Data persists until manually cleared.

- **Session Storage**  
  Stores data as key-value pairs per browser tab. Data is cleared when the tab/browser is closed.

- **Cookie**  
  Small pieces of data sent from server to browser, stored and sent with subsequent requests.  
  Example: “Remember my device” functionality on login uses cookies to keep you logged in.

---

## Navigator API

The Navigator API provides information about the browser and device.

- `navigator.geolocation` — Access geolocation info
- `navigator.platform` — Operating system info
- `navigator.language` — User preferred language
- `navigator.userAgent` — Browser and device info string  
  Example: `"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 ..."`
- `navigator.onLine` — Boolean, if browser is online
- `navigator.mediaDevices` — Access camera, mic, screen sharing
- `navigator.credentials` — Manage user credentials

---

## Window and Screen Properties

- `window.innerWidth` — Width of viewport including vertical scrollbar (if present)
- `window.innerHeight` — Height of viewport including horizontal scrollbar (if present)

- `window.screen` object provides screen info:
  - `screen.width`, `screen.height`
  - `screen.availWidth`, `screen.availHeight`
  - `screen.colorDepth`, `screen.pixelDepth`

---

## Document Properties

- `document.documentElement.clientWidth` — Visible viewport width excluding scrollbar
- `document.documentElement.clientHeight` — Visible viewport height excluding scrollbar
- `document.documentElement.scrollTop` — Pixels scrolled vertically
- `document.documentElement.scrollHeight` — Total document height (including offscreen content)
- `document.documentElement.scrollLeft` — Pixels scrolled horizontally
- `document.documentElement.scrollWidth` — Total document width (including offscreen content)

---

## Location API

Properties of `window.location`:

- `href` — Full URL
- `protocol` — Protocol part (e.g., `http:` or `https:`)
- `hostname` — Domain (e.g., `localhost`, `www.example.com`)
- `port` — Port number (e.g., `3000`)
- `pathname` — URL path (e.g., `/path/to/page`)
- `search` — Query string (e.g., `?name=value`)
- `hash` — Fragment identifier (e.g., `#section`)

Example usage:

```js
console.log(window.location.href);
console.log(window.location.protocol);
console.log(window.location.hostname);
console.log(window.location.port);
console.log(window.location.pathname);
console.log(window.location.search);
console.log(window.location.hash);
```
