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
