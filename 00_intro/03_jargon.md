# 🧾 Common Jargon in HTML (Beginner-Friendly)

## 1. **Tag**

- A **tag** is the building block of HTML.
- It usually looks like this: `<p>` or `<h1>`.
- Tags tell the browser what something _is_.

👉 Example:

```html
<p>This is a paragraph.</p>
```

Here, `<p>` is the **opening tag**, and `</p>` is the **closing tag**.

---

## 2. **Element**

- An **element** is the whole thing: opening tag + content + closing tag.
- Think of it as the “package.”

👉 Example:

```html
<p>This is a paragraph.</p>
```

The entire line is a **paragraph element**.

---

## 3. **Attribute**

- An **attribute** adds extra information to an element.
- It lives inside the opening tag.

👉 Example:

```html
<img src="cat.jpg" alt="A cute cat" />
```

- `src="cat.jpg"` → tells the browser where the image is.
- `alt="A cute cat"` → description of the image (important for accessibility).

---

## 4. **Indentation**

- **Indentation** means adding spaces at the beginning of lines to show **structure**.
- It makes your code easier to read.
- Browsers don’t care about spaces, but developers do (clean code = happy team).

👉 Example (bad indentation):

```html
<html>
  <body>
    <h1>Hello</h1>
    <p>Welcome</p>
  </body>
</html>
```

👉 Example (good indentation):

```html
<html>
  <body>
    <h1>Hello</h1>
    <p>Welcome</p>
  </body>
</html>
```

See how the nested parts are pushed to the right? That’s indentation.

---

## 5. **Nesting**

- **Nesting** is when one element sits inside another.
- Like boxes inside boxes.

👉 Example:

```html
<ul>
  <li>Apples</li>
  <li>Bananas</li>
</ul>
```

- `<ul>` = unordered list.
- Inside it are `<li>` elements (list items).
- The `<li>` tags are _nested_ inside `<ul>`.

---

## 6. **Self-closing Tag**

- Some tags don’t need a closing tag.
- They “close themselves.”

👉 Example:

```html
<img src="cat.jpg" alt="A cat" />
<br />
<hr />
```

- `<img />` = image
- `<br />` = line break
- `<hr />` = horizontal line

---

## 7. **Comment**

- A **comment** is a note in your code that the browser ignores.
- Good for leaving instructions or reminders.

👉 Example:

```html
<!-- This is a comment -->
<p>This shows on the page.</p>
```

---

## 8. **Boilerplate**

- **Boilerplate** means a standard starter template.
- It’s the “skeleton” of every HTML page.

👉 Example:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

Every HTML file starts with something like this.

---

## 9. **Semantic HTML**

- “Semantic” means meaningful.
- These are tags that describe _what_ the content is, not just _how it looks_.
- Helps with accessibility and SEO (search engines).

👉 Examples:

```html
<header>Page header</header>
<main>Main content</main>
<footer>Page footer</footer>
```

Instead of using a plain `<div>`, these tags give meaning.

---

## 10. **Viewport**

- The **viewport** is the visible area of a web page on your screen.
- On mobile, it’s smaller; on desktop, it’s bigger.
- You’ll see this line in the `<head>` for responsive design:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

---
