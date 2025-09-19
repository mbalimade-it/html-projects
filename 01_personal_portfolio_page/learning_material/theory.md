# HTML Document Structure

The HTML document structure is the **blueprint** of how elements are organized. It gives order to all the content, styles, and scripts.

- **`<!DOCTYPE html>`** → tells the browser the HTML version (HTML5).
- **`<html> ... </html>`** → wraps the entire document. Can include the `lang` attribute (for accessibility, SEO, translations).
- **`<head>`** → contains metadata about the page and its resources.
- **`<body>`** → holds all the visible content of the webpage.

---

# Head Section Elements

The `<head>` contains **metadata** about the page and resources.

- **`<meta charset="UTF-8">`** → character encoding (ensures letters, symbols, emojis display correctly across devices). - how do I represent all the letters
- `meta name="viewport" content="width=device-width, initial-scale=1.` - websites were initially made for computers, so narrowing it had to come into play with devices. So this code says, "hey i will handle all my mobile for me, do not handle it for me " because normally it would make the sites big enough to fit computer screen.
- **`<title>`** → page title (shown in the browser tab).
- **`<link>`** → external CSS files.
- **`<style>`** → internal CSS styles.
- **`<script>`** → JavaScript code.
- **SEO metadata** → `<meta name="description" content="...">`.

---

# Basic Text Elements

- **`<h1>` – `<h6>`** → headings (don’t repeat `<h1>`).
- **`<p>`** → paragraph element.
- **`<br>`** → line break (self-closing).
- **`<hr>`** → horizontal line across the page.

---

# Text Formatting

Formatting tags can add **style** or **meaning** (semantics). Screen readers and SEO benefit from semantic usage.

- **`<strong>`** → importance (bold, semantic).
- **`<em>`** → stress emphasis (italic, semantic).
- **`<b>`** → bold (visual only).
- **`<i>`** → italics (visual only).
- **`<u>`** → underline (rare, can be confused with links).
- **`<small>`** → smaller text (fine print, disclaimers).
- **`<mark>`** → highlighted text (yellow background).
- **`<del>`** → deleted content (strikethrough).
- **`<ins>`** → inserted content (underlined, revisions).
- **`<sub>`** → subscript (H₂O).
- **`<sup>`** → superscript (x²).

---

# Links (`<a>` tag)

The `<a>` (anchor tag) is used to create hyperlinks. Anything inside becomes **clickable** (text, images, other HTML).

- **`href` attribute** → tells the browser where the link goes.

Examples:

- External link → `<a href="https://example.com">Visit Example</a>`
- Internal link → `<a href="about.html">About Us</a>`
- Anchor link (page jump) →

  1. Add `id="section2"` to target element.
  2. `<a href="#section2">Go to Section 2</a>`

Types of links:

- **Absolute URL** → full address (`https://site.com/page.html`).
- **Relative URL** → relative path (`../folder/file.html`).
- **Fragment Identifier** → internal jump (`#section`).

**Best practices:**

- Use descriptive link text (good for accessibility & SEO).

  - Bad: “Click here”
  - Good: “Read our Privacy Policy”

- For external links with `target="_blank"`, also add `rel="noopener noreferrer"` for security.
